<div align="center">

<img src="https://raw.githubusercontent.com/JorgeEd13/machine_scanner/main/assets/logo.png" alt="Jorge Edson" width="150"/>

# Jorge Edson
### AI & Data Engineer
#### LLM agents · ML in production · Data pipelines

*From raw GPS traces to conversational AI agents — end-to-end systems, shipped.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jorgeedjson/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jorge.ed.ribeiro00@gmail.com)
[![GitHub followers](https://img.shields.io/github/followers/JorgeEd13?style=for-the-badge&logo=github&logoColor=white&color=181717)](https://github.com/JorgeEd13)

</div>

---

<div align="center">

## ▶ Two live demos — click and try them

**No signup. No API key. They're just up.**

| 🤖 **[Receivables Agent](https://jorgeed-receivables-agent.hf.space)** | 🔧 **[PdM Pipeline](https://forge-pdm-mlops-958199756179.us-central1.run.app/demo)** |
|:---|:---|
| Ask an AI agent about an invoice ledger in plain language. Runs its own **tiny local model** — no key, no quota. | Score live machine telemetry for failure risk. Runs on **managed cloud** (Cloud Run + Neon) at **$0**. |
| [jorgeed-receivables-agent.hf.space](https://jorgeed-receivables-agent.hf.space) | [forge-pdm-mlops…/demo](https://forge-pdm-mlops-958199756179.us-central1.run.app/demo) |

</div>

---

## About me

I'm an **AI & Data Engineer** in Pernambuco, Brazil. I build systems that run the full distance — raw ingestion to production AI — with a bias for things non-technical users can actually operate.

My flagship is a **conversational ReAct agent** (LangGraph) that lets non-technical users query a real fleet database in plain language: governed text-to-SQL, RAG, and GPS anomaly detection behind one authenticated API, on cloud or fully-local models. Underneath it is real data engineering — multi-GB DuckDB stores fed by concurrent ingestion — and a collection-coverage / route-optimization stack over OpenStreetMap that's the part of my work I'd call specialist-grade.

- 🤖 **AI agents & RAG** — governed text-to-SQL, dual cloud/local providers, an MCP server for agent-native tooling
- 🔧 **ML in production** — a full MLOps spine: train → registry → serve → drift → retrain, live on managed cloud
- 📊 **Data engineering at scale** — multi-GB DuckDB, 100K+ GPS records/day, hardware-aware concurrent ingestion
- 🗺️ **Geospatial & optimization** — 4-state coverage modeling and 2-opt TSP routing over OpenStreetMap
- 🎨 **Frontend (React / JS / CSS)** — a genuine second axis: authored control libraries, hand-built SVG dataviz
- 🌍 Open to **remote roles** (Brazil & international)

---

## 🏠 A product I sell

**Its own section on purpose — a different licence and a different audience from the showcase below.** `stillroom` is **source-available under [PolyForm Shield 1.0.0](https://github.com/JorgeEd13/stillroom/blob/main/LICENSE.md)**: read it, run it, modify it internally — you may not resell it as a competing product. **Source-available, not open source.**

### 🏠 [stillroom](https://github.com/JorgeEd13/stillroom)

**A private document assistant that runs entirely on a company's own hardware** — ask questions about your contracts, handbooks and price lists in Word, PDF, Excel or CSV, and get answers that cite the document they came from, with nothing sent to any cloud.

- 🔒 **No cloud path exists to switch on.** There is no fallback provider field, and unknown config keys are rejected rather than ignored — so one cannot be added by a hopeful edit.
- 🙈 **The documents are never sent to me either.** Indexing runs inside the build on the client's own machine; the only thing that travels back is a readiness report with filenames and question text withheld.
- 🤐 **It refuses.** When nothing in the documents is relevant, the model is never called — it says so instead of improvising.
- 🔍 **The privacy claim is auditable, not promised.** The source a client runs is the source published here, so their IT can check what leaves the machine instead of taking my word for it.

`Python · FastAPI · ChromaDB · Ollama · Docker · bge-m3 · zero-build UI`

---

## 🌟 Open-Source Showcase

**Four clean-room projects you can browse end-to-end.** Most of my production work is employer-confidential, so I rebuilt my patterns from scratch here, with **zero proprietary code or data**.

> **The honesty boundary, stated once:** every dataset here is **synthetic**. The numbers below are demonstrations of *process* — diagnosis, governance, measurement — not product performance. The hosted PdM model is a **labelled demo**, and nothing here claims a live production deployment. Each repo says the same thing on every surface it appears.

The last two are a **pair**: a synthetic-telemetry *data engine*, and the *ML-in-production system* built on top of it.

---

### 🤖 [receivables-agent](https://github.com/JorgeEd13/receivables-agent) · **[▶ try it live](https://jorgeed-receivables-agent.hf.space)**

**A shipped AI agent** — ask an invoice ledger questions in plain language, get answers backed by live SQL.

- 🛡️ **Governed text-to-SQL** — defense-in-depth (read-only connection **+** allow/deny-list), plus RAG over a collections-policy corpus.
- 🧩 **Makes a 0.5B model tool-call reliably** — tiny models fail native tool-calling. I measured it, then grammar-constrained the reply to the tool schema: **1/5 → 5/5**.
- ⚡ **Caches the *plan*, never the answer** — repeat questions reuse validated tool calls, but the SQL **re-executes live**, so the number is always current.
- ⚙️ **AI-native** — an **MCP server**, a Claude Code skill, and a `CLAUDE.md`: operable by coding agents, not just humans.

`LangGraph · FastAPI · React · DuckDB · ChromaDB · Gemini/Ollama · Docker · HF Spaces · MCP`

---

### 🔧 [forge-pdm-mlops](https://github.com/JorgeEd13/forge-pdm-mlops) · **[▶ try it live](https://forge-pdm-mlops-958199756179.us-central1.run.app/demo)**

**A complete MLOps spine** — train → registry → serve → drift → retrain → cloud, running end to end.

- 🚦 **A worse model cannot reach production** — metric-gated promotion + rollback, asserted by test. Auto-retrain routes through the **same gate**, so it can never mean *auto-degrade*.
- 🐛 **The bug was in the data, not the model** — the classifier scored 0.55 (chance). Rather than tune it, I measured *why*, traced it upstream, and fixed it there → **0.82 ROC-AUC**.
- 🧭 **Then I measured that 0.82 is the *data's* ceiling** — three probes converged; one **refuted my own hypothesis** and I reported it anyway. Knowing the ceiling is the license to stop optimizing.
- 🌩️ **Operated on managed cloud, not just containerized** — Cloud Run + managed Postgres (Neon) at **$0**, every prediction logged to the managed DB and read back.
- 🏗️ **The infrastructure is code, adopted from a live deploy** — the managed stack (API service, a **separate worker job**, registry, secrets, IAM) is defined in **Terraform**, imported from the running system until `plan` came back clean. Writing the IAM down is what proved the permission model was *wrong*.

`MLflow · LightGBM · Optuna · PyTorch · Evidently · Prefect · FastAPI · Docker · Cloud Run · Postgres (Neon)`

---

### 🛰️ [can-telemetry-forge](https://github.com/JorgeEd13/can-telemetry-forge)

**A synthetic heavy-equipment telemetry generator** — where the *data is the product*. One command builds a reproducible predictive-maintenance dataset for a realistic fleet.

- 📐 **Grounded, not faked** — signals modeled on the public **SAE J1939** standard (real SPNs, units, ranges); climates and road roughness pinned to cited public sources.
- 🧩 **The realism most synthetic CAN data skips** — capability is **gated by model-year era**: a signal an old bus never reported is `NULL`, *not* zero. Failures **degrade progressively** toward the event.
- 🔌 **Down to the wire** — a from-scratch **J1939 frame encoder/decoder** powers fault injection at the transport layer: corruption and truncation written into the *bytes*, decoded back as a receiver would see them.
- 🎲 **Byte-identical from config + seed.** 135 offline tests, ADR-documented.

`Python · NumPy · pandas · Parquet · DuckDB · SAE J1939 · pytest`

---

### 🛠️ [machine_scanner](https://github.com/JorgeEd13/machine_scanner)

**A cross-platform machine-inventory CLI** — one double-click scans the whole machine and opens an interactive HTML report.

- 🖥️ **17 self-registering, fault-isolated collectors** — CPU, RAM modules, GPU, SMBIOS, disks with **SMART**, monitors decoded from **EDID**. A new probe is one module, zero changes elsewhere.
- 🔒 **A second, scoped binary whose spec *excludes* 12 of those collectors** — it answers "can this machine run a local AI model?" and **cannot** read network addresses or serial numbers, which is a property of the artifact rather than a claim about how it was invoked.
- 📦 **One binary per OS** — PyInstaller, shipped by a tag-triggered Actions release whose per-OS smoke test **fails the build if a collector is lost in the freeze**.
- 🧪 **Standard-library only** (psutil the single runtime dependency), **307 offline tests**, CI green on Windows/Linux × Python 3.9–3.13.

`Python · PyInstaller · GitHub Actions · psutil · pytest · stdlib-only`

---

## Tech Stack

### AI & LLMs
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=chainlink&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google%20Gemini-4285F4?style=flat-square&logo=google&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat-square&logo=python&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square&logo=anthropic&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)

### ML & MLOps
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-9ACD32?style=flat-square&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![Optuna](https://img.shields.io/badge/Optuna-2A6EBB?style=flat-square&logo=python&logoColor=white)

### Cloud, DevOps & CI
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Google Cloud Run](https://img.shields.io/badge/Cloud%20Run-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![PyInstaller](https://img.shields.io/badge/PyInstaller-1C7EBB?style=flat-square&logo=python&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

### Data Engineering & Databases
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Apache Parquet](https://img.shields.io/badge/Parquet-50ABF1?style=flat-square&logo=apache&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)

### Geospatial & Frontend
![GeoPandas](https://img.shields.io/badge/GeoPandas-139C5A?style=flat-square&logo=python&logoColor=white)
![Leaflet](https://img.shields.io/badge/Leaflet.js-199900?style=flat-square&logo=leaflet&logoColor=white)
![OpenStreetMap](https://img.shields.io/badge/OpenStreetMap-7EBC6F?style=flat-square&logo=openstreetmap&logoColor=white)
![NetworkX](https://img.shields.io/badge/NetworkX-008080?style=flat-square&logo=python&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

---

## Featured Projects

> These are **employer-confidential and live in private repos** — a walkthrough, not clickable links. The four you *can* browse end-to-end are above. Happy to do a live code walkthrough of the rest.

### 🤖 AI & Agents

| Project | Description | Stack |
|---|---|---|
| 🤖 **Fleet Intelligence Agent** | Conversational ReAct agent that answers fleet questions in plain language — no SQL. Governed text-to-SQL, GPS anomaly detection, RAG. Dual-provider (cloud + fully-local), containerized, one-command Compose stack. | LangGraph · FastAPI · ChromaDB · DuckDB · Docker |
| 🗣️ **Meeting Minutes Generator** | Hybrid local-NLP + LLM pipeline turning raw transcripts into structured minutes — diarization and deterministic extraction cut ~70% of tokens before the LLM. | NLP · LLM · python-docx |

### 📊 Data & ML

| Project | Description | Stack |
|---|---|---|
| 🧠 **Fleet ML — Fuel Anomaly Detection** | LightGBM (Tweedie/Huber) with leakage-free temporal validation (**MAPE ~12.5%** per vehicle-day), ranking vehicle-days by recoverable cost. Feature store: **17.6M GPS points → 43k trips**, engineered in SQL/DuckDB. | LightGBM · DuckDB · pandas |
| 🔬 **Fuel Forensic Audit** | Board-requested audit that reconstructed real fuel use from on-board telemetry (**90M+ GPS points**), cross-checked the fuel-card system, and showed the flagged "anomalies" were **measurement errors, not waste**. | DuckDB · pandas · reportlab |
| 📡 **Fleet Telematics Pipeline** | Production pipeline ingesting **100K+ GPS records/day** via OAuth2 REST, with a hardware-aware dual thread/process concurrency model over a multi-layer DuckDB/Parquet store. | DuckDB · Parquet · OAuth2 |
| 🔀 **Database Sync Engine** | Standalone tool that **diffs 87M+ rows in ~75s** via a single DuckDB `FULL OUTER JOIN`, then merges additively by business key. | DuckDB · SQLite · PyInstaller |

### 🗺️ Geospatial & Optimization

| Project | Description | Stack |
|---|---|---|
| 🗺️ **Collection Coverage Heatmaps** | Coverage analyzer with a **4-state per-segment model** (collected / possible-manual / GPS-failure / missed), topological gap-filling, and dwell-based manual-collection inference. AES-256-GCM client-side encryption, signed PDF reports. | GeoPandas · Leaflet.js · reportlab |
| 🔁 **Route Optimizer (TSP)** | 8-stage collection-route optimizer: morphological clustering + **multi-seed 2-opt** TSP over OpenStreetMap graphs, with a temporal route registry (**SCD-2**) in DuckDB. | NetworkX · GeoPandas · DuckDB |

### ⚙️ Automation & Tooling

| Project | Description | Stack |
|---|---|---|
| 🛠️ **RPA Write-Back Automation** | Selenium automation that goes **beyond scraping**: detects data-entry errors, derives ground truth from GPS, and **writes corrections back** into the portal (declarative edit plan + dry-run). | Selenium · Python · PyInstaller |
| ⏱️ **Real-Time Overtime Alerting** | Daemon that ingests timekeeping into DuckDB (**idempotent, hash-ledgered**), re-derives clock punches from messy data, and emits **WhatsApp** alerts for forming overtime. | Python · DuckDB · WhatsApp |
| 📊 **Internalization Business Case** | Board-facing React app with **hand-built SVG charts** and a financial engine (ROI/payback/multi-scenario sensitivity), built with honest number provenance (measured vs. projected). | React 18 · SVG · JS |
| 📄 **Job-Tailored Resume Builder** | React SPA generating per-job résumé variants from a modular, tag-based content bank, with LLM-assisted adaptation and multi-format export. | React 18 · LLM · localStorage |

---

## GitHub Stats

<!--
  ✅ Stats card servido por uma instância PRÓPRIA do github-readme-stats no Vercel
  (self-host com PAT do Jorge), por isso conta a atividade em repos PRIVADOS.
  Host: github-readme-stats-seven-rose-28.vercel.app  (env var PAT_1 no Vercel).
  Flags-chave: count_private=true + include_all_commits=true (faz "Total Commits"
  contar os privados). hide=contribs esconde o "Contributed to: 0" (esperado).
  Se o token expirar, o card volta a mostrar só público → gerar novo PAT
  (fine-grained, Metadata:Read) e atualizar PAT_1 no Vercel + Redeploy.
  ⚠️ PRIVACIDADE: "Top Languages" pode revelar a DISTRIBUIÇÃO de linguagens dos repos
  privados (não nomes/código). Para ocultar uma linguagem: &hide=<lang> na URL.
  Ver [[user_github_private_repos]] + [[feedback_confidencialidade]].
-->

<div align="center">

<img src="https://github-readme-stats-seven-rose-28.vercel.app/api?username=JorgeEd13&count_private=true&include_all_commits=true&hide=contribs&hide_rank=true&show_icons=true&theme=tokyonight&hide_border=true" height="180em" alt="Jorge's GitHub Stats"/>
&nbsp;
<img src="https://github-readme-stats-seven-rose-28.vercel.app/api/top-langs/?username=JorgeEd13&count_private=true&layout=compact&langs_count=8&hide=jupyter%20notebook&theme=tokyonight&hide_border=true" height="180em" alt="Top Languages"/>

</div>

<div align="center">

<img src="https://streak-stats.demolab.com?user=JorgeEd13&theme=tokyonight&hide_border=true&date_format=j%20M%5B%20Y%5D&cache_seconds=86400" alt="GitHub Streak"/>

</div>

---

## Contribution Activity

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/platane/platane/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/platane/platane/output/github-contribution-grid-snake.svg">
  <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/platane/platane/output/github-contribution-grid-snake-dark.svg">
</picture>

---

<div align="center">

*"The goal is to turn data into information, and information into insight."* — Carly Fiorina

</div>
