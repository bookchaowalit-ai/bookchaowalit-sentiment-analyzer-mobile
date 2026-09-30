# Upgrade plan

## Current state

**Score: 1/10.** Initial commit: README, `.gitignore`, this plan. No code,
no CI (there is nothing to check yet).

## Proposed scaffold (decision needed)

Recommended stack: **Expo (React Native) + TypeScript**, so the web
version's scorer (`lib/sentiment.ts`) and its tests can be reused as-is.

```
app/index.tsx          # input, Analyze button, result with word weights
src/sentiment.ts       # scorer shared with the web version
tests/sentiment.test.ts  # same cases as the web repo
.github/workflows/ci.yml # npm ci, lint, typecheck, test, expo export
```

## Backlog

### P0
- Confirm the stack and how the scorer is shared (copy with a parity test,
  or a small package).
- Scaffold, port the scorer with its tests, add CI.

### P1
- Accessibility: announce the result to screen readers, do not rely on
  colour alone for positive/negative, support large text.
- Thai-language lexicon as a separate, clearly labelled mode (the web
  lexicon is English).

### P2
- Share-sheet input (analyse text shared from other apps), still on-device.

## Done in this pass (2026-09-30)
- Initial commit with an honest README (planning only), `.gitignore`, and
  this plan.
