### Stops LLM agents from burning money

Building [veronica-core](https://github.com/amabito/veronica-core) -- runtime cost and execution containment for LLM agent systems.
Your agent retries 3 times per layer. Three layers deep, that's 64 API calls from one user click. veronica-core caps it.

---

## What I build

**[veronica-core](https://github.com/amabito/veronica-core)** -- Runtime containment for LLM agents
- Hard budget, step limits, retry caps, circuit breakers -- evaluated before the call reaches the model
- Semantic loop detection, MCP containment, declarative YAML policies
- AG2 integration merged ([PR #2430](https://github.com/ag2ai/ag2/pull/2430)), LangChain / CrewAI / LangGraph adapters
- 4844 tests, 94% coverage, zero required dependencies
- `pip install veronica-core`

**[HyperRasterizer](https://github.com/amabito/hyper-rasterizer)** -- CUDA 3D Gaussian Splatting rasterizer
- 4169 FPS, MIT license, commercial OK
- Built from scratch on RTX 5090 (sm_120) / CUDA 12.8

**[HyperViewer](https://github.com/nicetomytyuk/hyper-viewer)** -- WebGPU 3DGS viewer

---

## Background

Construction consultant, 15 years. Regulated environments where failure has real cost.
Building CUDA rasterizers and LLM containment tools on the side.

---

## Technical

Python, C++, CUDA, TypeScript, WebGPU

Runtime containment, multi-agent orchestration, GPU kernels, 3D Gaussian Splatting

---

## Writing

- [The $0.64 bug: how nested retries silently multiply your LLM costs](https://dev.to/amabito/the-064-bug-how-nested-retries-silently-multiply-your-llm-costs-3g0p) (dev.to)
- [Zenn articles](https://zenn.dev/amabito) -- CUDA bugs, 3DGS, LLM agent cost control (Japanese)

---

## Open to work

Available for remote contract work -- AI safety, agent infrastructure, runtime systems.

keita.a.0609@gmail.com
