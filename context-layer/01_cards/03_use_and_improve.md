# Use and improve

## First use

Ask an agent to prepare the Weekly Launch Update using `06_context_capsules/weekly_launch_update.md`. The expected format and stop conditions come from the linked workflow contract and policies.

## Quality checks

- Every material claim can be traced to an included source.
- Facts, signals, assumptions, conflicts, and missing data remain distinct.
- The result names the status, top risks, blockers, and decisions needed.
- A stop condition produces an explicit stop, not a plausible completion.

## Improvement loop

1. Add or update the real source without changing earlier source snapshots.
2. Preserve provenance and update the relevant representation.
3. Revise the capsule only if the task needs different context.
4. Run the agent in a separate execution context.
5. Save the output and observation as a new run.
6. Change a rule only when the observation justifies it.

The mature v0.1/v0.2 comparison already present in ACME is an optional illustration of this loop, not a required route produced by the Builder.

