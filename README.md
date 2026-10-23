<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1000&color=6366F1&center=true&vCenter=true&width=700&lines=Hey%2C+I'm+Wesley+Reis+%F0%9F%91%8B;Software+Engineer+%C2%B7+AI+Engineering;LLM+Agents+%7C+MCP+%7C+Graph+RAG+%7C+Evals;TypeScript+%7C+Python+%7C+Java+%7C+Kotlin;From+backend+systems+to+AI+systems+%F0%9F%9A%80)](https://git.io/typing-svg)

<br/>

![Visitors](https://komarev.com/ghpvc/?username=wsqreis&color=6366f1&style=flat-square&label=Profile+Views)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/wesley-de-queiroz)

</div>

---

## 👨‍💻 About Me

I'm a full-stack engineer moving my backend experience into **AI engineering**: LLM agents, MCP servers and graph RAG, built with the same habits as any production system. Deterministic code makes the decisions, every claim is backed by an eval, and guardrails assume the model will get things wrong.

```kotlin
data class WesleyReis(
    val name     : String = "Wesley Reis",
    val role     : String = "Software Engineer · AI Engineering",
    val focus    : List<String> = listOf("LLM Agents", "MCP Servers", "Graph RAG", "Evals", "Backend"),

    val ai       : List<String> = listOf("LangGraph", "LangChain", "Spring AI", "MCP", "Neo4j / Cypher", "pgvector", "OpenRouter"),
    val practice : List<String> = listOf("Eval-driven prompts", "Retrieval evals", "Structured outputs", "Guardrails", "Agent memory"),
    val languages: List<String> = listOf("TypeScript", "Python", "Java 21", "Kotlin"),
    val backend  : List<String> = listOf("Node.js / Fastify", "Spring Boot 4", "FastAPI"),
    val frontend : List<String> = listOf("React 19", "Next.js"),
    val data     : List<String> = listOf("PostgreSQL", "Neo4j", "Redis", "SQLite", "Kafka"),
    val cloud    : List<String> = listOf("AWS", "Docker", "GitHub Actions"),

    val funFact  : String = "I turn ☕ into distributed systems"
)
```

---

## 🚀 Featured Projects

### 🟦 TypeScript · LangGraph · MCP

<table>
<tr>
<td width="50%" valign="top">

### 🏎️ [f1-graph-qa](https://github.com/wsqreis/f1-graph-qa)
Ask about **Formula 1 history in plain English**. A LangGraph agent writes Cypher over a Neo4j graph of every Grand Prix since 1950 (26k race results), fixes its own failed queries, and answers only from what the database returns.

- Self-correction on errors, guard rejections and empty results
- Read-only defence in depth: static guard + READ transactions
- Execution-accuracy eval against hand-written reference queries

![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

</td>
<td width="50%" valign="top">

### 🎬 [tmdb-mcp](https://github.com/wsqreis/tmdb-mcp)
An **MCP server for The Movie Database**, designed around how agents use tools: compact typed outputs, names instead of ids, and errors an agent can act on.

- Tool outputs up to 99% smaller than raw TMDB responses
- `discover` by genre and streaming service in one call
- Stdio and HTTP modes, with bearer auth and rate limiting

![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square&logo=anthropic&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Zod](https://img.shields.io/badge/Zod-3E67B1?style=flat-square&logo=zod&logoColor=white)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🧳 [travel-planner-agent](https://github.com/wsqreis/travel-planner-agent)
A travel assistant with **long-term memory the user controls**. It learns preferences from what the traveller says, never from its own suggestions, and keeps a change log.

- Memory extraction runs in parallel with the reply
- Structured `set`/`add`/`remove`/`clear` updates in SQLite
- `/memory`, `/history`, `/forget`; precision/recall eval

![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)

</td>
<td width="50%" valign="top">

### 🍝 [restaurant-booking-agent](https://github.com/wsqreis/restaurant-booking-agent)
A conversational **table-booking agent** where the LLM understands and phrases, and deterministic code decides availability.

- Multi-turn slot filling; side questions keep the booking
- Opening hours, table assignment and alternatives in code
- Intent and slot-extraction eval, in three languages

![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=flat-square&logo=fastify&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)

</td>
</tr>
</table>

### ☕ Java · Spring AI

<table>
<tr>
<td width="33%" valign="top">

### 🎫 [support-triage](https://github.com/wsqreis/support-triage)
**Event-driven ticket triage**: two Spring Boot services over Kafka. An LLM classifies tickets and drafts grounded replies; when the model is slow or down, keyword rules take over, and a human approves every reply.

- Transactional outbox, dead-letter topics, idempotent consumers
- Timeout and circuit breaker with a rules fallback
- Drafts only when retrieval, the model and citations agree

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apache-kafka&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/pgvector-316192?style=flat-square&logo=postgresql&logoColor=white)

</td>
<td width="33%" valign="top">

### 📚 [docs-assistant](https://github.com/wsqreis/docs-assistant)
Ask the **Spring Boot reference docs** and get streamed answers that cite the exact sections. The same index is an MCP server for coding agents.

- Vector, keyword and hybrid search in one PostgreSQL table
- A retrieval eval that overturned the hybrid-search default
- Semantic cache and an off-topic gate before any LLM call

![Spring AI](https://img.shields.io/badge/Spring_AI-6DB33F?style=flat-square&logo=spring&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/pgvector-316192?style=flat-square&logo=postgresql&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square&logo=anthropic&logoColor=white)

</td>
<td width="33%" valign="top">

### 🎧 [music-graph](https://github.com/wsqreis/music-graph)
**Explainable music recommendations** over a Last.fm listening graph, with a mood search tuned to each listener's taste.

- Similar artists, friends and tags as Cypher queries
- Explanations built from graph facts; the LLM only phrases them
- Holdout eval against a popularity baseline

![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)

</td>
</tr>
</table>

---

## 🧭 How I Build AI Systems

The same principles run through every project above:

| Principle | In practice |
|---|---|
| **The LLM understands, code decides** | The booking agent never decides availability; a rules engine does, and the reply may only use its result. |
| **No claim without an eval** | Each project ships an eval runner: execution accuracy for text-to-Cypher, intent and slot accuracy, memory precision and recall, retrieval hit rate, recommendation recall against a baseline. |
| **Assume the model will be wrong** | Read-only guards plus READ transactions for generated Cypher, retries fed with the actual error, and graceful failure when extraction breaks. |
| **The model will also be down** | A circuit breaker hands triage to keyword rules, explanations fall back to a template, and agents try the next model when a provider fails. |
| **Design tools for agents, not for APIs** | Compact outputs, human names instead of ids, and error messages that tell the agent how to fix its call. |
| **Users own their data** | Agent memory can be inspected, traced to when it was learned, and erased. |

---

## 🛠️ Tech Stack

### 🤖 AI Engineering
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Spring AI](https://img.shields.io/badge/Spring_AI-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![MCP](https://img.shields.io/badge/Model_Context_Protocol-000000?style=for-the-badge&logo=anthropic&logoColor=white)
![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?style=for-the-badge&logo=neo4j&logoColor=white)
![OpenRouter](https://img.shields.io/badge/OpenRouter-6467F2?style=for-the-badge&logoColor=white)
![Claude](https://img.shields.io/badge/Claude_Code-CC5500?style=for-the-badge&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_SDK-412991?style=for-the-badge&logo=openai&logoColor=white)

### 💻 Languages
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)

### ⚙️ Backend
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=for-the-badge&logo=fastify&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)

### 🖥️ Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)

### 🗄️ Data & Messaging
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Apache Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white)

### ☁️ Cloud, Infra & DevOps
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

---

## 📊 GitHub Stats

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=wsqreis&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=wsqreis&layout=compact&langs_count=8&theme=tokyonight&hide_border=true"/>

</div>

---

## 🔥 Contribution Streak

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=wsqreis&theme=tokyonight&hide_border=true&date_format=j%20M%5B%20Y%5D)](https://git.io/streak-stats)

</div>

---

<div align="center">

*"First, solve the problem. Then, write the code."* — John Johnson

⭐️ From [wsqreis](https://github.com/wsqreis)

</div>
