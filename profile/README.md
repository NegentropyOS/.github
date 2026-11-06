<a href="https://discord.gg/g8nqB3NtXt"><img align="right" src="https://img.shields.io/badge/NEGENTROPY-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="NEGENTROPY on Discord"></a>
<a href="https://opensource.org/licenses/Apache-2.0"><img align="right" src="https://img.shields.io/badge/Apache_2.0-181717?style=for-the-badge&logoColor=white" alt="Apache 2.0"></a>
<div align="left">English | <a href="./README_ES.md">Español</a></div>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="org-NEGENTROPY.gif">
  <img src="org-NEGENTROPY-light.gif" alt="NEGENTROPY wordmark animating into place" width="960">
</picture>

<p align="center"><strong>Order out of chaos for the age of AI agents.</strong></p>

<p align="center"><em>Deterministic infrastructure and persistent memory for autonomous systems you can trust.</em></p>

---

## What is NegentropyOS?

NegentropyOS builds **verifiable, deterministic infrastructure for AI agents**.

Large language models provide raw probabilistic intelligence, but operational enterprise environments require predictable state, reproducible memory, and strict sovereignty. NegentropyOS provides the architectural layer that turns non-deterministic inference into reliable, auditable execution.

Our engineering thesis is direct: **infrastructure must survive operational reality**. We separate statistical model output from deterministic, ACID-compliant storage and verifiable execution substrates.

---

## Active Substrate: VantaDB

Our core active production substrate is **VantaDB** — an embedded, persistent memory and hybrid vector retrieval engine built in **Rust**.

| Property | Details |
|---|---|
| **Repository** | [`ness-e/Vantadb`](https://github.com/ness-e/Vantadb) |
| **Current Release** | `v0.7.0` (Production library on PyPI & crates.io) |
| **Engine Architecture** | Embedded, local-first, zero-copy, SIMD-accelerated |
| **Retrieval Mechanics** | Dense Vector (HNSW) + Lexical Full-Text (BM25) with Reciprocal Rank Fusion (RRF) |
| **Durability & Guarantees** | ACID persistence, WAL (Write-Ahead Logging), MVCC snapshot isolation |
| **Ecosystem Connectors** | Python bindings (`vantadb-py`), LangChain (`vantadb-langchain`), Mem0 (`vantadb-mem0`) |

VantaDB provides autonomous agents with low-latency episodic and semantic memory without the operational overhead or latency of external database clusters.

---

## Repositories & Architecture

We maintain a streamlined, zero-bloat repository layout:

| Repository | Scope | Description |
|---|---|---|
| [`VantaDB`](https://github.com/ness-e/Vantadb) | **Core Substrate** | The embedded memory and hybrid retrieval engine (Rust). |
| [`NEGENTROPY`](https://github.com/NegentropyOS/NEGENTROPY) | **Specifications & RFCs** | Architectural blueprints, research roadmap, and agent runtime specifications. |
| [`.github`](https://github.com/NegentropyOS/.github) | **Organization & Governance** | Profile manifesto, development roadmap, and contribution standards. |

---

## Research & Architecture Roadmap

Rather than dispersing into empty repository stubs, our future capabilities are managed as rigorous specifications within [`NegentropyOS/NEGENTROPY`](https://github.com/NegentropyOS/NEGENTROPY):

```
┌─────────────────────────────────────────────────────────────┐
│                      AGENT RUNTIME                          │
└──────────────────────────────┬──────────────────────────────┘
                               ▼
┌─────────────────────────────────────────────────────────────┐
│  Phase 3: Verification & Metacognition (RFC Meta)          │
│  - Execution attestation, audit trails & hallucination checks│
└──────────────────────────────┬──────────────────────────────┘
                               ▼
┌─────────────────────────────────────────────────────────────┐
│  Phase 2: Context & Episodic Grounding (RFC Cardinal)        │
│  - Bitemporal state, token budgeting & working-memory graphs│
└──────────────────────────────┬──────────────────────────────┘
                               ▼
┌─────────────────────────────────────────────────────────────┐
│  Phase 1: Persistent Memory Substrate (VantaDB - Active)    │
│  - Embedded Rust core, HNSW + BM25, ACID local persistence  │
└─────────────────────────────────────────────────────────────┘
```

1. **Substrate (Active):** High-throughput, low-footprint persistent memory via **VantaDB**.
2. **Context Grounding (RFC Cardinal):** Bitemporal working memory tracking what an agent knew, when it learned it, and provenance sources.
3. **Auditability & Trust (RFC Meta):** Cryptographic attestation and immutable audit logging for tool executions.

---

## Engineering Principles

1. **Infrastructure, Not Consumer Apps:** We build the foundational layers others deploy upon.
2. **Local-First & Sovereign:** Minimize external cloud lock-in; optimize for local execution and on-premise governance.
3. **Deterministic State over Probabilistic Guarantees:** Isolate statistical model inference from strict data schemas and transactional storage.
4. **Radical Transparency:** Clear metrics, reproducible benchmarks, and documented failure modes.

📖 **Full Manifesto**: [MANIFESTO.md](https://github.com/NegentropyOS/.github/blob/main/MANIFESTO.md)

---

## Community & Contributing

- **🐛 Issue Tracking**: Submit bugs and benchmarks in relevant repositories.
- **💬 Community**: Join our discussions on [Discord](https://discord.gg/g8nqB3NtXt).
- **📧 Contact**: [NegentropyOS.ia@gmail.com](mailto:NegentropyOS.ia@gmail.com)
- **📖 Contribution Guide**: See [CONTRIBUTING.md](https://github.com/NegentropyOS/.github/blob/main/CONTRIBUTING.md)

---

## License

Code is distributed under the [Apache 2.0 License](https://github.com/NegentropyOS/.github/blob/main/LICENSE).

**NegentropyOS** — Order out of chaos.
