# Orient

Summarize everything so far so the human can step back into the work and correct the picture. Used when resuming, when asked, and as a step in bootstrap.

## Gather

- Read the project's `AGENTS.md` working approach, `pp/main.md`, and the active artefacts in `pp/`. Read machine logs, such as a sprint's `_log.md`, only for work already in progress.
- Then read what the artefacts do not yet hold: the project's own docs, code, results, and recent git history.

## Summarize

Give the human a summary of the project so far:

- Commitment: what we are building and what would count as success.
- Established: what we know, with the evidence behind it.
- Current phase(s), open questions, and prerequisites.
- Decisions made, and decisions pending.
- Proposed next move, and why.

Mark what comes from the artefacts versus what you inferred from the repository.

## Propose corrections

- Point out where artefacts are stale, wrong, or missing what the repository shows, and propose the specific updates.
- Docs outside `pp/` that duplicate an artefact's role, such as a separate project description, belong in that artefact: propose folding their content in and retiring the original.
- Let the human amend the summary and the proposals. Then record the agreed corrections in the artefacts that own them, so the next orientation starts from a correct picture. Do not change artefacts or retire docs before the human agrees.
