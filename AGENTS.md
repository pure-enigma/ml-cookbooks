# Working on ML Cookbooks

This repository contains reusable planning templates and setup instructions, not a consuming project's filled plans.

- Follow the human's current focus. Develop the structure through brief discussion and practical learning; do not jump ahead into unnecessary mechanisms.
- Read `README.md` for the intent and usage, then the relevant files before editing them.
- `templates/AGENTS.md` is the starter copied or merged into another project's root `AGENTS.md`. It is not this repository's setup instruction: do not clone this repository inside itself.
- Reusable material lives in `templates/`; consuming projects keep their actual planning artefacts in `pp/` and their gitignored cookbook clone in `.ml-cookbooks/`.
- Separate each mechanism's setup (`bootstrap.md`), ongoing agent instructions (`agents_template.md`), and fillable content (`artefacts/`). Keep installation and composition explanations in bootstrap, not in agent templates. The shared bootstrap and orientation (`bootstrap.md`, `orient.md`) live at the repository root; shared agent instructions live in `templates/AGENTS.md`.
- Reference cookbook files from artefacts with the `<ml-cookbooks-root>/...` placeholder; bootstrap replaces it with the consuming project's relative path to `.ml-cookbooks/`.
- Use snake_case filenames, except standard names such as `AGENTS.md` and `README.md`. Mark fillable content with `<what belongs here>` placeholders; keep guidance as ordinary prose.
- Preserve the human's README notes and transcript material. Keep documentation and references aligned when changing the structure.
