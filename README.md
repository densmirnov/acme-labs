# ACME Labs

Рабочий репозиторий ACME Labs: знания о компании и PolicyOS, материалы AI Workspace Layer, правила работы и история процессов.

**Начать работу:** [context-layer/00_START_HERE.md](context-layer/00_START_HERE.md).

## Контекстный слой

```text
context-layer/
  00_START_HERE.md              состояние работы и следующее действие
  AGENTS.md                    правила работы агента со слоем
  01_cards/                    задача и источники → знания и правила → запуск и проверка
  02_sources/                  первичные материалы и входы периода
  03_representations/          подготовленные представления источников
  04_canonical_context/        компания, продукт, роли и действующие правила
  05_current_context/          состояние направления и выбранный период
  06_context_capsules/         пакеты контекста для конкретных задач
  07_runs/                     запросы, входы, ответы, проверки и изменения
```

В каждом разделе находятся рабочие материалы. Три документа в `01_cards/` связывают их по источникам, основаниям правил и выполненным запускам. Исходник, его представление, действующее правило и ответ агента сохраняют разные роли.

## Работа команды

| Задача | Материал |
|---|---|
| Войти в контекст компании | [Компания](context-layer/04_canonical_context/company-profile.md), [PolicyOS](context-layer/04_canonical_context/product-overview.md), [роль Нади](context-layer/04_canonical_context/people/nadya-orlova.md) |
| Узнать состояние направления | [AI Workspace Layer: текущий срез](context-layer/05_current_context/launch_state.md) |
| Подготовить отчёт CEO | [Пакет Weekly Launch Update](context-layer/06_context_capsules/weekly_launch_update.md) и [контракт процесса](workflows/weekly-launch-update/workflow-contract.md) |
| Проверить происхождение сведений | [Реестр источников](context-layer/01_cards/01_use_case_and_sources.md) |
| Изменить контекст | [Схема, правила и обновление](context-layer/01_cards/02_context_layer_blueprint.md) |
| Проверить результат изменения | [Запуск и проверка](context-layer/01_cards/03_use_and_improve.md), [история запусков](context-layer/07_runs/README.md) |
| Продолжить проработку продукта | [Поручение CEO](context-layer/02_sources/company/ceo-email-launch-request.md), [working brief](documents/ai-workspace-layer-brief-2026-05-05.md) |

Последний период бизнес-данных — **18–22 мая 2026 года**. Даты выполнения агентных задач хранятся отдельно от периода источников.

## Процессы и инструменты

- [workflows/](workflows/) — контракты и порядок выполнения процессов; контекст, пакеты и результаты находятся в соответствующих слоях.
- [skills/](skills/) — инструкции агента для повторяемых задач.
- [evaluations/](evaluations/) — контрольные случаи, критерии и решения об автоматизации.
- [documents/](documents/README.md) — рабочие документы для обсуждения и согласования.
- [templates/](templates/) — заготовки новых процессов.

## Задание агенту

```text
Прочитай AGENTS.md и context-layer/AGENTS.md.
Выполни задачу по context-layer/06_context_capsules/weekly_launch_update.md.
Сохрани новый черновик, запрос, версии входов и проверку в
context-layer/07_runs/weekly-launch-update/<run-id>/.
Добавь наблюдение в журнал и обнови точку продолжения.
```

Надя проверяет факты, приоритет рисков и решения перед отправкой CEO. Изменение файла не заменяет утверждение владельцем.
