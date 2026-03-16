### Governed knowledge execution for LLM agents

Building the stack: [TriMemory](https://github.com/amabito/tri-memory) resolves what the agent knows, [veronica-core](https://github.com/amabito/veronica-core) enforces that the inference stays within budget.

---

## What I build

**[TriMemory](https://github.com/amabito/tri-memory)** -- Memory architecture for LLM agents
- Three-path memory: KV window + retrieval index + TRN recurrent state
- 8 KB per agent at any context length (vs 156 MB KV cache at 10K tokens)
- 1,000 concurrent agent states in 16 MB
- 277 tests, Apache 2.0

**[VERONICA Core](https://github.com/amabito/veronica-core)** v3.7.6 -- Runtime containment for LLM agents
- Hard budget, step limits, retry caps, circuit breakers -- evaluated before the call reaches the model
- Memory governance, message hooks, DEGRADE directives, semantic loop detection
- Contributor to [AG2 v0.11.3](https://github.com/ag2ai/ag2/releases/tag/v0.11.3) ([PR #2430](https://github.com/ag2ai/ag2/pull/2430)), LangChain / CrewAI / LangGraph / LlamaIndex adapters
- 6125 tests, 94% coverage, zero required dependencies
- `pip install veronica-core`

**[VERONICA](https://github.com/amabito/veronica)** v0.8.1 -- LLM governance control plane
- Policy authoring, simulation, rollout pipelines
- Tenant hierarchy, incident replay, audit dashboards
- Built on veronica-core
- 1197 tests
- `pip install veronica-cp`

---

## Background

Construction consultant, 15 years. Regulated environments where failure has real cost.
Now applying that mindset to LLM agent safety.

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
