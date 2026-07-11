## Systems engineer working at the intersection of **AI inference infrastructure** and **safety-critical embedded systems**.

Currently a pre-final year EE undergrad at MIT Manipal - published in **Springer Nature Q1** (2026), **IEEE VTC** (2026), and 3 provisional patents through MAHE/DGIP.

Building **multilingual voice AI** @ [Fettle](https://letsfettle.com) · **solar racing EV firmware** @ [SolarMobil](https://solarmobilmanipal.org) · **agentic B2B SaaS** @ [Guaq AI](https://guaqai.me)

---

## Open Source Contributions

> All PRs below are currently in review - code-owner responses pending.

| Repo | PR | What it does |
|---|---|---|
| [**vllm-project/vllm**](https://github.com/vllm-project/vllm/pull/44794) | [#44794](https://github.com/vllm-project/vllm/pull/44794) | **FlowPrefill**: checkpoint-based sub-chunk preemption for the v1 scheduler — CUDA event polling detects decode pressure and suspends prefill mid-chunk without `synchronize()`, using a pre-allocated event pool to eliminate per-step overhead |
| [**sgl-project/sglang**](https://github.com/sgl-project/sglang/pull/30852) | [#30852](https://github.com/sgl-project/sglang/pull/30852) | DSpark speculative decoding (SGLang): root-caused a checkpoint-format compatibility bug causing ~3.6x accept-length degradation (1.1→3.97 tokens/step) on speculators-format checkpoints in an actively-developed spec-decode feature backed by an official lmsys.org release. |
| [**microsoft/vidur**](https://github.com/microsoft/vidur/pull/80) | [#80](https://github.com/microsoft/vidur/pull/80) | **MoE + disaggregated scheduler**: DeepSeek-V3 and Mixtral-8x7B MoE configs with `BaseMoEModelConfig`, plus a disaggregated prefill/decode scheduler for Microsoft Research's LLM inference simulator |
| [**anthropics/anthropic-sdk-python**](https://github.com/anthropics/anthropic-sdk-python/pull/1663) | [#1663](https://github.com/anthropics/anthropic-sdk-python/pull/1663) | **Streaming perf**: skip `build_events()` and use O(1) buffers on the `get_final_message` drain path — eliminates unnecessary `TextEvent`/`InputJsonEvent` construction when caller doesn't iterate events, fixing [#1649](https://github.com/anthropics/anthropic-sdk-python/issues/1649) |
| [**jpmorganchase/QOKit**](https://github.com/jpmorganchase/QOKit/pull/139) | [#139](https://github.com/jpmorganchase/QOKit/pull/139) | **Lazy Ising kernel**: on-the-fly Ising energy computation inside the CUDA phase-separation kernel, eliminating the O(2ⁿ) precomputed diagonal array and its CPU→GPU transfer, fixing [#35](https://github.com/jpmorganchase/QOKit/issues/35) |
| [**finos/pylegend**](https://github.com/finos/pylegend/pull/311) | [#311](https://github.com/finos/pylegend/pull/311) | **Type system**: adds `Time`, `Variant`, and `Binary` primitive types through the full type chain (enum → class hierarchy → expression layer) in FINOS/JPMorgan's Python Legend query library, closing [#220](https://github.com/finos/pylegend/issues/220) |

---

## Research & IP

| | |
|---|---|
| 📄 | **Springer Nature Q1** — [Technical Validation of a Multimodal Emotion-Adaptive Biofeedback System for Autonomic Regulation](https://doi.org/10.1038/s41598-026-46105-9) · *Scientific Reports, Apr 2026* |
| 📄 | **IEEE VTC 2026** — [Physics-Informed Stochastic Receding Horizon Control for Autonomous Energy Management in Solar Racing](https://bit.ly/vtc2026-solarev) · *Accepted Apr 2026* |
| 🔒 | **3 provisional patents** via MAHE/DGIP — adaptive EV interface (202541050036), long-range EV telemetry (202541064383), robotic solar panel cleaning (202541079610) |

---

## Stack

```
AI/Inference    vLLM · SGLang · PyTorch · TorchRec · LangGraph · LangChain · Gemini ADK
Voice/RT        LiveKit · SIP/PSTN · WebSockets · Whisper · multilingual STT/TTS
Backend         FastAPI · Django · Spring Boot · Redis · Kafka · PostgreSQL · ClickHouse
Platform        Lago · Clerk · PostHog · Cloudflare Zero Trust · Prometheus · Grafana
Embedded        STM32H7 · FreeRTOS · TouchGFX · CAN · MISRA C/C++ · Verilog · TensorRT
Cloud           AWS (ECS, Fargate, Lambda) · GCP (Cloud Run, Vertex AI) · Kubernetes
```

---

## Current Areas

- **AI inference serving** — speculative decoding, scheduler preemption, MoE simulation
- **Voice AI infrastructure** — multilingual hospital workflow agents, SIP orchestration, inference pooling  
- **Safety-critical firmware** — Cortex-M7 ECU, FreeRTOS, CAN bus, race strategy digital twin
- **Agentic platform primitives** — multi-tenant auth, metering, tool integration, observability

---

## Contact

📧 [pulkit.talks@gmail.com](mailto:pulkit.talks@gmail.com) · [university](mailto:pulkit.kumar@learner.manipal.edu)  
🌐 [buddywhitman.vercel.app](https://buddywhitman.vercel.app) · [LinkedIn](https://linkedin.com/in/buddywhitman) · [ORC**i**D](https://orcid.org/0000-0003-4078-1780)  
💬 Discord: `buddywhitman`
