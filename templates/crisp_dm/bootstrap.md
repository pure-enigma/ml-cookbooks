# crisp_dm bootstrap

Enable a long-lived CRISP-DM project plan. Reuse existing project understanding rather than asking the human to repeat it.

- `agents_template.md` alongside this file is this mechanism's contribution to the project's `AGENTS.md`; the overall bootstrap copies it there, replacing `<project-plan>` with the project plan's path, e.g. `pp/project_001_ner.md`.
- If a suitable active project plan already exists in `pp/`, discuss using it rather than creating a duplicate. A project description elsewhere, such as `PROJECT.md`, is not a plan: fold it into the new plan during orientation.
- Otherwise import `artefacts/project.md` as `pp/project_001_<name>.md`, choosing the next project number across `pp/` and `pp/done/`.
- Replace `<ml-cookbooks-root>` in the imported artefact with the relative path to the cookbook clone: `../.ml-cookbooks` for a file directly under `pp/`. The instructions reference then points to `../.ml-cookbooks/templates/crisp_dm/agents_template.md`.
- During orientation, propose content for every section the existing work already informs, starting with `Commitment` (problem and intended value, success criteria) and `Current focus and progression` (current phase, next useful move). Keep unknowns explicit; the human amends the proposal.
- Link the project plan under `crisp_dm` in `pp/main.md`. The overall planning bootstrap marks it enabled and copies `agents_template.md` into the working approach.

On repeat runs, preserve the existing plan and its decisions. Repair missing links or setup without importing a fresh blank over it.
