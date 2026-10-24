<p align="center">
  <img src="assets/header.svg" alt="Rangarajan G — agentic AI engineer. An agent trace: plan, tool call, retrieval, a guardrail blocking a disallowed write, and a passing validation." width="100%">
</p>

<p align="center">
  <a href="https://rangarajan19.github.io/portfolio/"><img src="https://img.shields.io/badge/portfolio-rangarajan19.github.io-F2A63B?style=flat-square&labelColor=1A232A&logo=githubpages&logoColor=F2A63B" alt="Portfolio"></a>
  <a href="https://linkedin.com/in/rangarajan19"><img src="https://img.shields.io/badge/linkedin-rangarajan19-F2A63B?style=flat-square&labelColor=1A232A&logo=linkedin&logoColor=F2A63B" alt="LinkedIn"></a>
  <img src="https://img.shields.io/badge/chennai-india-78878F?style=flat-square&labelColor=1A232A" alt="Chennai, India">
</p>

<img src="assets/divider.svg" width="100%" alt="">

## About

Agentic AI engineer working on **LLM orchestration, MCP tooling and AI-driven test automation**.
By day I build MCP tools and multi-agent pipelines for enterprise PLM workflows — Google ADK, Jira MCP,
Playwright and Gemini self-healing tests. In my own time I build open-source agent tooling with one rule:
**the LLM steers, deterministic code and guardrails decide.**

That rule is the whole architecture. The model proposes; a tool layer checks the proposal against an
allow-list, dry-runs it or asks for approval; blocked calls come back as errors the model can recover from
rather than silent failures.

<img src="assets/guardrail.svg" width="100%" alt="The LLM proposes a tool call; a guardrail layer checks it against an allow-list with dry-run and approval; allowed calls reach the MCP tool, and blocked calls return an error the model can recover from.">

<img src="assets/divider.svg" width="100%" alt="">

## Featured projects

<table>
<tr>
<td width="50%" valign="top">

