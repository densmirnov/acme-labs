# Weekly Launch Update

Это полный пример регулярного процесса: от входных данных и первого результата до контракта версии 0.2, второго прогона и решения об упаковке в skill.

Надя Орлова, Product Lead ACME Labs, готовит update перед еженедельным sync. CEO должен за две–три минуты понять статус запуска, три главных риска и решения, требующие его участия.

## Как пройти пример

1. Прочитайте `runs/v0.1/output.md` и зафиксируйте проблемы первого результата.
2. Откройте `workflow-contract.md`: наблюдения первого прогона превращены в правила, проверки и stop conditions.
3. Изучите четыре файла в `inputs/`.
4. Сравните `runs/v0.1/output.md` и `runs/v0.2/output.md`.
5. Откройте `runs/comparison.md` и `run-log.md`, чтобы увидеть связь «сбой → изменение → новый результат».
6. Посмотрите `examples/source-conflict.md`: это отдельный сложный случай, а правило его обработки находится в контракте.
7. Если сценарий уже устойчив, изучите `../../skills/weekly-launch-update/`.
8. Чтобы проверить границы маршрута и принять решение об автоматизации, перейдите в `../../evaluations/weekly-launch-update/`.

## Структура

```text
weekly-launch-update/
  workflow-contract.md
  run-log.md
  inputs/
    approved-launch-goal.md
    current-week-notes.md
    previous-decisions.md
    customer-signals.md
  runs/
    v0.1/output.md
    v0.2/output.md
    comparison.md
  examples/
    source-conflict.md
```

## Источники правды

- Общие правила среды: `../../AGENTS.md` и `../../policies/`.
- Логика процесса: `workflow-contract.md`.
- Данные конкретного цикла: `inputs/`.
- История изменений: `run-log.md`.
- Упакованный повторяемый навык: `../../skills/weekly-launch-update/`.

Не редактируйте старый результат, чтобы сделать его «лучше». Создавайте новый прогон и фиксируйте, какое изменение процесса повлияло на результат.
