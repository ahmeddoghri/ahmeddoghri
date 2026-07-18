# Ahmed Doghri

Senior AI Engineer. 7+ years building LLM systems, NLP pipelines, and the unglamorous data engineering that keeps them running in production instead of just in a demo.

I care about one thing in AI engineering: claims you can check. Every open source repo below ships a benchmark that reproduces locally, with no API keys and no asterisk. If a number is in a README, a command in that README regenerates it.

### 💼 Professional Work

Real systems shipped in regulated and B2B environments. Proprietary, not open source, but the discipline behind them is exactly what the repos below are built to demonstrate.

| Project | Description |
|---------|------------|
| **LLM-Powered Regulatory Submission** | Automated FDA submission process using **7+ LLM pipelines**, reducing errors by **60%**. |
| **AI-Driven RAG System** | NLP-powered **retrieval-augmented generation** system for pharmaceutical documents. |
| **Streaming Data Platform** | Real-time event-driven ML pipeline on **Kafka, Spark, and Flink**. |
| **Biomedical Text Enrichment** | **Transformer models** enriching research papers with biomedical insights. |

### 🏆 Flagship Open Source

Six repos that cover the full surface of shipping LLM systems: cost, safety, hallucinations, memory, evals, and injection defense.

| Repo | What it proves | Result |
|---|---|---|
| [**vllm-cost-router**](https://github.com/ahmeddoghri/vllm-cost-router) | Complexity-based routing, caching, and batching in front of vLLM | **73%** lower cost and p95 latency vs. always-large-model serving |
| [**guardrail-gate**](https://github.com/ahmeddoghri/guardrail-gate) | PII redaction + citation grounding + rate limiting in one pass | **100%** precision/recall on structured PII, **83%** grounded-vs-hallucinated accuracy |
| [**semanticentropy**](https://github.com/ahmeddoghri/semanticentropy) | Hallucination detection via semantic entropy (Farquhar et al., Nature 2024) | Consistent answers score **0.08**, hallucinations **0.90**. No labels, no judge model |
| [**injectguard**](https://github.com/ahmeddoghri/injectguard) | Prompt injection and jailbreak detection with explainable verdicts | **100%** precision and recall on a red-team corpus of attacks and lookalikes |
| [**agentmem**](https://github.com/ahmeddoghri/agentmem) | Bounded, self-consolidating long-term memory for LLM agents | Salience-gated writes, decay-aware retrieval, a hard budget it actually respects |
| [**citebench**](https://github.com/ahmeddoghri/citebench) | What reranking actually buys you in citation-grounded RAG | Citation precision **62% → 88%** on an adversarial benchmark |

### 🧪 The Rest of the Lab

The same standard (reproducible benchmark, tests, CI, zero dependencies) applied across the stack. Grouped so you can jump to what you care about.

**LLM inference and cost.** [speculabench](https://github.com/ahmeddoghri/speculabench) (speculative decoding math, 1.4x to 2.9x), [kvsqueeze](https://github.com/ahmeddoghri/kvsqueeze) (KV-cache eviction, H2O and StreamingLLM style), [contextpack](https://github.com/ahmeddoghri/contextpack) (prompt compression with a recall check).

**Output reliability.** [structstream](https://github.com/ahmeddoghri/structstream) (JSON repair, 7% → 100% recovery), [rubricagent](https://github.com/ahmeddoghri/rubricagent) (LLM-as-judge rubrics learned from outcomes, AUC 0.77 → 1.00), [taggate](https://github.com/ahmeddoghri/taggate) (confidence-gated tagging in TypeScript).

**RAG done honestly.** [chunklab](https://github.com/ahmeddoghri/chunklab) (chunking strategies, measured), [clarifyrag](https://github.com/ahmeddoghri/clarifyrag) (asks clarifying questions only when evidence disagrees), [tablextract](https://github.com/ahmeddoghri/tablextract) (tables out of PDFs with cited cells).

**Agents that stop.** [toolrouter](https://github.com/ahmeddoghri/toolrouter) (tool selection that abstains on ties), [agentbudget](https://github.com/ahmeddoghri/agentbudget) (loop detection catching stalls that step limits miss), [debatekit](https://github.com/ahmeddoghri/debatekit) (multiagent debate, 57% → 80%).

**ML beyond LLMs.** [churnfm](https://github.com/ahmeddoghri/churnfm) (drift-triggered retraining), [orthoshift](https://github.com/ahmeddoghri/orthoshift) (double ML for causal effects), [fedcal](https://github.com/ahmeddoghri/fedcal) (non-IID federated learning), [riskbandit](https://github.com/ahmeddoghri/riskbandit) (conformal risk-controlled bandits), [chronopatch](https://github.com/ahmeddoghri/chronopatch) (conformal forecasting), [graphpulse](https://github.com/ahmeddoghri/graphpulse) (graph anomaly scoring), [tabflowmini](https://github.com/ahmeddoghri/tabflowmini) (synthetic tabular data with an audit), [proteinmask](https://github.com/ahmeddoghri/proteinmask) (masked protein-like infilling, honestly toy), [pendulumlab](https://github.com/ahmeddoghri/pendulumlab) (CEM control from scratch), [motifdiff](https://github.com/ahmeddoghri/motifdiff) (symbolic music that grades itself), [connectpuct](https://github.com/ahmeddoghri/connectpuct) (PUCT Connect Four you can play).

### 🛠️ Products People Actually Use

| Tool | What it does |
|---|---|
| [**VectorMorph**](https://github.com/ahmeddoghri/VectorMorph) | SVG to animated WebP/GIF with frame blending. Built because Figma's export flaked one time too many. |
| [**ATSProofResume**](https://github.com/ahmeddoghri/ATSProofResume) | Tailors your resume to a job posting without inventing experience. The free version of a $29/month industry. |
| [**bookconverter**](https://github.com/ahmeddoghri/bookconverter) | Local EPUB/MOBI/PDF conversion. No upload limits, no queues, no well-hidden subscription. |

### 📬 Get in Touch

<p>
  <a href="https://adoghri.com/" target="_blank"><img alt="Website" src="https://img.shields.io/badge/Website-%2312100E.svg?&style=for-the-badge&logo=firefox&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/ahmed-doghri/" target="_blank"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" /></a>
</p>
