# docs-site — how a repo of this lab gets a documentation page

One static page per repo, served by GitHub Pages out of `docs/`. No framework, no build step, no
generator: the page is a file a human can open in a text editor and fix. Two are live and were
written from this template — [claude-bible](https://palo-alto-ai-research-lab.github.io/claude-bible/)
and [verbatim-citation-gate](https://palo-alto-ai-research-lab.github.io/verbatim-citation-gate/).

`template.html` is the starting point, not a shared runtime dependency: you **copy** it into your
repo and fill the `{{slots}}`. Nothing links back to this file at runtime, so a repo's page can
never break because something here changed.

## Recipe (about 30 minutes, most of it writing)

1. `cp` this `template.html` to `docs/index.html` in your repo and `touch docs/.nojekyll`.
   The `.nojekyll` file is not decoration: without it GitHub runs Jekyll over the directory, and a
   markdown file with brace syntax in it can fail the build and take the whole page down.
2. Replace every `{{slot}}`. `grep -c '{{' docs/index.html` must return **0** before you commit.
3. Check the branch in every GitHub link. This lab has repos on `main` **and** on `master`
   (`gh api repos/Palo-Alto-AI-Research-Lab/<repo> -q .default_branch`). A hardcoded `/blob/main/`
   404s silently on a `master` repo — it happened on the first page shipped from this template.
4. Enable Pages:
   `gh api -X POST repos/Palo-Alto-AI-Research-Lab/<repo>/pages -f "source[branch]=<branch>" -f "source[path]=/docs"`
   then set the repo homepage to the resulting URL so the link shows on the repo page:
   `gh api -X PATCH repos/Palo-Alto-AI-Research-Lab/<repo> -f homepage="https://palo-alto-ai-research-lab.github.io/<repo>/"`
5. Add the page to the site sitemap: one line in `PROJECT_PAGES` in
   [`tools/build_site.py`](https://github.com/Palo-Alto-AI-Research-Lab/Palo-Alto-AI-Research-Lab.github.io/blob/main/tools/build_site.py)
   of the site repo, then run it. A page nothing points at is a page no crawler finds.
6. Add a live check: one line in `EXTRA_SURFACES` in `~/.claude/scripts/public_surface_audit.py`,
   with a **substring from the body** as the marker. A 200 proves the server answered, not that the
   page has content.
7. Verify **anonymously**, from outside: `curl -s <url> | grep '<title>'`. Published is not visible;
   only a stranger's request proves the page is up.

## What the page must contain

Not a style rule — these are the sections that make a docs page worth linking to:

- **A title under about 60 characters and a description under 160.** They are what a search result
  shows; longer text is cut off mid-sentence.
- **`<link rel="canonical">`, Open Graph and Twitter meta.** Without them a shared link renders as a
  bare URL.
- **An install command you have run today.** If the package is not published yet, say that on the
  page and give the command that works. A first command that fails costs you the reader.
- **A "known limits" section naming every open defect, each linked to its issue.** This is the
  section that makes the rest of the page believable, and the one a maintainer reading your PR
  notices. Omitting a known failure mode is a lie by layout.
- **The contribution deal**, matching [CONTRIBUTING.md](../CONTRIBUTING.md): the `accepted` queue,
  "claiming this", 7 days, 48-hour answer, and copyright staying with the author.

## Who this is waiting for

`agent-runtime-integrity-bench` (benchmarks) and `second-brain-starter-kit` (starter kits) are the
next two flagships in line for a page. Their Pages are deliberately **not** enabled yet: a live but
empty docs page is worse than none — it indexes, it disappoints, and it makes everything next to it
look thinner. Fill the template first, then flip the switch.
