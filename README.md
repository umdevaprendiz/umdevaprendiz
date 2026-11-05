<p align="center">
  <img src="name-animado.svg" alt="Sérgio Guilherme" width="100%" style="max-width:700px;" />
</p>

<h3 align="center">Software Engineer · AI / LLM Engineer · LLMOps &amp; Data · Java &amp; Spring Boot · Computer Science Student (UFPB)</h3>

<p align="center">
  <img src="https://skillicons.dev/icons?i=py,azure,postgres,mysql,java,spring,react,vite,ts,js" /><br>
  <img src="https://skillicons.dev/icons?i=html,css,git,githubactions,docker,maven,postman" /><img src="databricks.svg" alt="Databricks" height="48" /><img src="insomnia.svg" alt="Insomnia" height="48" />
</p>

<p align="center">
  <sub>
    <img src="https://cdn.simpleicons.org/gmail/EA4335" width="14" height="14" valign="middle"/> <a href="mailto:sergiodeveloperprofissional27@gmail.com">sergiodeveloperprofissional27@gmail.com</a> ·
    <img src="https://cdn.simpleicons.org/github/9e9e9e" width="14" height="14" valign="middle"/> <a href="https://github.com/umdevaprendiz">github.com/umdevaprendiz</a>
  </sub>
</p>

---

### About me

AI/LLM engineering intern. My day-to-day is keeping production LLM agents (LangChain and LangGraph, on Databricks and Azure) reliable and measurable: I build the benchmarks that show whether an agent got faster, cheaper, or more accurate (latency, tokens per call, accuracy rate), debug the Python pipelines when it didn't, and implement new AI use cases on top of the existing agents, with every experiment tracked in MLflow.

Outside of work, I build AI systems where a wrong answer is costly, and I measure them instead of trusting them. The rule I follow: the LLM reads and writes, anything that must be correct is deterministic, tested code, and "I didn't find it" beats an invented answer. On the software side, I build Java/Spring Boot applications solo, from the schema to the tests and CI.

---

### Experience

**AI Analyst / AI Engineer — Intern**
`Python` `LangChain` `LangGraph` `MLflow` `Databricks` `Azure`

- Create and run quality benchmarks for LLM agents: latency, cost per call (tokens), and accuracy rate.
- Administer and maintain production agents built with LangChain and LangGraph, tracked with MLflow.
- Implement AI use cases on the existing agents in Databricks and Azure, tracking experiments with MLflow.
- AI training.
- Endpoint tests.

---

### AI / LLM &amp; data projects

**[FarmaRAG](https://github.com/umdevaprendiz/farma-rag)** — a chat assistant that answers questions about medicines from real package leaflets, always showing its source and refusing when the leaflet doesn't support an answer. It runs locally, with no paid API. 🟡 in progress
`Python` `LangGraph` `FastAPI` `PostgreSQL + pgvector` `Ollama` `React`

- A 6-node LangGraph agent in which code, not the model, validates citations, numbers, and doses.
- An 80-question benchmark of its own: reranking took the right passage into the first round from 44 to 57 of 70 questions. 435 automated tests.

**[DevOps Agent](https://github.com/umdevaprendiz/agents-DevOps)** — an AI agent that finds failures in containers, logs, and configuration, explains the cause, and proposes the fix as a git branch for you to review. It runs on a local model, so nothing leaves your network. 🟡 in progress
`Python` `Ollama` `Docker` `Git` `GitHub Actions`

- No shell tool, 28 deterministic security rules that work as a CI gate, and permission modes in which "no answer" means "no".
- Prompt-injection defense: logs and files are treated as data, and the code refuses any proposed fix that adds a medium or high security finding.
- An evaluation harness with simulated Docker that scores models on bugs with known causes. 650+ tests, CI on Python 3.10 to 3.13.

**[DataSentinel](https://github.com/umdevaprendiz/data-sentinel-agent)** — an agent that watches business metrics, detects anomalies, investigates the cause, and gives its own opinion. The model proposes and opines; code runs the queries, checks every number, and vetoes any cause it can't confirm. 🟡 in progress
`Python` `Ollama` `PostgreSQL + pgvector` `SQLite` `pytest` `GitHub Actions`

- Runs on synthetic data with the cause of each anomaly injected on purpose (20 scenarios), so there is an answer key to measure against.
- Done: anomaly detector, drill-down, number verifier (every figure in a report comes from a query the code ran) and incident memory on pgvector. Next: the LLM-driven investigator and the benchmark. 224 tests.

**[Code Archaeologist](https://github.com/umdevaprendiz/archaeologist-agent)** — a fully local agent, written in Java, that will find the riskiest parts of a legacy Java system by crossing Git history with code complexity, modernize them on separate branches, and prove with tests that behavior did not change. 🟠 early stage: the design, CLI, validated configuration, and CI are done; the agents are not implemented yet.
`Java 21` `Spring Boot 4` `picocli` `Maven` `GitHub Actions`

- Safety limits defined from the start: never touches the main branch, never edits the tests that protect the code, builds run in Docker with no network. 56 tests, CI on Linux, Windows and macOS.

**[Juris.IA](https://github.com/umdevaprendiz/Juris.IA)** — a tool for law students: describe a criminal case and the agent finds the crime and suggests circumstances, citing the article and the phrase from the case behind each one. The sentence itself is always calculated by deterministic code, step by step. The agent is rule-based (legal lexicon and BM25), with no LLM.
`Python` `FastAPI` `Docker` `GitHub Actions` `Playwright`

- 5,271 indexed articles and 316 offense types. Evaluated on 130 case descriptions, 46 search questions (89.1% right at first position), and 17 hand-computed sentencing cases.

**[churn-prediction-ml](https://github.com/umdevaprendiz/churn-prediction-ml)** — a model that predicts which customers are likely to cancel and turns it into decisions: tuned decision threshold, customer personas, what-if scenarios, and campaign ROI, with an API and a Power BI dashboard. Built on a synthetic dataset.
`Python` `pandas` `scikit-learn` `FastAPI` `Power BI`

- Three models compared (ROC-AUC 0.80); moving the decision threshold raised recall from 56% to 74%.

---

### Software engineering projects

**[AppStudying](https://github.com/umdevaprendiz/AppStudying)** — a study platform where students organize subjects, track study time, connect with study partners, join groups, and chat in real time. 159 automated tests and CI.
`Spring Boot` `React` `MySQL` `Docker` `WebSocket`

**[API Bank](https://github.com/umdevaprendiz/financialbank)** — a banking API with accounts, atomic transfers between them, role-based access with Spring Security, and an admin metrics dashboard.
`Spring Boot` `Spring Security` `React + TypeScript` `MySQL`

---

### Education &amp; languages

Computer Science — UFPB *(expected graduation: 2030)* · Networking Technician — ETEMERB
Portuguese (native) · English (B2) · Spanish (basic/intermediate)
