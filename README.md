# ML Cookbooks ( AGENTS.md factory )

## How to use

From your project's root:

1. Clone the cookbook:
   ```sh
   git clone git@github.com:pure-enigma/ml-cookbooks.git .ml-cookbooks
   ```
2. Copy `.ml-cookbooks/templates/AGENTS.md` to your project's root `AGENTS.md`. If one already exists, merge the planning section instead of overwriting it.
3. Ask your agent:
   > Follow `.ml-cookbooks/bootstrap.md` to set up planning for this project with me.

Bootstrap ensures `.ml-cookbooks/` is gitignored, helps you select mechanisms, and sets up `pp/` while preserving existing work. Use the same request later to refresh the setup.

## Purpose

Importable Markdown artefacts that help a human and an agent stay immersed in project work.

Key reasons for failing to be in an immersed (flow-state):
- Absence of orientation of where I'm in the overall project trajectory.
- Agents trying to jump over and build simultaneously multiple phases of project trajectory.
- Agents working beyond what I'm looking forward to accomplish in my mind. ( E.g., I might be thinknig of data understanding and not yet solving -- often these are subconscious elements and tedious and impossible to state explicitly at each turn )

This repository is an attempt to establish structure about ways of working via project planning "artefacts".

Core idea: Import an artefact, fill it through conversation, that keeps agent and human oriented well. The structure helps us clarify what we committed to, do the necessary diligence, and avoid starting work too early—not add paperwork.

## How it works

**`pp` stands for project planning.** It is the project's home for planning artefacts: what we committed to, where we are, and what comes next.

- `pp/main.md` starts as a human-facing checklist, all mechanisms unselected. Together, we select what the project should enable.
- Checked means enabled, not completed. Each enabled mechanism links to its project artefacts; progress lives there.
- The shared working approach is part of `templates/AGENTS.md`. Bootstrap copies each enabled mechanism's `agents_template.md` into its own marked section of the project's `AGENTS.md`, preserving the instructions rather than merging or summarizing them.
- Only fillable files from `artefacts/` are imported into `pp/`. Agent templates and setup instructions remain in the cookbook clone.
- `orient.md` answers **Where are we? What should we work on next?** It summarizes everything so far from the artefacts and the repository, and the human corrects it. Bootstrap runs it to propose the first filled artefacts; agents run it when resuming.

Each mechanism separates setup (`bootstrap.md`), ongoing agent instructions (`agents_template.md`), and fillable project content (`artefacts/`). Bootstrap explains how to use them; agent templates contain the working instructions themselves, not installation explanations.

## Mechanisms

| Mechanism | What it helps us do | Availability |
|---|---|---|
| `crisp_dm` | Frame the project and progress through understanding, preparation, modeling, evaluation, and delivery. | Available |
| `sprints` | Commit to a manageable next body of work, review it, and decide what follows. | Planned |
| `model_iteration` | Test a change and capture what we learned. | Planned |
| `modular_dl_models` | Build models from clear blocks and maintain human-readable architecture documentation with visual aids where useful. | Available |

These are working views, not a rigid pipeline. A project plan can guide sprints; model findings can change either plan. Each mechanism's bootstrap and agent template explain how it is set up and used.

## Design principle

The structure carries context and brings the right questions into the work at the right time. The human's attention stays on exploring, deciding, and building—not administering the framework.

If a prompt or file does not help us think, act, or resume, simplify it or remove it.
