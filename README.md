<h1 align="center">Hi, I'm Rangarajan 👋</h1>

<p align="center">
  <b>I build AI agents and the tooling that keeps them safe and measurable.</b><br>
  MCP · tool-use guardrails · agent evaluation · open source
</p>

<p align="center">
  <a href="https://linkedin.com/in/rangarajan19"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <img src="https://img.shields.io/badge/Based%20in-India-orange" alt="India">
</p>

---

## 🚀 What I'm building

### [agentkit-mcp](https://github.com/rangarajan19/agentkit-mcp)
A small **MCP-first agent framework** where every tool comes from an MCP server, with
**guardrails at the tool layer**: dry-run, human approval, argument rules and tool allow-lists.

- Own agent loop with tracing and a step limit; tool errors go back to the model so it can recover
- Works with **Gemini** and **free OpenRouter models**, with automatic retry and model fallback
- Ships two example agents: **issue triage** (GitHub MCP server plus its own MCP server) and a **web research agent**
- Tested with 47 automated tests running in CI, and honest about what is and isn't verified in its README

### [agentic-api-testing](https://github.com/rangarajan19/agentic-api-testing)
Chat-driven API testing: a local LLM agent (**LangGraph + Ollama**) routes requests, while
**deterministic pytest checks** do the actual testing, so the LLM steers and the assertions stay reliable.

---

## 🤝 Open-source contributions

| Project | Merged contribution |
|---|---|
| [HelpCode-ai/anythingmcp](https://github.com/HelpCode-ai/anythingmcp) | [#698](https://github.com/HelpCode-ai/anythingmcp/pull/698): added an `adapter:new` scaffolder so new connector adapters start from a template (closes #585) |
| [agentevals-dev/agentevals](https://github.com/agentevals-dev/agentevals) | [#224](https://github.com/agentevals-dev/agentevals/pull/224): CI fix so autofixable ruff violations fail the build instead of passing silently |

---

## 🧰 Tools I work with

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C)
![Ollama](https://img.shields.io/badge/Ollama-000000)
![Gemini](https://img.shields.io/badge/Gemini_API-4285F4?logo=googlegemini&logoColor=white)
![OpenRouter](https://img.shields.io/badge/OpenRouter-6467F2)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?logo=pytest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=githubactions&logoColor=white)

## 🔎 Currently exploring
- Measuring agent accuracy across models, not just demoing them
- Agent safety: prompt injection and tool permissions
- Fixing bugs and improving tooling in projects I use

---

<p align="center">Feedback and collaboration welcome, reach me on <a href="https://linkedin.com/in/rangarajan19">LinkedIn</a>.</p>
