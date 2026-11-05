# MatterWave AI

**Wave mechanics and geometry for machine intelligence.**

Nature doesn't compute with brute-force matrices &mdash; it computes with phase, rotation, and conservation laws. Our **Geometric Rotation Transformer (GRT)** represents language as phase and amplitude, transformed through butterfly cascades of Clifford-coupled Givens rotations rather than dense weight grids.

- **[matterwave.ai](https://matterwave.ai)** &mdash; Research, architecture notes & benchmarks
- **[GRT Technical Whitepaper (PDF)](https://matterwave.ai/static/GRT_Whitepaper.pdf)** &mdash; Full 25-page mathematical specification & CUDA kernel architecture
- **[GRT Interactive Research Note](https://matterwave.ai/grt)** &mdash; Visual walkthrough of polar pairs, butterfly cascades & parameter math
- **[GRT-30M](https://matterwave.ai/grt-30m)** & **[GRT-30M-Embedding](https://matterwave.ai/grt-30m-embedding)** &mdash; Open-weight checkpoints & circular phase pooling benchmarks
- **[Hugging Face (`MatterWaveAI`)](https://huggingface.co/MatterWaveAI)** &mdash; Open model weights (`grt-30m`, `grt-30m-embedding`, GGUF & Safetensors)
- **[app.matterwave.ai](https://app.matterwave.ai)** & **[docs.matterwave.ai](https://docs.matterwave.ai)** &mdash; Hosted platform, API docs & client downloads

---

## Geometric Rotation Transformer (GRT) Ecosystem Integrations

| Repository | Upstream PR | Description |
|---|---|---|
| **[transformers](https://github.com/MatterWaveAI/transformers)** | [`huggingface/transformers#45937`](https://github.com/huggingface/transformers/pull/45937) | Native `GRTConfig`, `GRTModel`, `GRTForCausalLM`, `GRTForSequenceClassification`, and `AutoModel` registration |
| **[vllm](https://github.com/MatterWaveAI/vllm)** | [`vllm-project/vllm#39698`](https://github.com/vllm-project/vllm/pull/39698) | High-throughput GRT serving with PagedAttention, CUDA graphs, and tensor parallelism |
| **[llama.cpp](https://github.com/MatterWaveAI/llama.cpp)** | [`ggml-org/llama.cpp#22060`](https://github.com/ggml-org/llama.cpp/pull/22060) | Native C++/GGML graph execution (CPU, CUDA, HIP, Vulkan) and GGUF conversion for GRT |
| **[sentence-transformers](https://github.com/MatterWaveAI/sentence-transformers)** | [`huggingface/sentence-transformers#3797`](https://github.com/huggingface/sentence-transformers/pull/3797) | Circular phase pooling, semantic search embeddings, and reranker support on the rotational manifold |
| **[kernels-community](https://github.com/MatterWaveAI/kernels-community)** | &mdash; | Fused CUDA/HIP butterfly Givens rotation and Clifford-coupling kernels (`grt-kernels`) |

---

## Developer Platform, SDKs & Open-Source Tools

| Repository | Description |
|---|---|
| **[ia_modules](https://github.com/MatterWaveAI/ia_modules)** | Composable agent & workflow engine for AI applications (published on PyPI) |
| **[nexusql](https://github.com/MatterWaveAI/nexusql)** | Unified database abstraction layer across SQL backends (published on PyPI) |
| **[synthdoc](https://github.com/MatterWaveAI/synthdoc)** | Synthetic legal, medical, and financial document generator with pixel-exact NER ground truth |
| **[python-sdk](https://github.com/MatterWaveAI/python-sdk)** | Official Python SDK for the MatterWave OpenAI-compatible API |
| **[typescript-sdk](https://github.com/MatterWaveAI/typescript-sdk)** | Official TypeScript/JavaScript SDK for the MatterWave API |
| **[tui](https://github.com/MatterWaveAI/tui)** | Terminal UI client for MatterWave conversations and agent workflows |
| **[vscode-extension](https://github.com/MatterWaveAI/vscode-extension)** | VS Code extension for inline chat, code analysis, and agent execution |
| **[desktop](https://github.com/MatterWaveAI/desktop)** | Cross-platform desktop application for Windows, macOS, and Linux |
| **[pi-package](https://github.com/MatterWaveAI/pi-package)** | Official MatterWave provider, GRT model router, and skills for the Pi coding agent |
