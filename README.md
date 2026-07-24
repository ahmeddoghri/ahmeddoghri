# Ahmed Doghri

**Senior AI Engineer — RAG, multi-agent orchestration, LLM evaluation, and MLOps.** 8+ years shipping production LLM and ML systems in regulated domains (pharma / FDA, banking / fintech, B2B), plus the unglamorous data engineering that keeps them running in production instead of just in a demo.

I care about one thing in AI engineering: claims you can check. The systems below run end to end; the benchmarks regenerate their own numbers. No API keys, mystery services, or copied paper results. The same discipline spans LLM infrastructure and agents through bioinformatics, genomics, vision, and audio.

> 🟢 **Open to senior / staff / lead AI & ML engineering roles** (IC or founding) and AI-product roles — remote, or relocation for the right team. → **[adoghri.com](https://adoghri.com/)**

### 💼 Professional Work

Real systems shipped in regulated and B2B environments. Proprietary, not open source, but the discipline behind them is exactly what the repos below are built to demonstrate.

| Project | Description |
|---------|------------|
| **LLM-Powered Regulatory Submission** | Automated FDA submission process using **7+ LLM pipelines**, reducing errors by **60%**. |
| **AI-Driven RAG System** | NLP-powered **retrieval-augmented generation** system for pharmaceutical documents. |
| **Streaming Data Platform** | Real-time event-driven ML pipeline on **Kafka, Spark, and Flink**. |
| **Biomedical Text Enrichment** | **Transformer models** enriching research papers with biomedical insights. |

### 🚢 Systems You Can Run End To End

These are not notebook demos. Each one has a usable interface, a backend or CLI, persistence where the product needs it, tests, CI, and a documented local or containerized run path.

| Repo | What ships | Check it |
|---|---|---|
| [**spanjudge**](https://github.com/ahmeddoghri/spanjudge) | OTLP agent-trace receiver, SQLite store, operational dashboard, JSON API, CLI, Docker image, and regression policy gate | Six spans rebuild three traces; the fixture passes latency, error, cost, and eval release limits |
| [**vrsbridge**](https://github.com/ahmeddoghri/vrsbridge) | VCF parser, GA4GH VRS 1.3 translator, equivalence engine, browser workbench, JSON API, CLI, and Docker image | Four VCF encodings collapse into two normalized molecular variants |
| [**leterminale**](https://github.com/ahmeddoghri/leterminale) | Browser terminal, encrypted client-side workspace, import/export, keyboard workflow, and static deployment | Open the live product and use it without an account or server-side document store |

### 🔬 The Trust Layer

Ten local-first systems I wanted to exist: tools that decide what to trust across biology, agents, media, and audio. Each ships a CLI, JSON API, browser workbench, Docker image, tests, CI, and an explicit boundary around what its result does not prove.

| Theme | Repo | What it checks | Demo result |
|---|---|---|---|
| **Spatial biology** | [**spatialniche**](https://github.com/ahmeddoghri/spatialniche) | Cell-type neighborhood enrichment against a permuted null | Tumor neighborhood **z = 5.10** across 250 permutations |
| **Protein structure** | [**structuregrade**](https://github.com/ahmeddoghri/structuregrade) | Per-residue pLDDT bands and inter-residue geometry | Grade **C**, mean pLDDT **71.88**, two residues below 50 |
| **CRISPR genomics** | [**crisprradar**](https://github.com/ahmeddoghri/crisprradar) | Both-strand SpCas9 NGG mismatch and seed risk | **1 exact + 2 off-target** sites across 149 bases |
| **Clinical genomics** | [**phenopacketlint**](https://github.com/ahmeddoghri/phenopacketlint) | GA4GH Phenopacket semantic exchange readiness | Three phenotype assertions, quality score **100** |
| **Agent security** | [**mcpinterlock**](https://github.com/ahmeddoghri/mcpinterlock) | MCP tool authority, paths, approvals, secrets, and SSRF | One call denied with **2 independent violations** |
| **ML privacy** | [**unlearnaudit**](https://github.com/ahmeddoghri/unlearnaudit) | Unlearning leakage against retained utility | Membership AUC **1.000 → 0.481**, accuracy stays **0.988** |
| **Video privacy** | [**videoprivacy**](https://github.com/ahmeddoghri/videoprivacy) | Tracked redaction through detector gaps | **10 regions**, two identities, one gap filled |
| **Media provenance** | [**manifestlens**](https://github.com/ahmeddoghri/manifestlens) | C2PA ingredients, actions, signatures, and hard binding | One ingredient, three actions, valid hard binding |
| **Audio delivery** | [**loudnessgate**](https://github.com/ahmeddoghri/loudnessgate) | EBU R128 loudness, range, peak, and normalization | **-18.4 LUFS**, with a measured **+2.4 dB** correction |
| **Music libraries** | [**audiocatalog**](https://github.com/ahmeddoghri/audiocatalog) | Chromaprint duplicates across renamed or transcoded files | One duplicate at **98.65%** similarity |

### 🏆 Flagship Open Source

Six focused repos that isolate the hard parts of shipping LLM systems: cost, safety, hallucinations, memory, evals, and injection defense.

| Repo | What it proves | Result |
|---|---|---|
| [**vllm-cost-router**](https://github.com/ahmeddoghri/vllm-cost-router) | Complexity-based routing, caching, and batching in front of vLLM | **73%** lower cost and p95 latency vs. always-large-model serving |
| [**guardrail-gate**](https://github.com/ahmeddoghri/guardrail-gate) | PII redaction + citation grounding + rate limiting in one pass | **100%** precision/recall on structured PII, **83%** grounded-vs-hallucinated accuracy |
| [**semanticentropy**](https://github.com/ahmeddoghri/semanticentropy) | Hallucination detection via semantic entropy (Farquhar et al., Nature 2024) | Consistent answers score **0.08**, hallucinations **0.90**. No labels, no judge model |
| [**injectguard**](https://github.com/ahmeddoghri/injectguard) | Prompt injection and jailbreak detection with explainable verdicts | **100%** precision and recall on a red-team corpus of attacks and lookalikes |
| [**agentmem**](https://github.com/ahmeddoghri/agentmem) | Bounded, self-consolidating long-term memory for LLM agents | Salience-gated writes, decay-aware retrieval, a hard budget it actually respects |
| [**citebench**](https://github.com/ahmeddoghri/citebench) | What reranking actually buys you in citation-grounded RAG | Citation precision **62% → 88%** on an adversarial benchmark |

### 🧬 Five Research Themes, Ten Working Reproductions

Current research reduced to one mechanism, one baseline, and one number you can rerun. Every repo is MIT licensed, standard-library Python, and tested on 3.9, 3.11, and 3.13.

| Theme | Repo | What it proves | Reproduced result |
|---|---|---|---|
| **Bioinformatics** | [**cellcontext**](https://github.com/ahmeddoghri/cellcontext) | Cellular context matters for perturbation response | MAE **0.2699 → 0.1813** |
| **Bioinformatics** | [**foldcontact**](https://github.com/ahmeddoghri/foldcontact) | Contact constraints keep protein infilling fold-aware | Satisfaction **34.5% → 100%** |
| **Genomics** | [**pangraphmap**](https://github.com/ahmeddoghri/pangraphmap) | Pangenome paths recover structural-variant reads a linear reference loses | **6/25 → 25/25** mapped |
| **Genomics** | [**methyloadapt**](https://github.com/ahmeddoghri/methyloadapt) | Conserved motifs transfer when target-species labels run out | Accuracy **50% → 100%** |
| **Machine learning** | [**driftfilter**](https://github.com/ahmeddoghri/driftfilter) | Forward-only prototypes follow gradual deployment drift | Accuracy **77.9% → 100%** |
| **Machine learning** | [**taskrouter**](https://github.com/ahmeddoghri/taskrouter) | Routing preserves specialists that static merging averages away | MAE **1.379 → 0.000** |
| **Vision + video** | [**distractrack**](https://github.com/ahmeddoghri/distractrack) | Motion and identity memory prevent swaps at object crossings | Accuracy **73.8% → 100%** |
| **Vision + video** | [**d3video**](https://github.com/ahmeddoghri/d3video) | Synthetic motion artifacts show up in the difference of differences | Accuracy **50% → 100%** |
| **Sound + music** | [**restem**](https://github.com/ahmeddoghri/restem) | A separator can improve itself over multiple inference steps | SNR **8.78 → 36.52 dB** |
| **Sound + music** | [**binauralbench**](https://github.com/ahmeddoghri/binauralbench) | A clean stem still fails if it collapses the spatial cue | ILD error reduced **98.3%** |

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
| [**leterminale**](https://github.com/ahmeddoghri/leterminale) | A private, keyboard-first writing terminal with encrypted local workspaces and no account requirement. |
| [**VectorMorph**](https://github.com/ahmeddoghri/VectorMorph) | SVG to animated WebP/GIF with frame blending. Built because Figma's export flaked one time too many. |
| [**ATSProofResume**](https://github.com/ahmeddoghri/ATSProofResume) | Tailors your resume to a job posting without inventing experience. The free version of a $29/month industry. |
| [**bookconverter**](https://github.com/ahmeddoghri/bookconverter) | Local EPUB/MOBI/PDF conversion. No upload limits, no queues, no well-hidden subscription. |

### 📬 Get in Touch

<p>
  <a href="https://adoghri.com/" target="_blank"><img alt="Website" src="https://img.shields.io/badge/Website-%2312100E.svg?&style=for-the-badge&logo=firefox&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/ahmed-doghri/" target="_blank"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" /></a>
</p>