### [agentkit-mcp](https://github.com/rangarajan19/agentkit-mcp)
![Python](https://img.shields.io/badge/Python-1A232A?style=flat-square&logo=python&logoColor=F2A63B)
![MCP](https://img.shields.io/badge/MCP-1A232A?style=flat-square)
![tests](https://github.com/rangarajan19/agentkit-mcp/actions/workflows/tests.yml/badge.svg)

MCP-first agent framework with **guardrails at the tool layer**: dry-run, human approval, argument rules and allow-lists.

- Own agent loop with tracing and a step limit
- Gemini and free OpenRouter models, with retry and fallback
- Issue-triage and web-research example agents
- 47 automated tests in CI; the README states what is *not* verified yet

</td>
<td width="50%" valign="top">

### [agentic-api-testing](https://github.com/rangarajan19/agentic-api-testing)
![Python](https://img.shields.io/badge/Python-1A232A?style=flat-square&logo=python&logoColor=F2A63B)
![LangGraph](https://img.shields.io/badge/LangGraph-1A232A?style=flat-square)
![MIT](https://img.shields.io/badge/license-MIT-1A232A?style=flat-square)

Chat-driven API testing: a local LLM (**LangGraph + Ollama**) routes requests, **deterministic pytest checks** do the testing.

- "Run negative tests for payments", "create defects for the failures"
- The model can never invent a pass
- FastAPI backend, Streamlit UI, Docker Compose
- Runs on a 4 GB GPU with `llama3.2:3b`

</td>
</tr>
</table>

<img src="assets/divider.svg" width="100%" alt="">

## A year of commits, eaten

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/rangarajan19/rangarajan19/output/snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/rangarajan19/rangarajan19/output/snake-light.svg">
  <img src="https://raw.githubusercontent.com/rangarajan19/rangarajan19/output/snake-dark.svg" width="100%" alt="A snake moving across my GitHub contribution graph, eating each day's commits.">
</picture>

<img src="assets/divider.svg" width="100%" alt="">

## Open-source contributions

Nine merged pull requests across three projects I use.

| Project | Merged |
|---|---|
| [HelpCode-ai/anythingmcp](https://github.com/HelpCode-ai/anythingmcp) | [#1193](https://github.com/HelpCode-ai/anythingmcp/pull/1193) — warn instead of failing hard when `METRICS_TOKEN` is shorter than the shared 32-character secret minimum *(follow-up to #1131)* |
| [HelpCode-ai/anythingmcp](https://github.com/HelpCode-ai/anythingmcp) | [#1131](https://github.com/HelpCode-ai/anythingmcp/pull/1131) — opt-in Prometheus `/metrics` endpoint for tool calls *(closes [#1003](https://github.com/HelpCode-ai/anythingmcp/issues/1003))* |
| [HelpCode-ai/anythingmcp](https://github.com/HelpCode-ai/anythingmcp) | [#1057](https://github.com/HelpCode-ai/anythingmcp/pull/1057) — import a HAR capture as REST tools, stripping response bodies and cookies before upload *(closes [#1005](https://github.com/HelpCode-ai/anythingmcp/issues/1005))* |
| [HelpCode-ai/anythingmcp](https://github.com/HelpCode-ai/anythingmcp) | [#1019](https://github.com/HelpCode-ai/anythingmcp/pull/1019) — Connector Failure Alerts card in admin settings: configure, test and rotate the webhook secret *(closes [#1006](https://github.com/HelpCode-ai/anythingmcp/issues/1006))* |
| [HelpCode-ai/anythingmcp](https://github.com/HelpCode-ai/anythingmcp) | [#976](https://github.com/HelpCode-ai/anythingmcp/pull/976) — the backend behind those alerts: cooldown before dispatch, SSRF allow-list handling on Cloud *(closes [#1006](https://github.com/HelpCode-ai/anythingmcp/issues/1006))* |
| [HelpCode-ai/anythingmcp](https://github.com/HelpCode-ai/anythingmcp) | [#818](https://github.com/HelpCode-ai/anythingmcp/pull/818) — real multipart file uploads for connectors: fetch the URL server-side and attach an actual file part instead of stringifying it *(closes #645)* |
| [HelpCode-ai/anythingmcp](https://github.com/HelpCode-ai/anythingmcp) | [#698](https://github.com/HelpCode-ai/anythingmcp/pull/698) — `adapter:new` scaffolder so new connector adapters start from a template *(closes #585)* |
| [taskforcesh/bullmq](https://github.com/taskforcesh/bullmq) | [#4908](https://github.com/taskforcesh/bullmq/pull/4908) — annotate `job_id` and `Job.token` as `Optional[str]`, fixing implicit-Optional mismatches across the Python scheduler and lock methods *(closes [#4905](https://github.com/taskforcesh/bullmq/issues/4905), released in v3.3.3)* |
| [agentevals-dev/agentevals](https://github.com/agentevals-dev/agentevals) | [#224](https://github.com/agentevals-dev/agentevals/pull/224) — CI fix so autofixable ruff violations fail the build instead of passing silently |

<img src="assets/divider.svg" width="100%" alt="">

## What I build at work

AI automation engineer at Kripya Solution, on Centric PLM workflows for teams in the US and Europe.

- A **Google ADK multi-agent system** wired to Jira over MCP that turns stories into test cases on its own — 40% less manual design effort and 50% faster story-to-test-case turnaround across 30+ sprints.
- A **self-healing Playwright + Gemini framework** that recovers broken locators from DOM snapshots — 70% fewer flaky tests, and CI you can believe.
- A **CLI agentic PLM assistant** on LangGraph and Gemini: LLM-driven tool selection, RAG retrieval, code and config generation, multi-turn reasoning over a genuinely messy enterprise domain.
- **12+ reusable Claude prompt skills** covering BDD generation, validation logic and migration work.

<img src="assets/divider.svg" width="100%" alt="">

## Tech I work with

**Agents and LLMs**<br>
![MCP](https://img.shields.io/badge/MCP-1A232A?style=flat-square)
![LangGraph](https://img.shields.io/badge/LangGraph-1A232A?style=flat-square)
![Google ADK](https://img.shields.io/badge/Google_ADK-1A232A?style=flat-square&logo=google&logoColor=F2A63B)
![Gemini](https://img.shields.io/badge/Gemini-1A232A?style=flat-square&logo=googlegemini&logoColor=F2A63B)
![Claude](https://img.shields.io/badge/Claude_API-1A232A?style=flat-square&logo=anthropic&logoColor=F2A63B)
![Ollama](https://img.shields.io/badge/Ollama-1A232A?style=flat-square&logo=ollama&logoColor=F2A63B)
![OpenRouter](https://img.shields.io/badge/OpenRouter-1A232A?style=flat-square)

**Engineering and testing**<br>
![Python](https://img.shields.io/badge/Python-1A232A?style=flat-square&logo=python&logoColor=F2A63B)
![TypeScript](https://img.shields.io/badge/TypeScript-1A232A?style=flat-square&logo=typescript&logoColor=F2A63B)
![FastAPI](https://img.shields.io/badge/FastAPI-1A232A?style=flat-square&logo=fastapi&logoColor=F2A63B)
![Playwright](https://img.shields.io/badge/Playwright-1A232A?style=flat-square&logo=playwright&logoColor=F2A63B)
![pytest](https://img.shields.io/badge/pytest-1A232A?style=flat-square&logo=pytest&logoColor=F2A63B)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-1A232A?style=flat-square&logo=postgresql&logoColor=F2A63B)
![Docker](https://img.shields.io/badge/Docker-1A232A?style=flat-square&logo=docker&logoColor=F2A63B)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-1A232A?style=flat-square&logo=githubactions&logoColor=F2A63B)

<img src="assets/divider.svg" width="100%" alt="">

## Currently exploring

- Measuring agent accuracy across models, instead of demoing one happy path
- Agent safety: prompt injection, tool permissions, and what a blocked call should return
- Fixing bugs and improving tooling in the projects I actually use

<p align="center">
  <b>Feedback and collaboration welcome.</b> Reach me on <a href="https://linkedin.com/in/rangarajan19">LinkedIn</a>.
</p>

<img src="assets/footer.svg" width="100%" alt="">
