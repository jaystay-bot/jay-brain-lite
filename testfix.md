# TESTFIX MODE (LOW COST)

## Goal
Fix ONE issue and verify it works.

## Rules
- Fix ONLY the reported issue
- Do NOT refactor unrelated code
- Do NOT improve architecture
- Do NOT fix additional issues unless explicitly told
- Run verification ONCE only

## Scope
- Max 2 files changed
- Minimal edits only

## Process
1. Identify root cause of the issue
2. Fix the issue
3. Run ONE verification:
   - `npx tsc --noEmit` if TypeScript
   - or explain how to test locally
4. Stop

## Output
- Root cause
- What was changed
- Verification result

## STOP
Do NOT loop.
Do NOT re-run automatically.
Do NOT continue fixing additional issues.