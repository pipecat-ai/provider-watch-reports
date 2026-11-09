# Decisions — speechmatics/stt

- `sample_rate=16000` on an 8 kHz pipeline relabels PCM instead of converting it — resolved by the provider's native 8 kHz support; the guidance is to drop the override rather than resample or guard it ([issue #5717](https://github.com/pipecat-ai/pipecat/issues/5717) closed as completed 2026-11-04: "`SpeechmaticsSTTService` now supports 8 kHz audio alongside 16 kHz, so an 8 kHz telephony pipeline works as-is. Drop the `sample_rate=16000` override."; the resampling [PR #5719](https://github.com/pipecat-ai/pipecat/pull/5719) closed unmerged the same day)
