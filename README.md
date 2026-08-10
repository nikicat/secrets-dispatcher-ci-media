# secrets-dispatcher-ci-media

Throwaway CI media for [secrets-dispatcher](https://github.com/nikicat/secrets-dispatcher):
screen-recorded demo videos published by its **Demos** workflow.

- `pr-<N>/` — recordings from pull request #N (overwritten on each run).
- `main/`   — recordings from the latest master push.

Served over GitHub Pages so a PR's demo comment can embed the players inline.

## Maintenance

This repo grows unboundedly — one `pr-*/` dir per pull request, never pruned —
and git history keeps every superseded video blob. Neither is a source of
truth; it is safe to prune old `pr-*/` dirs and to `git gc` / squash the
history at will. A periodic cleanup is a TODO in secrets-dispatcher.
