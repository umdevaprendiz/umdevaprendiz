<p align="center">
  <img src="name-animado.svg" alt="Sérgio Guilherme" width="100%" style="max-width:700px;" />
</p>

<h3 align="center">AI / LLM Engineer · LLMOps &amp; Data · Software Engineer (Java &amp; Spring Boot) · Computer Science Student (UFPB)</h3>

<p align="center">
  <img src="https://skillicons.dev/icons?i=py,azure,postgres,mysql,java,spring,react,vite,ts,js" /><br>
  <img src="https://skillicons.dev/icons?i=html,css,git,githubactions,docker,maven,postman" /><img src="icons/databricks.svg" alt="Databricks" height="48" /><img src="icons/insomnia.svg" alt="Insomnia" height="48" />
</p>

<p align="center">
  <sub>
    <img src="https://cdn.simpleicons.org/gmail/EA4335" width="14" height="14" valign="middle"/> <a href="mailto:sergiodeveloperprofissional27@gmail.com">sergiodeveloperprofissional27@gmail.com</a> ·
    <img src="https://cdn.simpleicons.org/github/9e9e9e" width="14" height="14" valign="middle"/> <a href="https://github.com/umdevaprendiz">github.com/umdevaprendiz</a> ·
    <img src="https://appstudying.onrender.com/favicon.svg" width="14" height="14" valign="middle"/> <a href="https://appstudying.onrender.com">appstudying.onrender.com</a>
  </sub>
</p>

---

### About me

AI/LLM engineering intern focused on LLMOps and data: administering and maintaining production AI agents built with LangChain and LangGraph on Databricks and Azure, creating quality benchmarks (latency, cost per call/tokens, accuracy rate), implementing new AI use cases, and tracking experiments with MLflow.

Outside of work, I build my own AI and data projects end to end — from a local RAG assistant for medicine leaflets to a deterministic legal-sentencing engine and a full ML pipeline for churn prediction — always with the same principle: LLMs read and write, but anything that has to be correct is deterministic, testable, and auditable code, and "I didn't find it" beats an invented answer.

This is backed by a solid software engineering foundation: as a Computer Science student at UFPB, I've built complete end-to-end Java/Spring Boot applications solo, with automated testing, Docker-based CI/CD, and security best practices by default.

Self-taught, metrics-driven, and comfortable collaborating with remote teams.

---

### Experience

**AI Analyst / AI Engineer — Intern**
`Python` `LangChain` `LangGraph` `MLflow` `pytest` `Databricks` `Azure`

- Create and run quality benchmarks for LLM agents: latency, cost per call (tokens), and accuracy rate of the generated answers.
- Administer and maintain production LLM agents built with LangChain and LangGraph, with structured debugging of Python pipelines and automated tests (pytest).
- Implement AI use cases on top of the existing agents, in the Databricks and Azure environment (including Azure ML Notebooks).
- Track experiments with MLflow (parameters, metrics, and artifacts) to compare runs.

---

### AI / LLM &amp; data projects

**[FarmaRAG](https://github.com/umdevaprendiz/farma-rag)** — a pharmacy-counter assistant over medicine leaflets, RAG with a local LLM 🟡 in progress
`Python` `LangGraph` `FastAPI` `PostgreSQL + pgvector` `Ollama` `bge-m3` `React + TypeScript` `Docker`

A chat assistant that answers questions about medicines from real leaflets (*bulas*), always with a verified source, and refuses when the leaflet doesn't support the answer. It runs entirely on a CPU-only machine: no paid API, no cloud.

- RAG pipeline: PDF → sections → chunks → bge-m3 embeddings (cached) → vector search in PostgreSQL + pgvector, checked against a numpy implementation. 21 real leaflets (906 chunks) plus an ANVISA catalog of 6,999 name/active-ingredient pairs to detect the medicine before calling the LLM.
- LangGraph agent with 6 nodes and routing decided in code. Structured output (JSON Schema) lets the model cite only the chunks it received; citations, grounding of numbers/doses, and answer relevance are validated, with up to 3 adaptive rounds under a time budget. No unverified answer leaves the graph.
- Conversation: follow-up questions with context ("and for children?"), clarification questions, an allergy flow that suggests same-class alternatives, and answers copied verbatim from the leaflet where precision matters (doses, interactions).
- FastAPI (5 endpoints, history of every query with latency and each attempt), React + TypeScript chat UI, 246 automated tests, and latency measured on CPU (~50 tokens/s reading, ~9 tokens/s generating).

**[Juris.IA](https://github.com/umdevaprendiz/Juris.IA)** — explainable, deterministic AI for criminal sentencing (*dosimetria penal*) 🟢 in production
`Python` `FastAPI` `Docker` `GitHub Actions` `Playwright` `Jupyter` `LLM-based fact extraction (planned)`

A system that reads a criminal case description in Portuguese, identifies the crime, and works out the sentencing range under Brazil's three-phase method (art. 68 of the Penal Code), citing the legal provision behind every number. Nothing is guessed: every number is deterministic math, and every suggestion cites an indexed article.

- Sentencing engine in pure Python: exact fraction arithmetic (no floats), configurable policies (Strategy pattern), a step-by-step audit trail, and legal safeguards modeled as code (STJ Súmula 231, art. 68).
- Crime-identification agent: BM25 plus hand-written legal indicators over 5,271 indexed articles and 316 offense types; every suggestion cites the article and the case phrase behind it, and the user confirms before the engine calculates. Personal data is anonymized before anything is stored.
- Validated with 130 case descriptions (the right crime ranked first in all of them), a 46-question search benchmark (89.1% top-1, 100% top-5), and 17 hand-computed sentencing cases. CI runs API and browser (Playwright) tests and deploys only if they pass.

**[churn-prediction-ml](https://github.com/umdevaprendiz/churn-prediction-ml)** — customer churn prediction system
`Python` `pandas` `scikit-learn` `FastAPI` `pytest` `Jupyter` `Power BI`

- End-to-end ML pipeline: data cleaning, feature engineering, and a leakage-safe preprocessing pipeline; Logistic Regression vs. Random Forest, reaching a 0.80 ROC-AUC (0.804 vs. 0.781).
- REST API in FastAPI for single and batch predictions, with a pytest suite; Power BI dashboard with real-vs-predicted churn and customer segmentation; exploratory analysis in Jupyter.

---

### Software engineering projects

**[AppStudying](https://github.com/umdevaprendiz/AppStudying)** — a study platform with a social network for students (`Spring Boot` `React` `MySQL` `Docker` `WebSocket`) — [live](https://appstudying.onrender.com). Full-stack app built and deployed solo: study-session tracking, study partnerships, study groups with live presence, real-time chat, and an interface in English, Portuguese, and Spanish. Email verification, database-backed sessions, per-resource authorization, and rate limiting, with 159 automated tests and a CI/Docker pipeline running Flyway migrations.

**[API Bank](https://github.com/umdevaprendiz/financialbank)** — a banking system with a financial dashboard (`Spring Boot` `Spring Security` `React + TypeScript` `MySQL` `Docker`). RESTful API with role-based access control (admin, manager, user), atomic transfers between accounts, dynamic query filters, and an admin metrics dashboard; deployed on Railway.

---

### Education &amp; languages

Computer Science — UFPB *(expected graduation: 2030)* · Networking Technician — ETEMERB
Portuguese (native) · English (B2) · Spanish (basic/intermediate)
