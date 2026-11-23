# Decisions — aws/realtime

- Handle `InputTextRawFrame` in `AWSNovaSonicLLMService` so typed text drives a reply — closed unmerged; "realtime services weren't handling new messages programmatically appended to the context" is the real gap, and it is fixed by passing `LLMMessagesAppendFrame` on to the realtime service instead ([PR](https://github.com/pipecat-ai/pipecat/pull/4356), 2026-11-12)
