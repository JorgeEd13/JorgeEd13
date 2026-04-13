<div align="center">

# Jorge Edson
### Data Engineer · AI Engineer · GIS & Optimization

*Building end-to-end AI solutions — from raw GPS traces to conversational agents, from pipeline engineering to actionable insights.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jorgeedjson/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jorge.ed.ribeiro00@gmail.com)
[![GitHub followers](https://img.shields.io/github/followers/JorgeEd13?style=for-the-badge&logo=github&logoColor=white&color=181717)](https://github.com/JorgeEd13)

</div>

---

## About me

I'm a Data Engineer and AI Engineer based in Pernambuco, Brazil, building end-to-end solutions that go from raw data ingestion all the way to production AI products.

My most recent project is a **conversational AI agent** (LangGraph ReAct) that lets non-technical users query a real fleet database in plain Portuguese — no SQL required. It combines a production data pipeline, GPS anomaly detection, and semantic search (RAG) into a single REST API. Supports both Google Gemini and fully local Ollama models.

Day-to-day I also process **100K+ GPS records/day**, optimize waste collection routes across **12+ municipalities**, and build tools that non-technical users can actually use.

- Currently building **AI agents and RAG systems** applied to real operational problems
- Experienced in **fleet telematics, route optimization, and geospatial analytics**
- Exploring **ML in logistics**: anomaly detection, predictive maintenance, demand forecasting
- Background in **frontend development** (JS, HTML, CSS) — helps me think about usability when building data products

---

## Tech Stack

### AI & LLMs
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=chainlink&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google%20Gemini-4285F4?style=flat-square&logo=google&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)

### Data Science & Analytics
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

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
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)

---

## Featured Projects

| Project | Description | Stack |
|---|---|---|
| **🤖 Fleet Intelligence Agent** | Conversational AI agent that answers fleet questions in plain Portuguese — no SQL. LangGraph ReAct loop queries a real GPS database (DuckDB), detects 7 types of GPS anomalies, and searches historical patterns via RAG (ChromaDB). Dual-provider: Google Gemini (cloud, automatic model fallback) and Ollama (fully local, offline). Authenticated REST API with hardware-aware model selection. | LangGraph · FastAPI · ChromaDB · DuckDB · Gemini · Ollama |
| **🗺️ Heatmap Route Analyzer** | Interactive geospatial heatmaps for waste collection monitoring across 12+ municipalities. Includes AES-256-GCM encryption and signed PDF reports. | GeoPandas · Leaflet.js · Parquet |
| **🔁 Route Optimizer (TSP)** | 8-stage pipeline for waste collection route optimization using TSP with morphological clustering and NetworkX graph routing over OpenStreetMap. | NetworkX · GeoPandas · OpenStreetMap |
| **📡 Fleet Telematics Pipeline** | Production data pipeline ingesting 100K+ GPS records/day via REST API (OAuth2). Multi-layer cache (DuckDB + SQLite + Parquet) with incremental fetching. | DuckDB · Parquet · OAuth2 |
| **🗣️ Meeting Minutes Generator** | NLP tool converting raw meeting transcriptions into structured minutes using LLMs (Gemini & Ollama). Packaged as standalone `.exe`. | LLM · python-docx · PyInstaller |
| **🌐 Web Automation — Inlog** | Selenium-based scraper for fleet management platform with GUI and multi-format export, distributed as `.exe` for non-technical users. | Selenium · Tkinter · PyInstaller |

---

## GitHub Stats

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
