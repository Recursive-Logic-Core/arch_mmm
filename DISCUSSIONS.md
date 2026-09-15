# Public Discussions & Q&A Log

Tracking technical interventions, architectural input, and accepted resolutions across public community discussions.

| Repository / Link | Topic / Context | Audit & Technical Intervention | Status |
| :--- | :--- | :--- | :--- |
| [`ggml-org/llama.cpp` #28588](https://github.com/ggml-org/llama.cpp/discussions/28588) | Qwen 3.8 Flash Next saturating Windows host RAM | Stripped fragmentation vectors, enforced `--no-mmap` host isolation, and pinned batch worker threads | Resolved (Marked as answer) |
| [`ggml-org/llama.cpp` Discussions](https://github.com/ggml-org/llama.cpp/discussions) | Persistent state for recurrent models (SSM/DeltaNet) with `--context-shift` | Unpacked mathematical conflict between path-dependent recurrent states ($h_t$) and spatial sliding-window shifts; defined orchestrator-level compaction and clean-start re-anchoring pattern for proxy architectures | Open (Awaiting author response) |
| [`ggml-org/llama.cpp` #20243](https://github.com/ggml-org/llama.cpp/discussions/20243) | Managing context in Qwen 3.5 from C API | Diagnosed recurrent state leakage ($h_t$ non-invertibility) post-`llama_memory_seq_rm`; defined checkpoint restore vs. clean prefill boundary patterns for hybrid architectures in C API | Open (Awaiting author response) |
