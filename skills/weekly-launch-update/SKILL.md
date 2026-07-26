---
name: weekly-launch-update
description: This skill should be used when the user asks to "подготовить weekly launch update", "сделать еженедельное обновление по запуску", "написать update для CEO", "собрать статус запуска", "выделить риски запуска", "подготовить статус по проекту", or "prepare a weekly launch update". It creates concise launch status updates from project context, weekly changes, risks, blockers, and decisions needed from leadership.
version: 0.2.0
---

# Weekly Launch Update Skill

## Purpose

Prepare a concise weekly launch update for a CEO, founder, product lead, or project leadership group. Convert launch context, weekly changes, customer signals, risks, blockers, previous decisions, and open questions into a structured update that supports decision-making.

Use this skill for recurring launch or project-status communication, not for one-off strategic planning, long-form PRDs, investor updates, or general marketing copy.

## Trigger

Apply this skill when the user asks to:

- prepare a weekly launch update;
- write an update for CEO or leadership;
- summarize launch progress for the week;
- identify launch risks and decisions needed;
- turn project notes into a structured status update;
- prepare a status update before a weekly sync.

## Required Inputs

Collect or infer the following inputs before producing the update:

1. Launch goal or project objective.
2. Current launch status.
3. Changes since the previous update.
4. Key achievements or progress signals.
5. Current risks and blockers.
6. Decisions made last week.
7. Decisions needed from CEO, founder, or team.
8. Relevant customer, market, product, or engineering signals.
9. Known gaps in the available data.

If an input marked as required by the workflow contract is missing, stop and request it. If only optional context is missing, proceed with available data and explicitly list gaps in the final section. Do not invent facts to fill missing context.

## Process

1. Read the launch goal and current project context.
2. Identify what changed since the previous update.
3. Separate facts from assumptions.
4. Summarize the current launch status in 2–4 sentences.
5. Extract the most important achievements or progress signals.
6. Identify the three most important risks.
7. Identify blockers that require attention.
8. Identify decisions needed from CEO, founder, or team.
9. Produce the update in the required format.
10. List missing data explicitly.

## Output Format

Produce the result in Markdown:

```markdown
# Weekly Launch Update

## 1. Краткий статус

## 2. Что изменилось за неделю

## 3. Главные достижения

## 4. Три главных риска

## 5. Блокеры

## 6. Решения, которые нужны

## 7. Следующие шаги

## 8. Пробелы в данных
```

Keep the update short. Target 1–2 pages maximum. Prefer direct operational language over narrative or promotional language.

## Constraints

- Do not invent facts, dates, client names, metrics, or decisions.
- Do not hide uncertainty in polished language.
- Do not use real client names unless explicitly allowed.
- Do not turn the update into a long report.
- Do not bury risks in the middle of the text.
- Do not write generic phrases such as “the team is actively working”.
- Do not present assumptions as confirmed facts.
- Stop before generation when the workflow contract requires a missing source.
- Stop when raw personal or client-identifying data is present.

## Quality Criteria

The update is good if:

- leadership understands launch status in 2–3 minutes;
- risks are explicit and prioritized;
- decisions needed from leadership are clear;
- blockers are separated from general risks;
- next steps are concrete;
- missing data is named directly;
- the text can be sent after minimal editing.

## Additional Resources

Consult these files when more detail is needed:

- `../../workflows/weekly-launch-update/workflow-contract.md` — source workflow and control logic used in ACME Labs.
- `references/rubric.md` — detailed quality rubric for evaluating outputs.
- `references/openapi-usage.md` — when and how an OpenAPI file belongs in a skill package.
- `examples/normal-week.md` — example input and output for a normal launch week.
- `examples/risky-week.md` — example input and output for a risky launch week.
- `openapi/acme-launch-data.openapi.yaml` — optional example API schema for retrieving launch data. Use only when external launch-data APIs are part of the workflow.
