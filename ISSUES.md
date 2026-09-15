# Public Issues Tracking Log

Tracking technical feedback, runtime issue audits, and RFC contributions across public repositories.

| Repository / Link | Topic / Context | Audit & Technical Intervention | Status |
| :--- | :--- | :--- | :--- |
| [`vllm-project/vllm` #37003](https://github.com/vllm-project/vllm/issues/37003) | Context-Aware KV-Cache Retention API (RFC) | Addressed state-coupling bottlenecks in 200k agent sessions; proposed stateless orchestration via explicit state partitioning (DriftBreak) & line-based serialization (SLAP) | Open (Active maintainer exchange / Evaluated `👀`) |
| [`vllm-project/vllm` #55313](https://github.com/vllm-project/vllm/issues/55313) | XGrammar FSM desync emitting 250k whitespace loop under speculative decoding | Analyzed token-level grammar failure mode / whitespace sinks; proposed deterministic line-protocol alternative to mitigate FSM deadlocks | Open (Referenced in #53777) |
| [`vllm-project/vllm` #54919](https://github.com/vllm-project/vllm/issues/54919) | Long-prefill decode starvation on hybrid GDN (Qwen3.8-27B) | Traced mixed-phase starvation to unconstrained ingress & attention metadata overhead; community profile isolated root cause to blocking D2H sync (`backend.py:482`) | Open (Root cause profiled & reproduction verified) |
