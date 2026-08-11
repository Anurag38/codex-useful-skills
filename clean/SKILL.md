---
name: clean
description: Polish an existing code diff with KISS, DRY, and the repository's local style. Use for `/clean`, "clean this up," "tidy this," or before handing off a pull request. Inspect and improve the code; do not treat cleanup as permission to run a full test, typecheck, or lint suite.
---

# Clean Code

Polish the code until it is concise, efficient, readable, and consistent with its repository. Prefer the smallest sharp solution over ceremony.

## Scope

Use this skill for a focused cleanup pass. It is not a feature workflow, test workflow, or broad refactor. Preserve behavior unless the user explicitly requests a behavior change.

Before a pull-request handoff, run this pass automatically after the requested work is complete.

## Workflow

1. Read the full diff and identify its intended behavior.
2. Read neighboring code before changing style, names, imports, or file layout.
3. Remove dead code, debug logging, stale comments, accidental files, and duplication introduced by the diff.
4. Extend an existing helper when it already owns the behavior. Do not create a parallel implementation.
5. Simplify control flow and names when the result remains clear.
6. Remove abstractions with one caller unless they express an important domain boundary.
7. Keep unrelated code and existing behavior unchanged.
8. Re-read the final diff and report what was cleaned.

## Rules

- Apply KISS: choose the simplest design that meets the requirement.
- Apply DRY: centralize repeated behavior when the shared abstraction is stable and improves clarity.
- Copy the local code style. Match naming, imports, formatting, error handling, comments, file placement, and abstraction level.
- Prefer concise code, but do not use cleverness that makes the behavior harder to understand.
- Keep comments for decisions, constraints, and non-obvious behavior. Remove comments that only restate the code.
- Remove temporary logging after the problem is resolved. Keep diagnostic logging when the issue is still being investigated.
- Avoid speculative helpers, configuration, dependencies, or abstractions.
- Avoid drive-by refactors. A cleanup should make the requested diff easier to review, not enlarge its scope.

## Validation boundary

“Clean” means polish. Do not run the full test suite, typecheck, formatter, or linter merely because the user asked for cleanup. Run a targeted check only when a cleanup change could alter behavior or when the user requests validation. Report any check that you ran.

## Pull-request handoff

When cleaning before a pull request:

- Review the complete diff, not only the last edit.
- Ensure the title and body describe the resulting change as a whole.
- Remove implementation-process notes from the final description.
- Keep commits topical when the repository workflow supports it.
- Do not include unrelated cleanup in the pull request.

## Output

Return a short summary:

1. What was removed or simplified.
2. Which local conventions were matched.
3. Any behavior-sensitive cleanup that needs a targeted check.

If the diff is already clean, say so and leave it unchanged.

## Attribution

This skill is an original synthesis inspired by the `/clean` skill shared in [brooklyn-skills](https://github.com/OutThisLife/brooklyn-skills/tree/main/skills/clean), licensed under the MIT License. The linked repository remains the source for its own implementation.
