# Credits

Идея — тоже вклад. Ниже люди, чей совет мы взяли в работу, и что именно из него выросло.
Файл пересобирается из реестра `alpha_credit.py`, руками не правится.

- **Артём Холомянский** ([источник](https://t.me/ClawRus/16237)) — стандарт ANSS: писать ТЗ для агентов, а не для людей -- слой инструкций, механизм ревью, правила менять существующий код не ломая живое  
  Применено: идея принята, внедрение НЕ доказано (trial drop 06.08); честно сказано автору: https://github.com/Kholomyanskiy/anss-standard/issues/1
- **guglielmo-san (guglielmo-san)** ([источник](https://github.com/modelcontextprotocol/go-sdk/pull/1148)) — Убрать пояснительный абзац из quick_start — в доках go-sdk держат однострочный фикс без объяснений причины  
  Применено: https://github.com/modelcontextprotocol/go-sdk/pull/1148 (MERGED, docs/quick_start.md + internal/docs/quick_start.src.md)
- **Kirill Simakov** ([источник](https://www.facebook.com/AntonyDzi/posts/pfbid02pq6VDVLtu3pxD3PhqaNpuZJqt2kgs2ghhUKDXgLkavXpDG1ETW2eT6wBeYLT6ipDl)) — поверх данных нужна отдельная структура под быструю вычитку контекста  
  Применено: decision-always-on-memory-architecture (25.06) + memory always-on-memory-pilot + brain_ask.py Phase 2
- **LHMQ878 (@LHMQ878)** ([источник](https://github.com/openai/openai-agents-python/pull/3998#issuecomment-5160678412)) — Наш claim про non-tripwire guardrail exception — не регрессия, а design question; переформулировали ровно так в ответе 06.08  
  Применено: https://github.com/openai/openai-agents-python/pull/3998#issuecomment-5207474141
- **Pranav Mishra (@PranavMishra28)** ([источник](https://github.com/openai/openai-agents-python/pull/3998#pullrequestreview-4841599693)) — Over-capture в stop_on_first_tool: deferral нельзя распространять на tool-items — вошло в наш разбор мержа  
  Применено: https://github.com/openai/openai-agents-python/pull/3998#issuecomment-5207474141 (раздел @PranavMishra28's stop_on_first_tool case)
- **Eugeniu Ghelbur (@eugeniughelbur)** ([источник](https://github.com/eugeniughelbur/obsidian-second-brain/issues/171#issuecomment-5114817512)) — Отчёт о работе сборки = вставляй ЧТО ЗАПУСТИЛ и ЧТО НАПЕЧАТАЛО, а не вывод; применили в обоих своих отчётах  
  Применено: https://github.com/eugeniughelbur/obsidian-second-brain/issues/171#issuecomment-5207484648 + https://github.com/openai/openai-agents-python/pull/3998#issuecomment-5207474141
- **babyblueviper1 (@babyblueviper1)** ([источник](https://github.com/microsoft/semantic-kernel/pull/14199#issuecomment-5089457783)) — asyncio.gather диспатчит батч целиком, а terminate читается после — политику надо оценивать ДО диспатча; починили в 24a82d3 (batch hold)  
  Применено: microsoft/semantic-kernel@24a82d3 (в закрытом PR не числится) + issuecomment-5208770978
- **rpelevin (@rpelevin)** ([источник](https://github.com/microsoft/semantic-kernel/pull/14199)) — Пускать в батч только независимо ALLOWed вызовы, приостанавливая лишь требующие апрува — уточнённая форма фикса гонки  
  Применено: microsoft/semantic-kernel@24a82d3b685cc772e2cbc06600936210cdf26d6a
- **Teng Ling (teng-lin)** ([источник](https://github.com/teng-lin/notebooklm-py)) — notebooklm-py: OSS CLI, управляющий NotebookLM из терминала -- фундамент, на котором стоит наш скилл /notebooklm  
  Применено: C:/Users/Anton/.claude/skills/notebooklm/SKILL.md
- **itechmeat (itechmeat)** ([источник](https://github.com/itechmeat/open-second-brain)) — open-second-brain: общая память между OpenClaw/Claude Code/Codex -- признан ближайшим эталоном нашего слоя общего мозга  
  Применено: E:/Obsidian/Anton-Knowledge/05-Resources/Research/research-shared-brain-multi-person-agents.md

_Собрано 2026-08-06. Просьба убрать имя выполняется в тот же день: напишите нам, и строка исчезнет при ближайшей пересборке._
