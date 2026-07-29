# Contributing

_Default contributing guide for every public repository of the Palo Alto AI
Research Lab. A repository with its own `CONTRIBUTING.md` overrides this one._

This is an open build. A pattern, a fix, a test, a typo — pull requests are
welcome. No CLA, no corporate paperwork.

## The one gate: AK-47

Every contribution is checked against a single principle — **AK-47 simplicity**:

1. **Simple** — the smallest thing that solves the problem.
2. **Repairable with a hammer** — a non-engineer should be able to understand
   and fix it.
3. **Survives bad conditions** — flaky connection, token limits, no fancy infra.
4. **Useful to a normal person** — not only to programmers.

If a change adds a dependency, a service, or an abstraction, say in one line:
what pain it removes, what breaks without it, and the cheaper alternative you
considered.

## How

1. **Open an issue first** for anything non-trivial — let's agree on the shape
   before you write code.
2. **Keep PRs small.** One idea per PR.
3. **Explain the "why"** in plain words, not in jargon.
4. **No secrets, no personal data, no real third-party names** in code, tests,
   or examples — use synthetic data.
5. **If it is executable, prove it runs.** Paste the command you ran and its
   output in the PR body. "Should work" is not a test.

## What happens next

We read every issue and PR and answer in the thread — including "no, and here is
why". Silence is a bug on our side; ping the thread if we go quiet.

## Questions

Not sure whether something fits? Ask **before** you build it — open an issue in
the repo you want to change, or in
[`.github`](https://github.com/Palo-Alto-AI-Research-Lab/.github/issues) if it is
about the lab in general.

---

# Как контрибьютить (RU)

Это открытая стройка. Правка, тест, фикс, исправленная опечатка — присылай PR.
Никаких CLA и корпоративных бумажек.

## Единственные ворота: АК-47

1. **Просто** — самое маленькое решение, которое закрывает проблему.
2. **Чинится молотком** — не-инженер должен понять и починить сам.
3. **Живёт в плохих условиях** — кривая связь, лимиты токенов, нет красивой
   инфраструктуры.
4. **Полезно обычному человеку**, а не только программисту.

Добавляешь зависимость, сервис или абстракцию — одной строкой напиши: какую боль
это лечит, что сломается без неё, какую дешёвую альтернативу ты рассмотрел.

## Как

1. **Сначала issue**, если задача нетривиальная — договоримся о форме до кода.
2. **Маленькие PR.** Одна идея — один PR.
3. **Объясняй «зачем»** простыми словами.
4. **Никаких секретов, персональных данных и настоящих чужих имён** в коде,
   тестах и примерах — только синтетика.
5. **Собрал исполняемое — докажи, что работает:** команда, которую ты запускал,
   и её вывод прямо в теле PR. «Должно работать» тестом не считается.

## Что будет дальше

Мы читаем каждый issue и каждый PR и отвечаем в треде — в том числе «нет, вот
почему». Молчание с нашей стороны — это баг, пни тред.

## Вопросы

Не уверен, подходит ли идея? Спроси **до** того, как строить: открой issue в том
репозитории, который хочешь менять, или в
[`.github`](https://github.com/Palo-Alto-AI-Research-Lab/.github/issues), если
вопрос про лабораторию в целом.
