# Contributing

_The contribution deal for every public repository of the Palo Alto AI Research Lab._

This is an open build. A pattern, a fix, a test, a typo — pull requests are welcome.
**No CLA. No copyright assignment. No corporate paperwork. Ever.**

## Your code stays yours

We think the contributor-agreement habit is backwards, so we do not have one.

- **You keep the copyright** to everything you write. We never ask you to sign it over.
- **Inbound = outbound.** Your contribution is licensed under the same license the repository
  already carries (MIT unless the repo says otherwise) — the same terms as our own code, no
  special rights for us.
- **We will never relicense your work into a closed product.** If the license of a repo ever
  changes, we ask every contributor whose code is in it, by name, and anyone who says no keeps
  their code under the terms they contributed it under.
- **You get the credit.** Your name stays on the commit, goes into the release notes, and into
  `CONTRIBUTORS.md`. If your idea shaped a change we wrote ourselves, we credit you in the issue
  and in the changelog.

## Take an issue: the `accepted` queue

You should never have to guess whether we want your work.

| Label | What it means |
|---|---|
| `accepted` | **We want this and it is free to take.** Scope is agreed, no one is on it. |
| `good first issue` | `accepted` + small and self-contained. Start here if you are new. |
| `help wanted` | We want it but haven't scoped it yet — comment and we'll shape it with you. |
| `claimed` | Someone is on it. Don't duplicate the work; ask to pair instead. |

**How to claim:**

1. Find an issue labelled `accepted`. Comment **"claiming this"** — that's it, no permission needed.
2. We label it `claimed` and it is yours for **7 days**.
3. Open a PR, or drop one line in the thread if you need longer. Asking for more time always works.
4. Silence for 7 days → we remove `claimed` and it goes back to the pool. No hard feelings, no
   explanation owed. Come back whenever.

**Nothing in the queue fits?** Open an issue describing what you want to change. We answer with
`accepted` (go ahead), a counter-proposal, or an honest "no, because…" — *before* you write code, so
nobody's evening gets wasted.

## What we owe you

- **An answer within 48 hours** on every issue and PR, including "no, and here is why".
  Our silence is our bug — ping the thread, it is not rude.
- **A review that reads your code**, not a drive-by nit.
- **A merge or a real reason.** A PR that dies quietly in the queue is a failure on our side.

## The one gate: AK-47

Every contribution is checked against a single principle — **AK-47 simplicity**:

1. **Simple** — the smallest thing that solves the problem.
2. **Repairable with a hammer** — a non-engineer should be able to understand and fix it.
3. **Survives bad conditions** — flaky connection, token limits, no fancy infra.
4. **Useful to a normal person** — not only to programmers.

If a change adds a dependency, a service, or an abstraction, say in one line: what pain it removes,
what breaks without it, and the cheaper alternative you considered.

## House rules

1. **Keep PRs small.** One idea per PR.
2. **Explain the "why"** in plain words, not in jargon.
3. **No secrets, no personal data, no real third-party names** in code, tests, or examples — use
   synthetic data.
4. **If it is executable, prove it runs.** Paste the command you ran and its output in the PR body.
   "Should work" is not a test.
5. **Tell us if an AI wrote it.** We build with AI agents every day and think that's fine — but say
   so, and make sure you understand and have run what you're sending. Unreviewed generated code is
   the one thing we will close on sight.

## Questions

