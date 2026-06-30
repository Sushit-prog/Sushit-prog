<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=0A0F08&height=120&section=header&text=&fontColor=8AFF57" width="100%"/>

<h1>SUSHIT LAL PAKRASHY</h1>

<code>AI Systems Engineer — Infrastructure & Tooling for LLM-Based Systems</code>

<br/>

<img src="https://img.shields.io/badge/status-building-8AFF57?style=for-the-badge&logo=terminal&logoColor=0A0F08&labelColor=0A0F08"/>
<img src="https://img.shields.io/badge/focus-AI%20infrastructure-CAFF3C?style=for-the-badge&logo=opensourceinitiative&logoColor=0A0F08&labelColor=0A0F08"/>
<img src="https://img.shields.io/badge/location-West%20Bengal,%20India-8AFF57?style=for-the-badge&logo=googlemaps&logoColor=0A0F08&labelColor=0A0F08"/>

</div>

<br/>

```bash
$ whoami
```

I don't build AI apps. I build the systems that make AI apps trustworthy enough to ship.

Most LLM projects fail quietly — outputs drift, agents loop without explanation, and "it works on my machine" means nothing when the model is non-deterministic. My work sits underneath that layer: **evaluation frameworks, replay/debugging tooling, observability platforms, and retrieval infrastructure** that give AI systems the same engineering guarantees we expect from traditional software — testability, traceability, and reproducibility.

If you trace my projects back, they all answer one question: *how do you know your AI system is actually working?*

```bash
$ cat current_role.txt
```

**AI/ML Engineer Intern** @ iNeuBytes — production-oriented AI/ML work, applied modeling, and systems engineering practice.

Previously: Data Science Intern @ Thiranex (predictive modeling, applied ML workflows) · BCG GenAI Job Simulation (GenAI solution design for business problems).

Currently pursuing a B.Tech in Electronics & Communication Engineering at Guru Nanak Institute of Technology.

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=24&duration=3000&pause=1500&color=8AFF57&center=false&vCenter=true&width=300&height=40&lines=%E2%96%B8+stack" />

<table>
<tr>
<td valign="top" width="50%">

**Languages**
<br/>
`Python`

**AI / ML Systems**
<br/>
`LangChain` `LangGraph` `RAG` `LLM Evaluation` `Semantic Assertions` `AI Agents` `Prompt Engineering` `HuggingFace` `Groq` `OpenRouter`

</td>
<td valign="top" width="50%">

**Backend & Data**
<br/>
`FastAPI` `Streamlit` `Neo4j` `ChromaDB` `SQLite`

**Tooling**
<br/>
`Git` `GitHub` `pytest` `VS Code` `OpenCode` `Mimocode`

</td>
</tr>
</table>

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=24&duration=3000&pause=1500&color=8AFF57&center=false&vCenter=true&width=480&height=40&lines=%E2%96%B8+infrastructure+%26+tooling" />

*Projects built to make AI systems testable, debuggable, and observable — the layer most AI engineers skip.*

<br/>

