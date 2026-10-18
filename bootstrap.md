# Planning bootstrap

Set up or refresh project planning with the human. Preserve existing plans, findings, decisions, and unrelated project instructions.

## Shared setup

- Reuse the cookbook clone at `.ml-cookbooks/`. If something else exists at that path, ask the human rather than overwriting it. Ensure `/.ml-cookbooks/` is gitignored without replacing existing entries. Do not automatically pull or reset the clone; discuss refreshing it when needed.
- Use `templates/AGENTS.md` as the starter for the project's root `AGENTS.md`. Merge its planning section if that file already exists; do not copy the cookbook's own root `AGENTS.md`.
- Create `pp/` and `pp/done/` if missing. `pp` stands for project planning.
- Import `templates/artefacts/main.md` as `pp/main.md` only if that project file is missing. All mechanisms start unselected.

## Enable mechanisms

- Discuss what the project needs using `pp/main.md`.
- For each agreed mechanism, follow its `bootstrap.md` in `templates/<mechanism>/`. Its `agents_template.md` is copied into the project's `AGENTS.md` in the next step.
- Import only the artefacts directed by that mechanism's bootstrap. Keep setup and agent-template files in the cookbook clone.
- Mark the mechanism enabled once its setup is in place, and add links to the project artefacts. If a mechanism is not available yet, explain that rather than marking it enabled.
- In imported artefacts, replace `<ml-cookbooks-root>` with the relative path from that file to the cookbook clone: `../.ml-cookbooks` for files directly under `pp/`, `../../.ml-cookbooks` under `pp/done/`.

## Formulate the working approach

- Sources: each enabled mechanism's `.ml-cookbooks/templates/<mechanism>/agents_template.md`. Use `pp/main.md` to identify the enabled set.
- In the project's `AGENTS.md`, replace everything between `<!-- pp:mechanisms:start -->` and `<!-- pp:mechanisms:end -->` with one `##### <mechanism>` subsection per enabled mechanism, in `pp/main.md` order, each containing that mechanism's `agents_template.md`.
- Copy the instruction text as is: omit each template's top-level title (the destination heading replaces it), and replace path placeholders such as `<project-plan>` with the actual project paths as the mechanism's bootstrap defines; do not merge, summarize, or paraphrase. Keep the markers. Do not edit inside them otherwise; if project-specific notes or conflicts are found inside, discuss them with the human first.
- Outside the markers, change only `Project context`: propose one or two sentences from the existing project, for the human to amend.
- On refresh, compare the project's `## Planning` section with `templates/AGENTS.md`. Discuss differences in the shared text with the human rather than overwriting it.
- Read and apply the updated instructions in the current session. Request a session reload only if the current agent tool requires one to load the changes.

## Orient

Follow `orient.md`. For a project with existing work, propose filled content for the new artefacts from that work, and propose folding in docs that duplicate an artefact's role. The human amends; record what is agreed.

## Revisit

On repeat runs, preserve selections and filled artefacts. Add missing structure, refresh the working approach for the selected mechanisms, and discuss changes or conflicts instead of resetting existing content.

Bootstrap proposes; the human decides.
