# Example: Risky Launch Week

## Inputs

Launch goal: validate AI Workspace Layer as a new product direction within 90 days.

Weekly changes:

- Two customer calls confirmed interest in team-level AI workflows.
- Engineering raised concerns about access control for shared context.
- Sales wants a demo for a client next week, but product scope is not stable.
- Customer notes include sensitive client names and cannot be used directly.

Previous decisions:

- Use ACME Labs demo environment for early customer conversations.

Open questions:

- Who approves data boundaries for demo materials?
- Can Sales show the demo before Engineering validates access assumptions?

## Expected Output

# Weekly Launch Update

## 1. Краткий статус

Запуск остаётся перспективным, но на этой неделе появились существенные риски по scope, данным и срокам внешнего демо. Клиентский интерес подтверждается, но команда пока не готова безопасно показывать рабочий контур без уточнения границ данных и доступа.

## 2. Что изменилось за неделю

- Два клиентских разговора подтвердили интерес к командным AI workflows.
- Engineering поднял вопрос access control для общего контекста.
- Sales хочет показать демо клиенту уже на следующей неделе.
- Клиентские заметки требуют обезличивания.

## 3. Главные достижения

- Подтверждён интерес к командному уровню продукта.
- Выявлен ключевой инфраструктурный риск: права доступа к общему контексту.
- Появился потенциальный внешний демо-кейс.

## 4. Три главных риска

1. Риск показать демо раньше, чем определены границы данных.
2. Риск расширить scope из demo workspace в полноценную платформу доступа.
3. Риск использовать клиентские заметки без достаточного обезличивания.

## 5. Блокеры

- Нет утверждённых data boundaries для демо.
- Неясно, кто принимает решение о готовности демо для клиента.

## 6. Решения, которые нужны

- Решить, можно ли Sales показывать демо клиенту на следующей неделе.
- Назначить владельца data boundary для демо-материалов.
- Подтвердить, что до проверки access control демо остаётся sandbox-only.

## 7. Следующие шаги

- Обезличить customer notes.
- Согласовать data boundary checklist.
- Подготовить безопасную версию demo flow.

## 8. Пробелы в данных

- Нет оценки Engineering по срокам минимального access-control слоя.
- Нет финального списка материалов, допустимых для внешнего демо.
