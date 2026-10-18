# sprints bootstrap

Enable sprints: short commitments with a groomed hypothesis, checkbox tasks, and a closing review that proposes the next sprint.

- `agents_template.md` alongside this file is this mechanism's contribution to the project's `AGENTS.md`; the overall bootstrap copies it there. It has no path placeholders.
- Agree the first sprint's focus with the human before creating it. If a project plan exists, propose the focus from its next useful move and open questions.
- Import `artefacts/sprint.md` as `pp/sprint_001_<name>.md`, choosing the next sprint number across `pp/` and `pp/done/`. Keep one active sprint at a time unless the human asks otherwise.
- Replace `<ml-cookbooks-root>` in the imported artefact with the relative path to the cookbook clone: `../.ml-cookbooks` for a file directly under `pp/`.
- Propose the goal, `Serves`, grooming, tasks, and out-of-scope list from the agreed focus and existing work. Keep unknowns explicit; the human amends the proposal before implementation starts.
- Link the active sprint under `sprints` in `pp/main.md`. The overall planning bootstrap marks it enabled and copies `agents_template.md` into the working approach.

On repeat runs, preserve existing sprints. Create the next sprint only after the active one's closing review is agreed; update the `pp/main.md` link to the new active sprint.
