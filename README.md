# .github — default community health files

This repository holds the **default** community documents for every public
repository of the [Palo Alto AI Research Lab](https://github.com/Palo-Alto-AI-Research-Lab).

| File | Applies to | Overridable |
|---|---|---|
| [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) | all public repos | yes — a repo's own copy wins |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | all public repos | yes |
| [`SECURITY.md`](SECURITY.md) | all public repos | yes |
| [`SUPPORT.md`](SUPPORT.md) | all public repos | yes |

## Why one source instead of a copy per repo

GitHub falls back to these files whenever a repository does not ship its own.
One file, one place to fix — a copy in twelve repositories is twelve chances to
drift. `LICENSE` is deliberately **not** here: GitHub does not inherit licenses,
so every repository must carry its own.

## How it is enforced

A deterministic gate walks every public non-fork repository we own and fails if a
required document is missing — neither in the repo nor inherited from here. It
runs on our hub, not inside any of these repositories, so a broken repo cannot
silence its own watchdog.

## Contact

Questions about the lab in general: [open an issue here](https://github.com/Palo-Alto-AI-Research-Lab/.github/issues).
Questions about a specific project: open an issue in that project.

Prefer to talk to a human directly: WhatsApp +1 341 222 9178 · X [@Tony_Stef_](https://x.com/Tony_Stef_) · Telegram [@ClawRus](https://t.me/ClawRus) (RU) / [@ClawEng](https://t.me/ClawEng) (EN).

---

## По-русски

Здесь лежат документы **по умолчанию** для всех наших публичных репозиториев:
кодекс поведения, гайд для контрибьюторов, политика безопасности и страница
поддержки. GitHub сам подставляет их в любой репозиторий, где нет своей копии, —
один источник вместо двенадцати копий, которые разъезжаются. `LICENSE` сюда не
кладём: лицензия по наследству не работает, она обязана лежать в каждом
репозитории отдельно.
