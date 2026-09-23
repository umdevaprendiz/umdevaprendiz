<p align="center">
  <img src="name-animado.svg" alt="Sérgio Guilherme" width="100%" style="max-width:700px;" />
</p>

<h3 align="center">AI / LLM Engineer · LLMOps &amp; Data · Software Engineer (Java &amp; Spring Boot) · Computer Science Student (UFPB)</h3>

<p align="center">
  <img src="https://skillicons.dev/icons?i=py,azure,postgres,mysql,java,spring,react,vite,ts,js,html,css,git,githubactions,docker,maven,postman" />
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

AI/LLM Engineer focused on LLMOps and data: administering and maintaining production AI systems built with LangChain and LangGraph, structured debugging of Python pipelines, quality benchmarking (latency, cost per call/tokens, LLM accuracy rate), and experiment tracking with MLflow.

Outside of client work, I build my own AI and data projects end to end — from a deterministic legal-sentencing engine to a full ML pipeline for churn prediction — always with the same principle: LLMs read and write, but never do the math or invent facts. Anything that has to be correct is deterministic, testable, and auditable code.

This is backed by a solid software engineering foundation: as a Computer Science student at UFPB, I've built complete end-to-end Java/Spring Boot applications solo, with automated testing, Docker-based CI/CD, and security best practices by default.

Self-taught, metrics-driven, and comfortable collaborating with remote teams.

---

### Experience

**AI Analyst / AI Engineer (Independent Contractor)** — Independent Consulting
`Python` `LangChain` `LangGraph` `MLflow` `pytest`

- Responsible for the administration and maintenance of production AI systems built with LangChain and LangGraph.
- Structured debugging of Python-based AI pipelines, identifying and fixing failures with the support of automated tests (pytest).
- Quality benchmarking of AI systems — latency, cost per call (tokens), and the accuracy rate of LLM-generated responses.
- Experiment tracking with MLflow: logging parameters, metrics, and run artifacts.
- Development, testing, and documentation of solutions using Python notebooks (Jupyter / Azure ML Notebooks).

---

### AI / LLM &amp; data projects

**[ia-judge](https://github.com/umdevaprendiz/ia-judge)** — explainable AI for criminal sentencing (*dosimetria penal*) 🚧 in progress
`Python` `LangChain` (planned) `PostgreSQL + pgvector` (planned) `Azure OpenAI` (planned) `Jupyter`

An AI-assisted system that reads a criminal case description and works out the sentencing range under Brazil's three-phase sentencing method (art. 68 of the Penal Code), citing the real legal provisions behind every number. The core design principle: **LLMs interpret and explain, they never calculate** — a language model reading legal text and inventing numbers or citations is exactly the failure mode this architecture is built to avoid.

- Deterministic sentencing engine (all 3 phases) built as pure, dependency-free Python: immutable value objects, exact fraction arithmetic (no floats — a rounding bug here is a real sentence being wrong), a Strategy pattern for configurable sentencing policies, and a full step-by-step audit trail for every calculation.
- Built-in legal safeguards as code: sentences never drop below the statutory minimum via mitigating factors (STJ Súmula 231), and the "apply only the largest aggravating/mitigating factor" rule (CP art. 68, sole paragraph) is modeled explicitly rather than left to a prompt.
- Validated against real judgments in a Jupyter notebook, phase by phase.
- Planned next: LLM-based fact extraction with mandatory evidence citations for every extracted fact, RAG-grounded legal reasoning over the indexed Penal Code (PostgreSQL + pgvector), and a benchmark against real court decisions.

**[churn-prediction-ml](https://github.com/umdevaprendiz/churn-prediction-ml)** — customer churn prediction system
`Python` `pandas` `scikit-learn` `FastAPI` `pytest` `Jupyter` `Power BI`

- End-to-end ML pipeline to predict customer churn: data cleaning, feature engineering, and model comparison (Logistic Regression vs. Random Forest), reaching a 0.80 ROC-AUC.
- REST API in FastAPI for single predictions and batch report generation, with an automated pytest suite.
- Power BI dashboard with real-vs-predicted churn rate and segmentation by customer profile.
- Exploratory data analysis (Jupyter, pandas, seaborn) to identify the main churn risk factors.

---

### Software engineering projects

**[AppStudying](https://github.com/umdevaprendiz/AppStudying)** — a study platform with a social network for students (`Spring Boot` `React` `MySQL` `Docker` `WebSocket`) — [live](https://appstudying.onrender.com). Full-stack app built and deployed solo: session tracking, study partnerships, and real-time chat, with a real production pipeline (Docker, CI, automated tests).

**[API Bank](https://github.com/umdevaprendiz/financialbank)** — a banking system with a financial dashboard (`Spring Boot` `Spring Security` `React + TypeScript` `MySQL`). RESTful API with role-based authorization, dynamic query filters, and an admin metrics dashboard.

---

### Education &amp; languages

Computer Science — UFPB *(expected graduation: 2030)* · Networking Technician — ETEMERB
Portuguese (native) · English (B2) · Spanish (basic/intermediate)
