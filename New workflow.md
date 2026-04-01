# workflow.md — Lean Build Workflow

## Session Start
Always start with:
1. Load `CLAUDE.md`
2. State the current task in one sentence

Do not auto-load every command file.

## Task Types

### Bug Fix
1. Identify exact bug
2. Load `fix.md` only if needed
3. Edit the minimum files necessary
4. Run type-check or relevant test
5. Stop

### Small Feature
1. Define exact feature scope
2. Load `feature-dev.md` only if needed
3. Build only that feature
4. Run type-check or relevant test
5. Stop

### Research Task
1. Load `research.md` only if external APIs/data are involved
2. Summarize findings
3. Stop
4. Do not start building unless asked

### Review Task
1. Load `review.md` only if a review is explicitly requested
2. Report findings
3. Stop

### Ship Task
1. Load `ship.md` only when preparing deployment
2. Run deployment checklist
3. Stop before live deploy unless explicitly requested

## Global Rules
- Never chain commands automatically
- Never load more than one task file unless necessary
- Never do build + review + ship in one pass unless explicitly requested
- Stop after the requested task is complete