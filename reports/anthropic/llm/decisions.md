# Decisions — anthropic/llm

- Default claude-sonnet-4-6 is superseded by claude-sonnet-5 — skip; aiewf-eval's `aiwf_medium_context` scores `claude-sonnet-5` at 93% pass / 1204 ms TTFAT P50 with thinking disabled against 100% / 850 ms for `claude-sonnet-4-6`, so 4.6 stays the default and the next Sonnet gets evaluated when it ships ([comment](https://github.com/pipecat-ai/provider-watch-reports/issues/1#issuecomment-5427783747), 2026-08-26)
