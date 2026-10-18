# modular_dl_models bootstrap

Set up pure-block model development with a living view of the final model.

- `agents_template.md` alongside this file is this mechanism's contribution to the project's `AGENTS.md`; the overall bootstrap copies it there, replacing `<model-arch>` with the architecture record's path, e.g. `pp/model_arch_001_pointer_decoder.md`. If the project has several models, list each record's path.
- Discuss the model's purpose and boundaries with the human. For existing code that is not yet modular, agree with the human whether and when to refactor it into blocks; do not restructure working code unasked.
- For a model needing an architecture record, import `artefacts/model_arch.md` as `pp/model_arch_001_<name>.md`. Choose the next architecture number across `pp/` and `pp/done/`. Reuse an existing record for the same model rather than creating a duplicate.
- Replace `<ml-cookbooks-root>` in the imported artefact with the relative path to the cookbook clone: `../.ml-cookbooks` for a file directly under `pp/`.
- Let the project shape the record from practical learnings. Describe what exists, mark proposed blocks, and leave unknowns explicit.
- Link the architecture record under `modular_dl_models` in `pp/main.md`. The overall planning bootstrap marks it enabled and copies `agents_template.md` into the working approach.

On repeat runs, preserve existing architecture records. Create another only for another model that needs one. When a model is retired, move its record to `pp/done/` without renumbering and update references.
