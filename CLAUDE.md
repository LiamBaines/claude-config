# Global preferences

## Workflow
- Start non-trivial work in plan mode. Don't implement until I approve the plan.
- Ask clarifying questions before complex work; state assumptions explicitly.
- Write plans to `docs/specs/<feature>.md`, with a numbered task list. Keep them short.
- Do ONE task at a time, then stop.
- Don't log progress into CLAUDE.md. Update the spec's task checkboxes instead.

## Cost discipline
- Work in the main agent by default. Use subagents only for broad searches whose result can be summarised, and only when I ask or when it clearly saves context.
- Don't spawn review or verification subagents unless I ask.
- Use `@file` references or direct paths; avoid broad searching.
- Keep tool output small: filter noisy commands (failures only, tail of logs).
- No extended thinking unless I ask.

## Quality
- Never fabricate tool results; report actual errors.
- Verify with the narrowest relevant test while iterating. Run the full suite once at the end of a task.
- If it can't be tested, say so rather than calling it complete.
- No unrequested features, and no backwards-compat code unless asked.
- Browser testing: Playwright by default.

## Git
- Feature branches for non-trivial work; single-line imperative commit messages, no emojis.
- Commit logical chunks. Squash-merge and delete the branch after merging.

## Style
- Be direct. Skip preamble and recaps. Report blockers immediately.