Not sure whether something fits? Ask **before** you build it — open an issue in the repo you want to
change, or in [`.github`](https://github.com/Palo-Alto-AI-Research-Lab/.github/issues) if it is about
the lab in general.

---

# Как контрибьютить (RU)

Это открытая стройка. Правка, тест, фикс, исправленная опечатка — присылай PR.
**Никакого CLA. Никакой передачи прав. Никаких корпоративных бумажек. Никогда.**

## Твой код остаётся твоим

Мы считаем привычку с contributor-agreement вывернутой наизнанку, поэтому её у нас нет.

- **Копирайт остаётся у тебя** на всё, что ты написал. Мы не просим его переписать на нас.
- **Inbound = outbound.** Твой вклад лицензируется на тех же условиях, что уже стоят на
  репозитории (MIT, если в репо не сказано иное) — ровно как наш собственный код, без особых прав
  для нас.
- **Мы никогда не перелицензируем твою работу в закрытый продукт.** Если лицензия репо когда-то
  поменяется, мы спросим поимённо каждого, чей код внутри, и чей ответ «нет» — тот остаётся на тех
  условиях, на которых вносил.
- **Кредит твой.** Имя остаётся в коммите, попадает в release notes и в `CONTRIBUTORS.md`. Если
  твоя идея легла в изменение, которое написали мы, — кредит в issue и в чейнджлоге.

## Как взять задачу: очередь `accepted`

Ты не должен гадать, нужна ли нам твоя работа.

| Лейбл | Что значит |
|---|---|
| `accepted` | **Нам это нужно, и задача свободна.** Форма согласована, никто не занят. |
| `good first issue` | То же `accepted`, только маленькое и самодостаточное. Начинать отсюда. |
| `help wanted` | Хотим, но форму ещё не придумали — напиши, придумаем вместе. |
| `claimed` | Кто-то уже делает. Не дублируй — предложи пару. |

**Как забрать:**

1. Находишь issue с лейблом `accepted`. Пишешь в тред **«claiming this»** — всё, разрешения не нужно.
2. Мы вешаем `claimed`, и задача твоя на **7 дней**.
3. Открываешь PR — или роняешь строку в тред, если нужно больше времени. Попросить время можно всегда.
4. Тишина 7 дней → снимаем `claimed`, задача возвращается в общий котёл. Без обид и без объяснений
   с твоей стороны. Возвращайся когда угодно.

**Ничего не подошло?** Открой issue с тем, что хочешь поменять. Мы ответим `accepted` (бери),
встречным предложением или честным «нет, потому что…» — **до** того, как ты напишешь код, чтобы
ничей вечер не пропал зря.

## Что мы должны тебе

- **Ответ за 48 часов** на каждый issue и каждый PR, включая «нет, и вот почему».
  Наше молчание — это наш баг, пни тред, это не невежливо.
- **Ревью, которое читает твой код**, а не придирку на бегу.
- **Мерж или настоящую причину.** PR, тихо умерший в очереди, — провал с нашей стороны.

## Единственные ворота: АК-47

1. **Просто** — самое маленькое решение, которое закрывает проблему.
2. **Чинится молотком** — не-инженер должен понять и починить сам.
3. **Живёт в плохих условиях** — кривая связь, лимиты токенов, нет красивой инфраструктуры.
4. **Полезно обычному человеку**, а не только программисту.

Добавляешь зависимость, сервис или абстракцию — одной строкой напиши: какую боль это лечит, что
сломается без неё, какую дешёвую альтернативу ты рассмотрел.

## Домашние правила

1. **Маленькие PR.** Одна идея — один PR.
2. **Объясняй «зачем»** простыми словами.
3. **Никаких секретов, персональных данных и настоящих чужих имён** в коде, тестах и примерах.
4. **Собрал исполняемое — докажи, что работает:** команда, которую ты запускал, и её вывод прямо в
   теле PR. «Должно работать» тестом не считается.
5. **Скажи, если писал ИИ.** Мы сами строим с ИИ-агентами каждый день и считаем это нормой — но
   скажи об этом и убедись, что понимаешь и прогнал то, что присылаешь. Непрочитанный
   сгенерированный код — единственное, что мы закроем не глядя.

## Вопросы

Не уверен, подходит ли идея? Спроси **до** того, как строить: открой issue в том репозитории,
который хочешь менять, или в
[`.github`](https://github.com/Palo-Alto-AI-Research-Lab/.github/issues), если вопрос про
лабораторию в целом.
