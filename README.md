<div align="center">

<!-- Brand mark (hipercubo). Servido por raw URL de um repo público p/ renderizar
     no perfil. Alternativa: commitar o logo em JorgeEd13/JorgeEd13/assets/ e usar
     caminho relativo. Ver memória [[reference_brand_logo]]. -->
<img src="https://raw.githubusercontent.com/JorgeEd13/machine_scanner/main/assets/logo.png" alt="Jorge Edson" width="150"/>

# Jorge Edson
### AI & Data Engineer
#### LLM agents · Data pipelines · GIS & optimization

*Building end-to-end systems — from raw GPS traces to conversational AI agents, from data pipelines to actionable insight.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jorgeedjson/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jorge.ed.ribeiro00@gmail.com)
[![GitHub followers](https://img.shields.io/github/followers/JorgeEd13?style=for-the-badge&logo=github&logoColor=white&color=181717)](https://github.com/JorgeEd13)

</div>

---

## About me

I'm an **AI & Data Engineer** based in Pernambuco, Brazil. I build systems that run the full distance — from raw data ingestion to production AI — with a bias for things non-technical users can actually operate: **LLM agents, data pipelines, ML models, and geospatial analytics**.

I lead with **AI engineering**: my flagship is a **conversational ReAct agent** (LangGraph) that lets non-technical users query a real fleet database in plain language — no SQL. It pairs **governed text-to-SQL** (defense-in-depth: allow/deny-list **+** read-only DB) with **RAG** (ChromaDB) and **GPS anomaly detection** behind a single authenticated REST API, running on either Google Gemini (cloud, active-probe fallback) or fully local Ollama models — packaged so it comes up with one command.

Underneath the agents is real **data & geospatial engineering**: multi-GB DuckDB stores fed by concurrent ingestion, and a **collection-coverage / route-optimization** stack over OpenStreetMap that's the part of my work I'd call specialist-grade.

- 🤖 **AI agents & RAG on real operational data** — governed text-to-SQL, dual cloud/local providers with active fallback, an **MCP server** for agent-native tooling
- 📊 **Data engineering at scale** — multi-GB DuckDB stores, 100K+ GPS records/day, hardware-aware concurrent ingestion
- 🗺️ **Geospatial & optimization** — 4-state collection-coverage modeling and multi-seed 2-opt TSP route optimization over OpenStreetMap
- 🧠 **Applied ML** — fuel-anomaly detection (LightGBM) with a baseline-first, leakage-free discipline *(a self-supervised TCN encoder is designed/documented as a next phase, not shipped)*
- 🎨 **Frontend (React / JS / CSS)** — a genuine second axis: authored control libraries, hand-built SVG dataviz, client-side Web Crypto
- 🌟 **Public, browsable showcase** — [receivables-agent](https://github.com/JorgeEd13/receivables-agent) (clean-room AI agent) and [machine_scanner](https://github.com/JorgeEd13/machine_scanner) (cross-platform inventory CLI); most of my production work is private/employer-confidential
- 🌍 Open to **remote roles** (Brazil & international)

---

## 🌟 Open-Source Showcase

**Two fully public, clean-room projects you can browse end-to-end.** Most of my production work is employer-confidential, so I rebuilt my patterns from scratch here, with **zero proprietary code or data**.

### 🤖 [receivables-agent](https://github.com/JorgeEd13/receivables-agent) — a shipped AI agent

- 🧠 **Conversational ReAct agent** (LangGraph) with **defense-in-depth governed text-to-SQL** (read-only connection + allow/deny-list) over **1M+ synthetic invoices**, plus **RAG** (ChromaDB) over a collections-policy knowledge base.
- 🔌 **Dual-provider** — Google Gemini (cloud) or **Ollama (fully local/offline)**, with active-probe fallback.
- 🧱 **Full-stack & shipped** — FastAPI + React, one-command **Docker Compose**, **76 offline tests**, a property-based **eval suite** (golden questions), and architecture decisions captured as **ADRs**.
- ⚙️ **AI-native by design** — an **MCP server**, a **Claude Code skill**, and a `CLAUDE.md`, so the project is operable by coding agents, not just humans.

`LangGraph · FastAPI · React · DuckDB · ChromaDB · Gemini / Ollama · Docker · MCP · pytest`

### 🛠️ [machine_scanner](https://github.com/JorgeEd13/machine_scanner) — a cross-platform machine-inventory CLI

- 🖥️ **One scan of the whole machine** — 16 self-registering, isolated collectors map hardware (CPU, RAM modules, GPU, SMBIOS), physical disks with **SMART health**, and peripherals (USB, monitors decoded from **EDID**, battery, bluetooth, printers) into **text / JSON / interactive HTML**.
- 📦 **Drop-on-a-USB-stick portability** — one codebase packaged by **PyInstaller** into one binary per OS (Windows / Linux / macOS), published by a **tag-triggered GitHub Actions release** with a per-OS smoke test that fails the build if any collector is lost in the freeze.
- 🎁 **Product-minded UX** — a plain double-click scans, writes a self-contained HTML report and opens it in the browser, with the filename localized to the OS language.
- 🧪 **Engineered like production** — **240 offline tests**, ADR-documented decisions, **standard-library only** (psutil the single runtime dependency), CI green across Windows/Linux × Python 3.9–3.13.

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

### Data Science & ML
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-9ACD32?style=flat-square&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)

### Geospatial & GIS
![GeoPandas](https://img.shields.io/badge/GeoPandas-139C5A?style=flat-square&logo=python&logoColor=white)
![Shapely](https://img.shields.io/badge/Shapely-2C8EBB?style=flat-square&logo=python&logoColor=white)
![Leaflet](https://img.shields.io/badge/Leaflet.js-199900?style=flat-square&logo=leaflet&logoColor=white)
![OpenStreetMap](https://img.shields.io/badge/OpenStreetMap-7EBC6F?style=flat-square&logo=openstreetmap&logoColor=white)
![NetworkX](https://img.shields.io/badge/NetworkX-008080?style=flat-square&logo=python&logoColor=white)

### Data Engineering & Databases
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Apache Parquet](https://img.shields.io/badge/Parquet-50ABF1?style=flat-square&logo=apache&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

### Automation & APIs
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)
![REST API](https://img.shields.io/badge/REST%20API-FF6C37?style=flat-square&logo=postman&logoColor=white)
![OAuth2](https://img.shields.io/badge/OAuth2-EB5424?style=flat-square&logo=auth0&logoColor=white)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-59666C?style=flat-square&logo=python&logoColor=white)

### DevOps, CI & Packaging
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![PyInstaller](https://img.shields.io/badge/PyInstaller-1C7EBB?style=flat-square&logo=python&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

### Frontend
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

---

## Featured Projects

> Most of the projects below are **employer-confidential and live in private repos** — this is the walkthrough, not a set of clickable links. The ones you can browse end-to-end are **[receivables-agent](https://github.com/JorgeEd13/receivables-agent)** and **[machine_scanner](https://github.com/JorgeEd13/machine_scanner)** (above). Happy to do a live code walkthrough of the rest.

### 🤖 AI & Agents

| Project | Description | Stack |
|---|---|---|
| 🤖 **Fleet Intelligence Agent** | Conversational AI agent (LangGraph ReAct) that answers fleet questions in plain language — no SQL. **Governed text-to-SQL** (allow/deny-list **+** read-only DB, defense-in-depth), GPS anomaly detection, and RAG (ChromaDB). Dual-provider: Gemini (cloud, active-probe fallback) and Ollama (fully local). Authenticated FastAPI, hardware-aware model selection, `pytest` suite on the SQL guardrail, and a **containerized deploy** — image built and running, one-command **Docker Compose** stack (API + local LLM + HTTPS reverse proxy) with opt-in GPU. | LangGraph · FastAPI · ChromaDB · DuckDB · Gemini/Ollama · Docker |
| 🗣️ **Meeting Minutes Generator** | Hybrid local-NLP + LLM pipeline turning raw transcripts into structured minutes (DOCX) — speaker diarization and deterministic data extraction cut ~70% of tokens before the LLM. Cloud (Gemini) or local (Ollama). | NLP · LLM · python-docx |

### 📊 Data & ML

| Project | Description | Stack |
|---|---|---|
| 🧠 **Fleet ML — Fuel Anomaly Detection** | LightGBM (Tweedie/Huber) with leakage-free temporal validation (**MAPE ~12.5%** per vehicle-day), ranking vehicle-days by recoverable cost. Feature store of **17.6M GPS points → 43k trips**, engineered 100% in SQL/DuckDB. *(A self-supervised TCN encoder is designed/documented as a next phase, not shipped.)* | LightGBM · DuckDB · pandas |
| 🔬 **Fuel Forensic Audit** | Board-requested audit that reconstructed real fuel use (liters/km) straight from on-board telemetry counters (**90M+ GPS points**), cross-checked it against the fuel-card system, and showed the flagged "anomalies" were **data/measurement errors, not waste** — with driver attribution and an executive PDF for a non-technical audience. | DuckDB · pandas · reportlab |
| 📡 **Fleet Telematics Pipeline** | Production pipeline ingesting **100K+ GPS records/day** via REST API (OAuth2), with a **dual thread/process concurrency model** (hardware-aware) and a multi-layer DuckDB/Parquet store with incremental fetching. | DuckDB · Parquet · OAuth2 |
| 🔀 **Database Sync Engine** | Standalone tool that **diffs 87M+ rows in ~75s** via a single DuckDB `FULL OUTER JOIN` with conditional aggregation, then merges additively by business key. | DuckDB · SQLite · PyInstaller |

### 🗺️ Geospatial & Optimization

| Project | Description | Stack |
|---|---|---|
| 🗺️ **Collection Coverage Heatmaps** | Interactive geospatial coverage analyzer with a **4-state per-segment model** (collected / possible-manual / GPS-failure / missed) over a projected CRS, topological gap-filling, dwell-based manual-collection inference, plus AES-256-GCM client-side encryption and signed PDF reports. | GeoPandas · Leaflet.js · reportlab |
| 🔁 **Route Optimizer (TSP)** | 8-stage pipeline for collection-route optimization: morphological clustering + **multi-seed 2-opt / or-opt** TSP + shortest-path routing over OpenStreetMap graphs; temporal route registry (**SCD-2**) in DuckDB. | NetworkX · GeoPandas · DuckDB |

### ⚙️ Automation & Tooling

| Project | Description | Stack |
|---|---|---|
| 🛠️ **RPA Write-Back Automation** | Selenium automation over a fleet portal that goes **beyond scraping**: detects data-entry errors, derives ground truth from GPS, and **writes corrections back** into the system (declarative edit plan + dry-run). Shipped as a standalone `.exe`. | Selenium · Python · PyInstaller |
| ⏱️ **Real-Time Overtime Alerting** | Daemon that ingests workforce timekeeping into DuckDB (**idempotent, hash-ledgered**), re-derives clock punches from messy positional data, and emits end-of-shift **WhatsApp** alerts for forming overtime — with anti-spam state. | Python · DuckDB · WhatsApp |
| 📄 **Job-Tailored Resume Builder** *(personal product)* | React 18 SPA that generates per-job résumé variants from a modular, tag-based content bank, with **LLM-assisted adaptation** (structured-JSON extraction) and multi-format export (PDF / Word / Markdown). | React 18 · LLM · localStorage |
| 📊 **Internalization Business Case** *(React + dataviz)* | Interactive board-facing app (React 18, authored control library) with **hand-built SVG charts** and a financial engine (ROI/payback/multi-scenario sensitivity), built with honest number provenance (measured vs. projected). | React 18 · SVG · JS |

---

## GitHub Stats

<!--
  ✅ Stats card servido por uma instância PRÓPRIA do github-readme-stats no Vercel
  (self-host com PAT do Jorge), por isso conta a atividade em repos PRIVADOS.
  Host: github-readme-stats-seven-rose-28.vercel.app  (env var PAT_1 no Vercel).
  Flags-chave: count_private=true (soma stars/commits de privados) +
  include_all_commits=true (faz "Total Commits" contar os privados — sem ela
  caía p/ ~36/ano só dos públicos; com ela = 609). hide=contribs esconde o
  "Contributed to: 0" (não há contribuição em repos de terceiros, é esperado).
  Se o token expirar, o card volta a mostrar só público → gerar novo PAT
  (fine-grained, Metadata:Read) e atualizar PAT_1 no Vercel + Redeploy.
  ⚠️ PRIVACIDADE: o card "Top Languages" pode revelar a DISTRIBUIÇÃO de linguagens
  dos repos privados (não nomes/código). Para ocultar uma linguagem específica,
  acrescentar &hide=<lang>,<lang> na URL do langs-card. Ver [[user_github_private_repos]]
  + [[feedback_confidencialidade]].
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
