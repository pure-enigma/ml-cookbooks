# Project: <name>

Instructions (copied into `AGENTS.md`): <ml-cookbooks-root>/templates/crisp_dm/agents_template.md

Fill through conversation and practical work, starting with the commitment and current focus. Reuse existing understanding; do not complete every phase upfront. Leave unknowns explicit and distinguish assumptions from evidence-backed findings. Link detailed artefacts rather than duplicating them.

## Commitment

- Problem and intended value: <What problem are we solving, for whom, and why does it matter?>
- Success criteria: <What result would make this work worthwhile? How will we judge it?>
- Scope and constraints: <What is in scope, what is out, and what constraints apply?>

## Current focus and progression

- Current phase(s): <Which phase or phases need attention now?>
- Established understanding: <What do we know, and what evidence supports it?>
- Open questions and prerequisites: <What is unresolved or would make downstream work premature?>
- Next useful move: <What should we resolve or do next, and why?>
- Readiness to progress: <What would justify moving to another phase? Record the agreed next phase or reason to revisit an earlier one.>

Phases can overlap. Completed activities do not, by themselves, resolve a phase's questions. Exploratory work can proceed provisionally when its assumptions and limits are understood with the human.

## 1. Business / problem understanding

Establish the problem, intended user, value, scope, constraints, and success criteria in the commitment above. For research, this may be a research question rather than a business case. Separate technical metrics from the outcome they serve: a better benchmark score is not automatically a more useful model.

<What have we established about the problem? What remains uncertain about the intended outcome or our commitments?>

**Before progressing:** Do we know what result would make this work worthwhile—and what we are not committing to?

## 2. Data understanding

Inspect examples, labels, distributions, missing values, and likely sources of bias or contamination. Record provenance, usage restrictions, and coverage gaps. Distinguish inspected facts from expectations.

<What data is available and permitted? What have we inspected, what did we find, and what limitations or open questions matter? Link data assessments and supporting evidence.>

**Before progressing:** Is the data suitable for the question, and which limitations could mislead later work?

## 3. Data preparation

Define how raw data becomes inputs, targets, and evaluation splits. Make transformations reproducible. Check that labels and boundaries survive preprocessing and that related records or held-out information do not leak across splits.

<How are inputs, targets, and splits produced? What preparation and leakage checks have we completed, and what remains? Link preparation code and data versions.>

**Before progressing:** Can we reproduce the prepared data and trust the separation between learning and evaluation?

## 4. Modeling

Choose approaches under the agreed constraints. Establish a useful baseline before attributing value to added complexity. State what a candidate should improve and why; use small tests to resolve important uncertainties before expensive training or broad implementation.

<What baseline and candidates are we testing? What uncertainty does each test resolve, and what have we learned? Link architecture and iteration records if enabled.>

**Before progressing:** What are we comparing against, and is the candidate ready for the intended evaluation?

## 5. Evaluation

Judge results against the agreed success criteria. Check that comparisons use compatible data, metrics, and measurement conditions. Examine errors, relevant slices, robustness, and practical costs where they matter. Separate exploration from held-out conclusions; do not tune repeatedly against the final test set.

<What does the evidence show against our criteria? What are the errors, limitations, and remaining uncertainties? Should we proceed, revise, or stop? Link results and evaluation records.>

**Before progressing:** What does the evidence justify—and what does it not justify?

## 6. Deployment / delivery

Define how the result will be used or handed over: a system, model release, or reproducible research finding. Include reproduction instructions and known limitations. Consider integration, monitoring, ownership, and maintenance only where ongoing operation is needed.

<What are the deliverables, who will use them, and how? What is needed for reproduction or ongoing use? Link the deliverables and supporting instructions.>

**Before closing:** Can the intended recipient use or reproduce the result, with its limitations understood?

## Decisions and open questions

<What consequential decisions have we made, and what questions remain? Include rationale and links to evidence or detailed records.>

Update this same plan as understanding evolves. Discuss changes to scope, commitments, or success criteria with the human. If sprints are enabled, let this plan shape their commitments and revisit it when their findings change our understanding.

## Closure

<How did the outcome compare with our commitment? What remains unresolved, where are the deliverables, and has closure been agreed with the human?>

Once closure is agreed, move this plan to `pp/done/` without renumbering and update references, including relative cookbook links.
