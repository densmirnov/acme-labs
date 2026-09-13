# Context layer blueprint

| Layer | Folder | ACME example | Purpose |
|---|---|---|---|
| Sources | `02_sources/` | Pointers to original context, policies, and workflow inputs | Preserve where information came from |
| Representations | `03_representations/` | Structured customer-signal view | Make source material easier to use without changing its authority |
| Canonical context | `04_canonical_context/` | Product goal and policies | Reuse stable approved rules across tasks |
| Current context | `05_current_context/` | Weekly notes, decisions, and signals | Keep time-bound state separate from stable rules |
| Context capsules | `06_context_capsules/` | Weekly Launch Update capsule | Select only what one task needs |
| Runs | `07_runs/` | Pointers to existing versioned outputs | Preserve results and observations without rewriting history |

## Update rules

- Update canonical context only when the corresponding source-of-truth decision changes.
- Create a new current-period input rather than overwriting an old period.
- Keep source links and transformation notes with each representation.
- Resolve conflicts using the workflow contract; if it has no applicable rule, stop for human review.
- A capsule is a selection manifest, not a new source of truth.

