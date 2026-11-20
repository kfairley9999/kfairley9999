# Hi, I'm Kevin Fairley

Living in Los Angeles. I build AI agents, LLM tooling, and automation in **Python, TypeScript, and Rust**. I'm open to roles in agentic AI and LLM engineering.

Every project below ships with tests and CI. The web apps have live demos that open without an account, and any sample or simulated data is labeled as such on the page.

## Agentic AI and LLM tooling

| Project | What it is | Results |
| --- | --- | --- |
| [leadflow-mcp](https://github.com/kfairy9999/leadflow-mcp) · [live endpoint](https://leadflow-mcp.kfairley9999.workers.dev) | MCP server in TypeScript that lets Claude, Cursor, or any MCP client run a small shop's lead pipeline: 11 tools, 3 resources, 2 prompts. stdio and Streamable HTTP, deployed on Cloudflare Workers and D1. | 113 unit/integration tests + 4 end-to-end, 99.6% line coverage, 82% Stryker mutation score. `/mcp` is token-gated; the seed shop is fictional. |
| [mcp-doctor](https://github.com/kfairy9999/mcp-doctor) · [live playground](https://mcp-doctor.kfairley9999.workers.dev) | Library, CLI, and stdio MCP server that checks MCP config files against the client that will load them. | 193 tests, 93.7% line coverage. The playground validates a pasted config in-request and discards it. |
| [mcp-sync](https://github.com/kfairy9999/mcp-sync) · [demo](https://github.com/kfairy9999/mcp-sync#demo) | Synchronous Python client for the official MCP SDK, for calling MCP servers from ordinary non-async code. | 41 tests, 91% coverage, CI on Linux, macOS, and Windows. |
| [ai-sdk-resilience](https://github.com/kfairy9999/ai-sdk-resilience) · [live playground](https://ai-sdk-resilience.kfairley9999.workers.dev) | Retry, fallback, hedging, and circuit-breaker middleware for the Vercel AI SDK. | 50 tests, 97.9% coverage. The chaos playground runs against mock providers. |
| [agent-crew](https://github.com/kfairy9999/agent-crew) · [live demo](https://agent-crew.kfairley9999.workers.dev) | Multi-agent research desk in TypeScript: planner, researcher, writer, and critic share a blackboard you can watch live. | Citation checks against retrieved sources, a capped critic loop, a hard token budget. 34 unit tests. |
| [mini-agent](https://github.com/kfairy9999/mini-agent) | Tool-calling agent in Python with a self-check step and an eval harness. | 14/15 (93%) on a real Groq run, report committed. 78 tests; runs offline with a mock policy. |
| [llm-watch](https://github.com/kfairy9999/llm-watch) · [live demo](https://llm-watch.kfairley9999.workers.dev) | LLM call ledger and eval regression gate (Python, FastAPI, React), on SQLite or MongoDB. | Flags a cheaper model that drops quality, catching 6 pass-to-fail flips in the demo suite. |
| [Retrieval-Augmented-Generation](https://github.com/kfairy9999/Retrieval-Augmented-Generation) · [live demo](https://personal-knowledge-engine.kfairley9999.workers.dev) | Personal Knowledge Engine: RAG over your own files with Gemini embeddings and streamed, cited Grok answers. | Keys stay server-side; without them it falls back to keyword search. 34 tests. |
| [hermes-phone-agent](https://github.com/kfairy9999/hermes-phone-agent) | Guarded Python wrapper around the Nous Research Hermes telephony skill, with Twilio, Bland, and Vapi adapters. | Allowlist, confirmations, daily caps, quiet hours, append-only audit log. Mock mode by default; not yet used for live calls. |
| [fast-tokenizer](https://github.com/kfairy9999/fast-tokenizer) | Byte-level BPE tokenizer in Rust with Python bindings. | Exact GPT-2 token parity with tiktoken on 3.3 MB of text; about 2× tiktoken single-threaded and 140–155 MB/s on 4 threads. |

## Full-stack apps and data

| Project | What it is | Notes |
| --- | --- | --- |
| [pulse-crm](https://github.com/kfairy9999/pulse-crm) · [live demo](https://pulse-crm.kfairley9999.workers.dev/demo) | Single-owner CRM on Cloudflare Workers and D1: contacts, a six-stage pipeline, tasks, reports, and its own sign-in. | The demo runs the real CRM handlers in your browser against fictional data. 99 tests. |
| [EquiFlow-Stock-App](https://github.com/kfairy9999/EquiFlow-Stock-App) · [live demo](https://equiflow.kfairley9999.workers.dev) | Stock-tape dashboard with a moving average, drift alerts, and an optional Grok read of the tape. | Prices are simulated in the browser. Not investment advice. |
| [us-economic-dashboard](https://github.com/kfairy9999/us-economic-dashboard) · [live site](https://kfairy9999.github.io/us-economic-dashboard/) | Mobile-first dashboard of U.S. economic indicators from FRED: inflation, jobs, GDP, rates, the yield curve, and the Sahm-rule recession signal. | Python and pandas pipeline refreshed daily by GitHub Actions and published to GitHub Pages. |

## Background

- Data & Workflow Specialist at Solvis Corp (2024–present). Earlier work in IT and server management.
- Bilingual: English and Spanish

## How I work

I design and direct my projects and build them with AI coding agents. I set the requirements, test against real models and real data, and publish honest results, limits included.

[LinkedIn](https://www.linkedin.com/in/kevin-fairley-94330b42a/)
