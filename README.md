# Tharun Jagarlamudi

**Systems & Performance Engineer** · GPU Programming · Distributed Training · LLM Infrastructure

Building high-performance systems for large-scale machine learning.

---

## Featured Work

### GPU Kernel Development
**[triton-kernels](https://github.com/rtj1/triton-kernels)** — Production-grade Triton GPU kernels
- FlashAttention with online softmax algorithm (O(N) memory vs O(N²))
- Optimized MatMul with 15 autotune configs targeting T4/V100/A100/H100
- LayerNorm, Softmax with fused operations
- Achieves 60-90% of cuBLAS performance

### Memory Systems
**[cuda-mempool](https://github.com/rtj1/cuda-mempool)** — High-performance CUDA memory allocator
- Size-class binning with configurable thresholds
- Stream-ordered allocation for async kernels
- Thread-safe with fine-grained locking
- Defragmentation and memory statistics

**[arena-alloc](https://github.com/rtj1/arena-alloc)** — C++17 arena, slab, and pool allocators
- Zero-overhead abstraction for hot paths
- RAII-compliant with custom deleters

### Distributed Training
**[ddp-lora-trainer](https://github.com/rtj1/ddp-lora-trainer-)** — Multi-GPU LoRA fine-tuning
- PyTorch DDP with gradient checkpointing
- Mixed precision (FP16/BF16) with loss scaling
- GPT-2 Conv1D layer support for LoRA injection

### LLM Safety & Security
**[aria](https://github.com/rtj1/aria)** — Automated Red-teaming & Iterative Attack Agent
- 10 attack strategy families, 77 variants
- Reflexion-based learning from failed attacks
- Campaign results: 12% ASR on Claude 3.5 Sonnet across 1,078 attacks
- ChromaDB-powered attack memory with similarity search

**[vibeclean-ai](https://github.com/rtj1/vibeclean-ai)** — Static analysis for AI-generated code
- AST-based detection (Babel, tree-sitter, java-parser)
- OWASP Top 10 vulnerability detection
- Prompt injection pattern matching

### Low-Level Systems
**[lockfree-queue](https://github.com/rtj1/lockfree-queue)** — Lock-free SPSC/MPMC queues in Rust
- Cache-line padding to prevent false sharing
- Memory ordering with acquire/release semantics

**[tensor-serde](https://github.com/rtj1/tensor-serde)** — Fast binary serialization for ML checkpoints
- Zero-copy deserialization where possible
- Streaming support for large models

---

## Technical Focus

```
GPU Programming     Triton, CUDA, cuBLAS, TensorRT
Distributed Systems PyTorch DDP, NCCL, gradient checkpointing
Memory Management   Custom allocators, memory pools, arena allocation
Performance         Profiling, kernel optimization, memory bandwidth analysis
Languages           Python, C++, Rust, CUDA
```

---

## Links

[LinkedIn](https://linkedin.com/in/tharun-jagarlamudi-664a9331b)
