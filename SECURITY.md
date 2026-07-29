# Security Policy

_Default security policy for every public repository of the Palo Alto AI
Research Lab._

## Reporting a vulnerability

**Do not open a public issue for a security problem.**

Use GitHub's private reporting instead: go to the **Security** tab of the
affected repository → **Report a vulnerability**. That opens a private security
advisory visible only to you and the maintainers.

If private reporting is unavailable in that repository, open a private advisory
in [`.github`](https://github.com/Palo-Alto-AI-Research-Lab/.github/security/advisories/new)
and name the affected repo in the body.

## What to expect

- We aim to acknowledge a report within **72 hours**.
- We will tell you plainly whether we can fix it, and when.
- We credit reporters in the fix commit unless you ask us not to.

There is no bug-bounty budget — this is a free, self-funded lab. What we can
offer is a fast, honest answer and public credit.

## Scope

These repositories publish **methods, patterns and sanitized tooling**, not a
hosted service. Most useful reports are about: leaked secrets or personal data in
the published files, prompt-injection paths in the agent patterns we describe,
and scripts that can destroy a user's data when run as documented.

## Уже нашёл проблему? (RU)

Публичный issue не открывай. Вкладка **Security** нужного репозитория →
**Report a vulnerability** — это приватный тред, видим только ты и мы. Ответим в
течение 72 часов и честно скажем, чиним или нет. Особенно ждём сообщений про
утёкшие секреты и персональные данные в опубликованных файлах.
