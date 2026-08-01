# AI contributors — how we credit the models that work here

_Applies to every public repository of the Palo Alto AI Research Lab.
Policy adopted 2026-07-31; commits before that date carry Claude credits only,
though other models were already in the workflow._

This lab is a human + AI team, and we say so in the git history rather than in
marketing copy. AI involvement is recorded with commit trailers — **self-reported
by us, the committers**. GitHub does not verify who did the work. These trailers
are our process log, kept honest by one rule:

> **A credit goes on a commit only if that model's output changed the committed content.**

No decorative credits. A model that did not touch the work does not appear.

## Roles and credits

| Model | Role | Credit |
|---|---|---|
| **Claude** (Anthropic, via Claude Code) | Writes most of the code and docs | `Co-authored-by: Claude <noreply@anthropic.com>` |
| **Codex** (OpenAI) | Reviewer — executable changes go through it before we call them done | `Co-authored-by: Codex <267193182+codex@users.noreply.github.com>`, only when its review produced actual edits in that commit |
| **Grok** (xAI) | Second review rail | `Reviewed-by: Grok (xAI)` in the commit body, same only-if-it-changed-things rule. No co-author trailer: xAI publishes no GitHub identity for Grok, and we will not invent an address on someone else's domain |
| **Gemini** (Google) | Deep-research fan-out | research alone does not edit files, so no co-author trailer — credit goes in the commit body when its findings shaped the change |

Models we do not run in our pipeline do not get credits here, however good they are.

## The fine print

- `Co-authored-by` is GitHub's trailer for multiple authors. We apply it when a
  model wrote content, or when its review comments were incorporated — i.e. its
  words ended up shaping the diff. Review that produced no changes, and
  background research, get a line in the commit body instead.
- A co-author trailer needs a real e-mail identity. Claude and Codex have
  vendor-published GitHub accounts; models whose vendor publishes none get
  body-line credit until that changes.
- When GitHub associates a trailer e-mail with an account, it may show that
  account's avatar on the commit and in contributor surfaces. That display means
  *"the committer credited this identity"* — nothing more. It is not a vendor
  endorsement, not GitHub-verified provenance, and not a claim of legal authorship.
- `git log -i --grep 'co-authored-by: codex'` lists the commits where **we recorded**
  that model's involvement. Trust it as far as you trust our process log — which
  this document exists to keep auditable.

## How this relates to human contributors

The same principle, pointed the other way: humans keep copyright and credit for
everything they write ([CONTRIBUTING.md](CONTRIBUTING.md) — no CLA, ever), and
models get named for work they actually did. Nobody, carbon or silicon, gets
credit for work they did not do.

## Why we bother

We are building an AI digital twin in public. The AIs are not tools we hide —
they are the co-workers this whole body of work is about. Per-commit credits keep
the record honest in both directions and make the claim checkable by anyone with
`git log`.
