# Hi, I'm Kevin Fairley

Living in Los Angeles. I build AI agents, LLM tooling, and automation in **Python, TypeScript, and Rust**. I'm open to roles in agentic AI and LLM engineering.

Every project below has tests and CI, and each web app has a live demo you can open without an account. When a demo runs without a model key, the page says so and labels its sample output as sample output.

## Agentic AI and LLM tooling

| Project | What it is | Results |
| --- | --- | --- |
| [leadflow-mcp](https://github.com/kfairy9999/leadflow-mcp) · [live endpoint](https://leadflow-mcp.kfairley9999.workers.dev/health) | An MCP server in TypeScript that lets Claude, Cursor, or any MCP client run a small shop's lead pipeline: 11 tools, 3 resources, and 2 prompts to capture, score, follow up, and report. stdio and Streamable HTTP on SQLite, live on Cloudflare Workers and D1. | 113 unit and integration tests plus 4 end-to-end tests, 99.61% line and 96.88% branch coverage, 82% Stryker mutation score. `/mcp` requires a bearer token, and the seed shop is fictional. |
| [mcp-doctor](https://github.com/kfairy9999/mcp-doctor) · [live playground](https://mcp-doctor.kfairley9999.workers.dev) | A TypeScript library, CLI, stdio MCP server, and playground that checks MCP config files against the client that will load them. | 193 tests, 93.69% line and 85.81% branch coverage. The playground validates a pasted config (up to 64KB) in the request and then drops it; PATH checks and live handshakes stay on your machine. Not published to npm; the npm name belongs to an unrelated package. |
| [mcp-sync](https://github.com/kfairy9999/mcp-sync) | A synchronous Python client for the official MCP Python SDK, for calling MCP servers from ordinary, non-async code. | 41 tests, 91% coverage, CI on Linux, macOS, and Windows. The demo is a recorded run in the README. Install from GitHub; the PyPI name belongs to an unrelated project. |
| [ai-sdk-resilience](https://github.com/kfairy9999/ai-sdk-resilience) · [live playground](https://ai-sdk-resilience.kfairley9999.workers.dev) | Retry, fallback, hedging, and circuit-breaker middleware for the Vercel AI SDK 7. | 50 tests, 97.9% coverage. The chaos playground uses mock providers only, does not accept API keys, and rejects request bodies larger than 16KB. Not published to npm. |
| [agent-crew](https://github.com/kfairy9999/agent-crew) · [live demo](https://agent-crew.kfairley9999.workers.dev) | A multi-agent research desk in TypeScript. A planner, researcher, writer, and critic share one blackboard, and you can watch each agent work live. | Citation checks against retrieved sources, a capped critic loop, and a hard token budget. 34 unit tests. The public demo replays a labeled, scripted run. |
| [mini-agent](https://github.com/kfairy9999/mini-agent) | A tool-calling AI agent in Python with a self-check step and an eval harness. | 14/15 (93%) on a real Groq model run, with the report committed. 78 tests. Runs offline with a mock policy. |
| [llm-watch](https://github.com/kfairy9999/llm-watch) · [live demo](https://llm-watch.kfairley9999.workers.dev) | An LLM call ledger and eval regression gate (Python, FastAPI, React). | It flags a cheaper model that drops quality, catching 6 pass-to-fail flips in the demo suite. The demo data is synthetic and labeled. |
| [Retrieval-Augmented-Generation](https://github.com/kfairy9999/Retrieval-Augmented-Generation) · [live demo](https://personal-knowledge-engine.kfairley9999.workers.dev) | Personal Knowledge Engine: RAG over your own files. Chunks in the browser, Gemini embeddings, streamed Grok answers that cite the retrieved passages. | Keys stay on the server. Without keys it falls back to a labeled keyword-search mode that shows the matching passages instead of a generated answer. 34 tests. |
| [hermes-phone-agent](https://github.com/kfairy9999/hermes-phone-agent) | A guarded Python wrapper around the official Nous Research Hermes telephony skill, with mock-first Twilio, Bland, and Vapi adapters. | Allowlist, confirmation, daily caps, quiet hours, and an append-only audit log. Default is mock mode; no live Twilio, Bland, or Vapi calls or texts have been sent. |
| [fast-tokenizer](https://github.com/kfairy9999/fast-tokenizer) | A byte-level BPE tokenizer in Rust with Python bindings. | Exact GPT-2 token parity with tiktoken on 3.3 MB of text. About 2× tiktoken from Python on one thread, and 140–155 MB/s on 4 threads across runs. |

## Full-stack apps on Cloudflare Workers

| Project | What it is | Notes |
| --- | --- | --- |
| [pulse-crm](https://github.com/kfairy9999/pulse-crm) · [live demo](https://pulse-crm.kfairley9999.workers.dev/demo) | A single-owner CRM: contacts, a six-stage pipeline, tasks, and reports, on Workers and D1 with its own sign-in. | The demo runs the real CRM handlers in your browser against fictional sample data, so it never touches the private workspace. 82 tests. |
| [Veo-3D-Architect](https://github.com/kfairy9999/Veo-3D-Architect) · [live demo](https://veo-3d-architect.kfairley9999.workers.dev) | Turns up to three reference photos and a shot description into an 8-second video with xAI Grok Imagine. | The key stays on the Worker, and a Durable Object enforces a hard daily render cap. Live rendering is off until a key is added, and the page says so. 30 tests. |
| [EquiFlow-Stock-App](https://github.com/kfairy9999/EquiFlow-Stock-App) · [live demo](https://equiflow.kfairley9999.workers.dev) | A stock-tape dashboard with a moving average, drift alerts, and an optional Grok read of the tape. | Prices are simulated in the browser and labeled that way. Not investment advice. |

## Background

- U.S. Marine Corps, 2010–2014
- Data & Workflow Specialist at Solvis Corp (2024–present). Earlier work in IT and server management.
- Bilingual: English and Spanish

## How I work

I design and direct my projects and build them with AI coding agents. I set the requirements, test against real models and real data, and publish honest results, limits included.

[LinkedIn](https://www.linkedin.com/in/kevin-fairley-94330b42a/)
