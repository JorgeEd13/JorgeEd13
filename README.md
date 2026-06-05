<div align="center">

# Jorge Edson
### Data & AI Engineer · GIS & Optimization

*Building end-to-end systems — from raw GPS traces to conversational AI agents, from data pipelines to actionable insight.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jorgeedjson/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jorge.ed.ribeiro00@gmail.com)
[![GitHub followers](https://img.shields.io/github/followers/JorgeEd13?style=for-the-badge&logo=github&logoColor=white&color=181717)](https://github.com/JorgeEd13)

</div>

---

## About me

I'm a **Data & AI Engineer** based in Pernambuco, Brazil. I build end-to-end systems that go all the way from raw data ingestion to production AI — data pipelines, ML models, geospatial analytics, and LLM-powered agents that non-technical users can actually use.

My flagship project is a **conversational AI agent** (LangGraph ReAct) that lets non-technical users query a real fleet database in plain Portuguese — no SQL required. It combines a production data pipeline, GPS anomaly detection, and semantic search (RAG) behind a single authenticated REST API, and runs on either Google Gemini (cloud) or fully local Ollama models.

- 🤖 Building **AI agents & RAG systems** on real operational data — governed text-to-SQL, dual cloud/local providers with active fallback
- 📊 **Data engineering at scale** — multi-GB DuckDB stores, 100K+ GPS records/day, concurrent ingestion
- 🗺️ **Geospatial & optimization** — collection-coverage modeling and TSP route optimization over OpenStreetMap
- 🧠 **Applied ML** — fuel-anomaly detection (LightGBM) with a baseline-first, leakage-free discipline
- 🎨 **Frontend background** (React / JS / CSS) — keeps me focused on usability when building data products
- 🌍 Open to **remote roles** (Brazil & international)

---

## Tech Stack

### AI & LLMs
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=chainlink&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google%20Gemini-4285F4?style=flat-square&logo=google&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat-square&logo=python&logoColor=white)
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

### Frontend (Background)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

---

## Featured Projects

| Project | Description | Stack |
|---|---|---|
| 🤖 **Fleet Intelligence Agent** | Conversational AI agent (LangGraph ReAct) that answers fleet questions in plain language — no SQL. Governed text-to-SQL (allow/deny-list **+** read-only DB, defense-in-depth), GPS anomaly detection, and RAG (ChromaDB). Dual-provider: Gemini (cloud, active-probe fallback) and Ollama (fully local). Authenticated FastAPI, hardware-aware model selection, first `pytest` suite (36 tests on the SQL guardrail). | LangGraph · FastAPI · ChromaDB · DuckDB · Gemini/Ollama |
| 📄 **Job-Tailored Resume Builder** *(personal product)* | React 18 SPA that generates per-job résumé variants from a modular, tag-based content bank, with **LLM-assisted adaptation** (structured-JSON extraction) and multi-format export (PDF / Word / Markdown). | React 18 · LLM · localStorage |
| 🧠 **Fleet ML — Fuel Anomaly Detection** | LightGBM (Tweedie/Huber) with leakage-free temporal validation (**MAE ~2.5 L/day · MAPE ~12.5%**), ranking vehicle-days by recoverable cost. Feature store of **17.6M GPS points → 43k trips**, engineered 100% in SQL/DuckDB. *(A self-supervised TCN encoder is designed/documented as a next phase.)* | LightGBM · DuckDB · pandas |
| 🗺️ **Collection Coverage Heatmaps** | Interactive geospatial coverage analyzer with a **4-state per-segment model** (collected / possible-manual / GPS-failure / missed) over a projected CRS, plus AES-256-GCM client-side encryption and signed PDF reports. | GeoPandas · Leaflet.js · reportlab |
| 🔁 **Route Optimizer (TSP)** | 8-stage pipeline for collection-route optimization: morphological clustering + **multi-seed 2-opt / or-opt** TSP + shortest-path routing over OpenStreetMap graphs; temporal route registry (**SCD-2**) in DuckDB. | NetworkX · GeoPandas · DuckDB |
| 📡 **Fleet Telematics Pipeline** | Production pipeline ingesting **100K+ GPS records/day** via REST API (OAuth2), with a **dual thread/process concurrency model** (hardware-aware) and a multi-layer DuckDB/Parquet store with incremental fetching. | DuckDB · Parquet · OAuth2 |
| 🛠️ **RPA Write-Back Automation** | Selenium automation over a fleet portal that goes **beyond scraping**: detects data-entry errors, derives ground truth from GPS, and **writes corrections back** into the system (declarative edit plan + dry-run). Shipped as a standalone `.exe`. | Selenium · Python · PyInstaller |
| ⏱️ **Real-Time Overtime Alerting** | Daemon that ingests workforce timekeeping into DuckDB (**idempotent, hash-ledgered**), re-derives clock punches from messy positional data, and emits end-of-shift alerts for unclosed overtime — with anti-spam state. | Python · DuckDB |
| 🔀 **Database Sync Engine** | Standalone tool that **diffs 87M+ rows in ~75s** via a single DuckDB `FULL OUTER JOIN` with conditional aggregation, then merges additively by business key. | DuckDB · SQLite · PyInstaller |
| 🗣️ **Meeting Minutes Generator** | Hybrid local-NLP + LLM pipeline turning raw transcripts into structured minutes (DOCX) — speaker diarization and deterministic data extraction before the LLM cuts tokens. | NLP · LLM · python-docx |

---

## GitHub Stats

<!--
  ⚠️ Estes cards leem só dados PÚBLICOS. Como a maior parte da atividade do Jorge é
  em repos privados, para refletir o real: (1) GitHub → Settings → Profile →
  "Include private contributions on my profile"; (2) self-host do github-readme-stats
  no Vercel com um PAT próprio (count_private=true). Ver memória [[user_github_private_repos]].
-->

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=JorgeEd13&theme=tokyonight" width="100%"/>

</div>

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=JorgeEd13&theme=tokyonight" height="160em"/>
&nbsp;
<img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=JorgeEd13&theme=tokyonight" height="160em"/>
&nbsp;
<img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=JorgeEd13&theme=tokyonight" height="160em"/>

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
