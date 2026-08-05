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

These are not notebook demos. Each one has a usable interface, a backend or CLI, persistence where the product needs it, tests, and a documented local or containerized run path.

| Repo | What ships | Check it |
|---|---|---|
| [**spanjudge**](https://github.com/ahmeddoghri/spanjudge) | OTLP agent-trace receiver, SQLite store, operational dashboard, JSON API, CLI, Docker image, and regression policy gate | Six spans rebuild three traces; the fixture passes latency, error, cost, and eval release limits |
| [**vrsbridge**](https://github.com/ahmeddoghri/vrsbridge) | VCF parser, GA4GH VRS 1.3 translator, equivalence engine, browser workbench, JSON API, CLI, and Docker image | Four VCF encodings collapse into two normalized molecular variants |

### 🔬 The Trust Layer

Ten local-first systems I wanted to exist: tools that decide what to trust across biology, agents, media, and audio. Each ships a CLI, JSON API, browser workbench, Docker image, tests, and an explicit boundary around what its result does not prove.

| Theme | Repo | What it checks | Demo result |
|---|---|---|---|
| **Spatial biology** | [**spatialniche**](https://github.com/ahmeddoghri/spatialniche) | Cell-type neighborhood enrichment against a permuted null | Tumor neighborhood **z = 5.10** across 250 permutations |
| **Protein structure** | [**structuregrade**](https://github.com/ahmeddoghri/structuregrade) | Per-residue pLDDT bands and inter-residue geometry | Grade **C**, mean pLDDT **71.88**, two residues below 50 |
| **CRISPR genomics** | [**crisprradar**](https://github.com/ahmeddoghri/crisprradar) | Both-strand SpCas9 NGG mismatch and seed risk | **1 exact + 2 off-target** sites across 149 bases |
| **Clinical genomics** | [**phenopacketlint**](https://github.com/ahmeddoghri/phenopacketlint) | GA4GH Phenopacket semantic exchange readiness | Three phenotype assertions, quality score **100** |
| **Agent security** | [**mcpinterlock**](https://github.com/ahmeddoghri/mcpinterlock) | MCP tool authority, paths, approvals, secrets, and SSRF | One call denied with **2 independent violations** |
| **ML privacy** | [**unlearnaudit**](https://github.com/ahmeddoghri/unlearnaudit) | Unlearning leakage against retained utility | Original metric was a self-lookup tautology; leave-one-out correction finds **no detectable leak** |
| **Video privacy** | [**videoprivacy**](https://github.com/ahmeddoghri/videoprivacy) | Tracked redaction through detector gaps | **10 regions**, two identities, one gap filled |
| **Media provenance** | [**manifestlens**](https://github.com/ahmeddoghri/manifestlens) | C2PA ingredients, actions, signatures, and hard binding | One ingredient, three actions, valid hard binding |
| **Audio delivery** | [**loudnessgate**](https://github.com/ahmeddoghri/loudnessgate) | EBU R128 loudness, range, peak, and normalization | **-18.4 LUFS**, with a measured **+2.4 dB** correction |
| **Music libraries** | [**audiocatalog**](https://github.com/ahmeddoghri/audiocatalog) | Chromaprint duplicates across renamed or transcoded files | One duplicate at **99.48%** similarity |

### ⚡ The Frontier Lab

Ten useful experiments at the edge of current ML engineering. Every result below comes from the committed fixture or an actual generated media artifact, not from the source paper.

| Theme | Repo | End-to-end job | Demo result |
|---|---|---|---|
| **Genomics** | [**strandshift**](https://github.com/ahmeddoghri/strandshift) | Audit sequence models across strand and window transforms | **18 views**, prediction range **0.3273** after fixing a strand-orientation bug |
| **Rare disease** | [**phenorank**](https://github.com/ahmeddoghri/phenorank) | Rank HPO disease candidates and test stability | Top score **0.6334**, stable **3/3** |
| **ML security** | [**tensorwarden**](https://github.com/ahmeddoghri/tensorwarden) | Scan real checkpoint containers without loading them | Safe artifact accepted; **2 quarantined** |
| **LLM privacy** | [**cacheisolate**](https://github.com/ahmeddoghri/cacheisolate) | Reproduce and stop cross-tenant cache timing leakage | **86 ms** oracle removed with useful reuse retained |
| **RAG security** | [**ragpoisonbench**](https://github.com/ahmeddoghri/ragpoisonbench) | Inject corpus poison and test provenance quarantine | Recall **1.0 → 0.0 → 1.0** |
| **3D vision** | [**splatgrade**](https://github.com/ahmeddoghri/splatgrade) | Parse and grade Gaussian Splat PLY artifacts | Grade **D / 49**, every defect localized |
| **Generated video** | [**physicsvideo**](https://github.com/ahmeddoghri/physicsvideo) | Render MP4 scenarios and audit physical consistency | **4/4 faults**, **0** false positives |
| **Multimodal media** | [**avsyncdoctor**](https://github.com/ahmeddoghri/avsyncdoctor) | Detect and repair offset plus clock drift | **120 ms**, **5,000 ppm**, repaired below **40 ms** |
| **Audio engineering** | [**codecguard**](https://github.com/ahmeddoghri/codecguard) | Run real codec round trips behind a CI quality gate | Clean build passes; degraded build fails **4/4** gates |
| **Robot safety** | [**safepathshield**](https://github.com/ahmeddoghri/safepathshield) | Project policy actions onto a barrier constraint | Collision steps **39 → 0**, goal still reached |

### 🏆 Flagship Open Source

Six focused repos that isolate the hard parts of shipping LLM systems: cost, safety, hallucinations, memory, evals, and injection defense.

| Repo | What it proves | Result |
|---|---|---|
| [**vllm-cost-router**](https://github.com/ahmeddoghri/vllm-cost-router) | Complexity-based routing, caching, and batching in front of vLLM | **73%** lower cost and p95 latency vs. always-large-model serving |
| [**guardrail-gate**](https://github.com/ahmeddoghri/guardrail-gate) | PII redaction + citation grounding + rate limiting in one pass | Adversarial suite found the original grounding check missed **6/8** hallucinations; fixed check scores **85%** on the same set (was **46%**) |
| [**semanticentropy**](https://github.com/ahmeddoghri/semanticentropy) | Hallucination detection via semantic entropy (Farquhar et al., Nature 2024) | Consistent answers score **0.08**, hallucinations **0.90**. No labels, no judge model |
| [**injectguard**](https://github.com/ahmeddoghri/injectguard) | Prompt injection and jailbreak detection with explainable verdicts | **100%** precision and recall on a red-team corpus of attacks and lookalikes |
| [**agentmem**](https://github.com/ahmeddoghri/agentmem) | Bounded, self-consolidating long-term memory for LLM agents | Salience-gated writes, decay-aware retrieval, a hard budget it actually respects |
| [**citebench**](https://github.com/ahmeddoghri/citebench) | What reranking actually buys you in citation-grounded RAG | The published **62% → 88%** lift was filename leakage; blinded content-based reranking still reaches **100%**, zero fabricated citations |

### 🧬 Five Research Themes, Ten Working Reproductions

Current research reduced to one mechanism, one baseline, and one number you can rerun. Every repo is MIT licensed, standard-library Python, and tested on 3.9, 3.11, and 3.13.

| Theme | Repo | What it proves | Reproduced result |
|---|---|---|---|
| **Bioinformatics** | [**cellcontext**](https://github.com/ahmeddoghri/cellcontext) | Cellular context matters for perturbation response | MAE **0.2699 → 0.1813** |
| **Bioinformatics** | [**foldcontact**](https://github.com/ahmeddoghri/foldcontact) | Contact constraints keep protein infilling fold-aware | Satisfaction **34.5% → 100%** |
| **Genomics** | [**pangraphmap**](https://github.com/ahmeddoghri/pangraphmap) | Pangenome paths recover structural-variant reads a linear reference loses | Published **6/25 → 25/25** was a tautology (error-free reads); with realistic sequencing error, gain holds at **~58pt mean** across 65 seeds |
| **Genomics** | [**methyloadapt**](https://github.com/ahmeddoghri/methyloadapt) | Conserved motifs transfer when target-species labels run out | Accuracy **50% → 100%** |
| **Machine learning** | [**driftfilter**](https://github.com/ahmeddoghri/driftfilter) | Forward-only prototypes follow gradual deployment drift | Accuracy **77.9% → 100%** at the shipped drift rate; a position-only EMA falls to 68.6% at 4.4x faster drift, fixed with velocity tracking |
| **Machine learning** | [**taskrouter**](https://github.com/ahmeddoghri/taskrouter) | Routing preserves specialists that static merging averages away | MAE **1.399 → 0.276**, an 80.2% reduction with a real noise floor (a 0.000 MAE would have meant the benchmark couldn't fail) |
| **Vision + video** | [**distractrack**](https://github.com/ahmeddoghri/distractrack) | Motion and identity memory prevent swaps at object crossings | Published **73.8% → 100%** read the ground-truth label directly; genuine label-free fix recovers **~1.7–2.8pt**, not 26pt |
| **Vision + video** | [**d3video**](https://github.com/ahmeddoghri/d3video) | Synthetic motion artifacts show up in the difference of differences | Published **100%/54pt** used a best-case artifact; a plausible weaker one drops it to **~72-73%/23pt** — mechanism holds, magnitude overstated |
| **Sound + music** | [**restem**](https://github.com/ahmeddoghri/restem) | A separator can improve itself over multiple inference steps | Published **8.78 → 36.52 dB** hardcoded the interferer frequency (0.5 Hz off collapses the gain to 0); estimating it holds **~20 dB** mean gain across dozens of unseen frequencies |
| **Sound + music** | [**binauralbench**](https://github.com/ahmeddoghri/binauralbench) | A clean stem still fails if it collapses the spatial cue | ILD error reduced **99.8%** |

### 🧪 The Rest of the Lab

The same standard (reproducible benchmark, tests, zero dependencies) applied across the stack. Grouped so you can jump to what you care about.

**LLM inference and cost.** [speculabench](https://github.com/ahmeddoghri/speculabench) (speculative decoding math, 1.4x to 2.9x — the optimal draft length shifts once real bursty agreement patterns replace an independent-draw assumption), [kvsqueeze](https://github.com/ahmeddoghri/kvsqueeze) (KV-cache eviction, H2O and StreamingLLM style — the original policy's "win" was freezing the cache entirely, scoring 0% on recent-token recall; fixed), [contextpack](https://github.com/ahmeddoghri/contextpack) (prompt compression with a recall check — the safe-compression knee point only held when the source text used digit numerals; fixed for prose-spelled numbers too).

**Output reliability.** [structstream](https://github.com/ahmeddoghri/structstream) (JSON repair, 7% → 100% recovery on the bundled corpus, 0% on a common failure mode it originally never tested — now fixed), [rubricagent](https://github.com/ahmeddoghri/rubricagent) (LLM-as-judge rubrics learned from outcomes, AUC 0.77 → 1.00, confirmed on a disjoint holdout), [taggate](https://github.com/ahmeddoghri/taggate) (confidence-gated tagging in TypeScript).

**RAG done honestly.** [chunklab](https://github.com/ahmeddoghri/chunklab) (chunking strategies, measured — the 30-point margin on the bundled document nearly disappears on a second, independent one), [clarifyrag](https://github.com/ahmeddoghri/clarifyrag) (asks clarifying questions only when evidence disagrees — auditing its own circular benchmark surfaced a real stopword-filtering bug, fixed, natural-question accuracy 3/7 → 7/7), [tablextract](https://github.com/ahmeddoghri/tablextract) (tables out of PDFs with cited cells — found and fixed silently-dropped rows and fabricated citations, recall 71% → 100%).

**Agents that stop.** [toolrouter](https://github.com/ahmeddoghri/toolrouter) (tool selection that abstains on ties, though it also abstains on 10/15 real natural-language queries — fixed), [agentbudget](https://github.com/ahmeddoghri/agentbudget) (loop detection catching stalls that step limits miss, plus a blind spot of its own it didn't originally catch), [debatekit](https://github.com/ahmeddoghri/debatekit) (multiagent debate: the panel effect, 57% → 79%, is real; the extra lift from debate *rounds* specifically never clears one standard error at proper sample size).

**ML beyond LLMs.** [churnfm](https://github.com/ahmeddoghri/churnfm) (drift-triggered retraining), [orthoshift](https://github.com/ahmeddoghri/orthoshift) (double ML for causal effects — a multi-seed check found plain adjustment quietly beats it as often as it loses), [fedcal](https://github.com/ahmeddoghri/fedcal) (non-IID federated learning — a single-seed calibration win reverses to a net loss across 60 seeds), [riskbandit](https://github.com/ahmeddoghri/riskbandit) (conformal risk-controlled bandits — the quantile formula undercovered its own stated 90% target by 1-1.5pt, fixed), [chronopatch](https://github.com/ahmeddoghri/chronopatch) (conformal forecasting — the gain holds on the paper's exact seasonality, drops to single digits on a different but equally realistic series shape), [graphpulse](https://github.com/ahmeddoghri/graphpulse) (graph anomaly scoring — most of the published AUC traced back to reading the ground-truth label directly; the honest label-free score is lower but still clearly ahead of degree alone), [tabflowmini](https://github.com/ahmeddoghri/tabflowmini) (synthetic tabular data with an audit — the "fit" churn model was the generator's own coefficients copy-pasted, now actually fit), [proteinmask](https://github.com/ahmeddoghri/proteinmask) (masked protein-like infilling, honestly toy — its "random baseline" was a rigged formula tuned to never match, fixed to a real uniform draw), [pendulumlab](https://github.com/ahmeddoghri/pendulumlab) (CEM control from scratch — beats a fair grid-search baseline, not just an under-tuned guess), [motifdiff](https://github.com/ahmeddoghri/motifdiff) (symbolic music that grades itself — isolated the weighting's real contribution once two confounds were removed), [connectpuct](https://github.com/ahmeddoghri/connectpuct) (PUCT Connect Four you can play — a perfect record vs. weak baselines drops to ~55% against real depth-3 minimax, a fair fight).

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
