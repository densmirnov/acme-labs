# Учебные маршруты ACME

Оба занятия используют одну компанию, один набор источников и общие правила.

- [Вебинар об ИИ-среде](ai-workspace.md): собрать рабочую среду, повторить процесс, разобрать версии, skill и проверку устойчивости.
- [Воркшоп о контекстном слое](context-layer/README.md): выбрать задачу, подготовить знания и правила, собрать пакет, выполнить и проверить одну правку.

## Куда переехал прежний context-layer/

Отдельная папка была учебной схемой поверх существующих документов. Теперь общие знания живут в `context/`, правила — в `policies/`, пакет и результаты — у своего процесса. Материалы обучения находятся в `workshops/`.

| Прежний путь внутри context-layer/ | Текущее место |
|---|---|
| `README.md`, `00_START_HERE.md` | [Начало воркшопа](context-layer/README.md) |
| `AGENTS.md` | [Общие инструкции](../AGENTS.md) |
| `01_cards/01_use_case_and_sources.md` | [Задача и источники](context-layer/01_use_case_and_sources.md) |
| `01_cards/02_context_layer_blueprint.md` | [Знания и правила](context-layer/02_context_layer_blueprint.md) |
| `01_cards/03_use_and_improve.md` | [Запуск и проверка](context-layer/03_use_and_improve.md) |
| `02_sources/` | [Карта оригиналов](../context/README.md) |
| `03_representations/customer_signal.md` | [Представление клиентских сигналов](../context/representations/customer-signals.md) |
| `04_canonical_context/` | [Контекст компании](../context/README.md), [политики](../policies/), [правила применения](../context/decision-rules.md) |
| `05_current_context/` | [Входы учебного периода](../workflows/weekly-launch-update/inputs/) |
| `06_context_capsules/weekly_launch_update.md` | [Пакет задачи](../workflows/weekly-launch-update/context-capsule.md) |
| `07_runs/` | [История процесса](../workflows/weekly-launch-update/runs/) и [журнал](../workflows/weekly-launch-update/run-log.md) |

Семь пронумерованных папок остаются удобной схемой для отдельной рабочей папки участника. Общему репозиторию компании не нужно хранить рядом второе дерево с копиями тех же материалов. Папка `workshops/context-layer/` содержит только учебный маршрут и три рабочих документа.

Пути старого вебинара `context/`, `policies/`, `workflows/`, `skills/`, `evaluations/` и `templates/workspace/` сохранены. Для просмотра прежнего дерева `context-layer/` по старой записи занятия доступен [снимок до объединения](https://github.com/densmirnov/acme-labs/tree/08eee79730b9698476d8ced4f95bb7fe45bfeb3e/context-layer). Ссылки на этот commit продолжают указывать на исходную версию.
