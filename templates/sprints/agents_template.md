# sprints

The active sprint is the `sprint_<nnn>_<name>.md` file in `pp/` (closed sprints are in `pp/done/`). Work on its tasks; anything outside them goes to its out-of-scope list or the next sprint's proposal. Groom a task before implementing it: what we will build, the analysis it depends on, the hypothesis, how we'll know, and the solution we will try. Ask the human before implementing an ungroomed task.

Tick a subtask only when it is done, and a task only when its done-when checks pass. Keep the summary counts in step with the checkboxes. In the sprint file, add one log line per completed subtask or decision, with today's date and evidence links. Record working detail for resuming agents (commands, outputs, dead ends, in-progress state) in the sprint's machine log, `sprint_<nnn>_<name>_log.md`; read it when resuming a task already in progress. Put work products in the project's own folders, not `pp/`, and link them from the sprint.

When the tasks are done, run the closing review with the human, update the project plan with what we learned, and propose the next sprint's focus.
