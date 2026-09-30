# bookchaowalit-sentiment-analyzer-mobile

Planned mobile version of **Tone Lab**, the transparent sentiment bench whose
web version lives in
[`bookchaowalit-ai/bookchaowalit-sentiment-analyzer-frontend`](https://github.com/bookchaowalit-ai/bookchaowalit-sentiment-analyzer-frontend).

## Status

**Empty / planning.** This repository has no app code yet.

## Intended scope

- Type or paste text and see a positive / negative / neutral reading with
  every contributing word and its weight, like the web version.
- Same method as the web version: a small hand-weighted lexicon with
  negation and intensifier handling. It is a heuristic, not a trained model,
  and the app should say so.
- Runs entirely on the device: text is never sent to a server, and there is
  no account or analytics.

## Related repositories

| Repository | Role |
|---|---|
| `bookchaowalit-sentiment-analyzer-frontend` | Web version; source of the scoring logic (`lib/sentiment.ts`) and its tests |

## Next step

See [`docs/UPGRADE-PLAN.md`](docs/UPGRADE-PLAN.md).