**[pytest-llm-sushit](https://github.com/Sushit-prog/pytest-llm)** — `PyPI package`

LLM outputs can't be tested with `assert output == "expected"`. This is a pytest plugin that replaces brittle string-matching with semantic, LLM-judged assertions across multiple model providers. It exists because most AI projects ship with no real test coverage — this gives them one.

`Multi-provider LLM-as-a-Judge` `Semantic assertions` `Published on PyPI`

<br/>

**[langgraph-replay](https://github.com/Sushit-prog/langgraph-replay)**

When a LangGraph agent fails, the failure is usually buried three nodes deep in a trace you can't replay. This is a callback-based recorder for LangGraph applications — it logs execution to SQLite, replays runs deterministically, and includes a blame engine that auto-diagnoses which node and which decision caused a failure, surfaced through a terminal debugger and CLI. It's designed to integrate directly with `pytest-llm-sushit`, so failed semantic assertions can be traced back to the exact agent step that caused them.

`Execution replay` `Blame engine` `Auto-diagnosis` `TUI debugger`

<br/>

**[AgentTrace](https://github.com/Sushit-prog) `· early stage`**

`langgraph-replay` solves replay for a single agent graph. AgentTrace extends the same idea to multi-agent systems — an observability platform for tracing execution, debugging inter-agent behavior, and analyzing performance across agent fleets, not just single graphs.

`Trace visualization` `Multi-agent debugging` `LLMOps`

<br/>

**Vector Database (from scratch)** `· in progress`

Built in pure Python to understand retrieval systems at the level most RAG developers never go — rather than treating vector search as a library import. Phase 1 (flat index, cosine + Euclidean similarity) is complete with full test coverage; HNSW is the next milestone, approached by working through the algorithm deeply before implementing it.

`Flat index` `Cosine / Euclidean similarity` `HNSW (in progress)` `Full test coverage`

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=24&duration=3000&pause=1500&color=8AFF57&center=false&vCenter=true&width=350&height=40&lines=%E2%96%B8+applied+systems" />

*Where the infrastructure above gets put to work.*

<br/>

**[SENTINEL](https://github.com/Sushit-prog/SENTINEL)** — *ET AI Hackathon* · `Phase 5`

A Digital Public Safety Intelligence Platform covering scam detection, currency authentication, and fraud network mapping through relationship analysis. Built as a multi-agent system on LangGraph, with Neo4j for network/relationship mapping, ChromaDB for retrieval, Groq for inference, and FastAPI serving the platform. Currently in active polish toward demo readiness.

`LangGraph` `FastAPI` `Groq` `Neo4j` `ChromaDB`

<br/>

**[Applyt](https://github.com/Sushit-prog/Applyt)**

An AI-powered career toolkit — resume scoring and matching, cover letter generation, and a career-coaching chatbot, built on LangChain and OpenRouter with a Streamlit frontend.

**[ARXIS](https://github.com/Sushit-prog/ARXIS-)**

A multi-agent research pipeline exploring automated literature and research workflows using LangGraph and LangChain agents.

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=24&duration=3000&pause=1500&color=8AFF57&center=false&vCenter=true&width=320&height=40&lines=%E2%96%B8+open+source" />

* Two **merged pull requests** in the `marimo` project.
* Active `marimo` PR `#9302` — fixes a reactive error-handling bug in the code-mode execution path; passed all CI checks, awaiting maintainer review.
* Bounty contribution to `Onyx` implementing a **Jira Service Management connector**; automated review scored it 5/5 confidence.
* Contribution strategy targets impactful, lower-competition issues in active repos rather than racing for newly opened ones — sustained involvement over one-off PRs.

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=24&duration=3000&pause=1500&color=8AFF57&center=false&vCenter=true&width=480&height=40&lines=%E2%96%B8+engineering+constraints" />

Everything above is designed, built, and tested on a 12th Gen Intel i5, 8GB RAM, no dedicated GPU. No fine-tuning, no local large-model inference, no luxury of "just add more compute." That constraint forces resource-aware architecture, efficient algorithms, and API-first design over local heavy lifting — a discipline that tends to produce more deployable systems, not less capable ones.

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=24&duration=3000&pause=1500&color=8AFF57&center=false&vCenter=true&width=280&height=40&lines=%E2%96%B8+workflow" />

```
research the problem  →  design the architecture  →  break into milestones
        ↓
AI-assisted implementation (OpenCode / Mimocode)  →  review & refine
        ↓
tests + docs + polish  →  iterate until production-ready
```

AI assistants accelerate implementation. Architecture, system design, and correctness are mine.

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=24&duration=3000&pause=1500&color=8AFF57&center=false&vCenter=true&width=400&height=40&lines=%E2%96%B8+currently+learning" />

`LangGraph` → `Model Context Protocol (MCP)` → `LLMOps` → `Production AI Infrastructure` → `Multi-Agent Systems` → `AI Observability` → `Distributed AI Systems`

Depth in AI engineering fundamentals, deliberately over breadth.

<br/>


<h2>▸ activity</h2>

<p align="center">
  <img
    src="https://github-readme-activity-graph.vercel.app/graph?username=Sushit-prog&bg_color=0A0F08&color=E8F5E1&line=8AFF57&point=CAFF3C&area=true&area_color=1A2B1A&hide_border=true"
    width="100%"
    alt="GitHub Activity Graph"
  />
</p>

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=24&duration=3000&pause=1500&color=8AFF57&center=false&vCenter=true&width=280&height=40&lines=%E2%96%B8+open+to" />

`AI Engineering Internships` · `AI / ML Engineer roles` · `LLM Infrastructure Engineering` · `Developer Tooling` · `Open Source Collaboration` · `Freelance AI Development`

<br/>

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Sushit-prog&show_icons=true&bg_color=0A0F08&title_color=8AFF57&icon_color=CAFF3C&text_color=E8F5E1&border_color=1A2B1A&hide_border=false" width="48%"/>
<img src="https://github-readme-streak-stats.herokuapp.com/?user=Sushit-prog&background=0A0F08&stroke=1A2B1A&ring=8AFF57&fire=CAFF3C&currStreakLabel=8AFF57&sideLabels=E8F5E1&dates=E8F5E1&currStreakNum=E8F5E1&sideNums=E8F5E1" width="48%"/>

<br/><br/>

<a href="mailto:pakrashys@gmail.com"><img src="https://img.shields.io/badge/email-pakrashys@gmail.com-8AFF57?style=for-the-badge&logo=gmail&logoColor=0A0F08&labelColor=0A0F08"/></a>
<a href="https://www.linkedin.com/in/sushit-lal-pakrashy-590a1130b"><img src="https://img.shields.io/badge/linkedin-connect-CAFF3C?style=for-the-badge&logo=linkedin&logoColor=0A0F08&labelColor=0A0F08"/></a>

<br/><br/>

<sub>I build reliable AI infrastructure, developer tools, and open-source software that improve how AI systems are engineered.</sub>

</div>
