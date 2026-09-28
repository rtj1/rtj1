# Tharun Jagarlamudi

**AI Engineer** · LLM Agents · Voice AI · Testing & Evaluation

I build LLM agents and voice AI products, and I measure them before I trust them. Right now I'm building **Katha**, an iOS reader that gives every character in a book its own AI voice. Before that I launched **[indes.ai](https://indes.ai)**, a multi-LLM platform with agentic routing.

---

## Current work

**Katha: Multi-Voice AI Reader for iOS** · *in development*
- **Agentic voice casting:** Claude profiles each character from the book and writes a voice prompt; Qwen3-TTS renders candidates until one passes a pitch check, then it becomes that character's voice
- **Speaker attribution** (NER, alias resolution, Claude as LLM fallback), measured on a 380-quote annotated benchmark: explicit-quote accuracy 0.68 → 0.82 at 95% precision
- **4 TTS engines** routed by language: Kokoro on-device (MLX), self-hosted Qwen3-TTS and Indic Parler-TTS, Apple as fallback, with consent-gated voice cloning
- 1,500+ Swift tests and 150+ Pytest tests in CI · Swift, Python, Claude API, MLX

**[indes.ai](https://indes.ai): Multi-LLM Platform with Agentic Routing**
- Streams GPT, Claude, Gemini and DeepSeek side by side and merges them into one answer (web, iOS/Android)
- **Agentic routing:** 11-type query classifier with LLM fallback, plus a 7-tool orchestrator that answers simple queries without an LLM call
- Fine-tuned a **T5 synthesis model** on Claude outputs, evaluated with BLEU/ROUGE
- 650+ Jest/Supertest tests gating every PR, Playwright E2E across Chromium, Firefox and WebKit · Node.js, React Native, Python

---

## Agents

**[aria](https://github.com/rtj1/aria)**: LLM red-teaming agent
- 10 attack strategies, 77 variants
- Reflexion-based learning from failed attempts

**[reflexive-llm-agent](https://github.com/rtj1/reflexive-llm-agent)**: self-reflective tool-using agent
- ReAct + Reflexion loop with long-term ChromaDB memory
- FastAPI backend and Streamlit UI

---

## Open-source contributions

- **[vllm-project/llm-compressor#2330](https://github.com/vllm-project/llm-compressor/pull/2330)**: GSM8K evaluation script and AWQ + FP8 results (merged)
- **[instructlab/training#682](https://github.com/instructlab/training/pull/682)**: fix HYBRID_SHARD failure when world_size < available GPUs (merged)

---

## ML systems

- **[triton-kernels](https://github.com/rtj1/triton-kernels)**: FlashAttention, MatMul, Softmax and LayerNorm in Triton, autotuned for T4/V100/A100/H100
- **[ddp-lora-trainer](https://github.com/rtj1/ddp-lora-trainer-)**: multi-GPU LoRA fine-tuning with PyTorch DDP and mixed precision
- **[llm-quantization](https://github.com/rtj1/llm-quantization)** · **[llm-sparsity](https://github.com/rtj1/llm-sparsity)**: GPTQ, AWQ, SmoothQuant; magnitude, 2:4 and WANDA pruning
- **[vibeclean-ai](https://github.com/rtj1/vibeclean-ai)**: AST-based security analysis for AI-generated code
- **[cuda-mempool](https://github.com/rtj1/cuda-mempool)** · **[lockfree-queue](https://github.com/rtj1/lockfree-queue)** · **[arena-alloc](https://github.com/rtj1/arena-alloc)**: CUDA, Rust and C++ systems work

---

## Skills

- **Agents & LLMs:** Claude, GPT, Gemini APIs · tool calling · agentic routing · RAG · ReAct · LangChain · MCP
- **Voice AI:** Qwen3-TTS · Indic Parler-TTS · Kokoro · Chatterbox · MLX
- **Testing & Evaluation:** Playwright · Jest · Pytest · Swift Testing · load testing · eval sets · BLEU/ROUGE
- **Languages:** Python · Swift · JavaScript/Node.js · SQL · C++ · Rust
- **Infrastructure:** Google Cloud · AWS · Docker · GitHub Actions · Redis · PostgreSQL · Kafka
