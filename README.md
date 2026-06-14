# Hey, I'm FugoP 👋

> Building **PENSO** — corporate governance, implemented for AI organizations.
> [governances.ai](https://governances.ai)

I design and operate **AI agent organizations**: multi-agent systems where Claude, Codex, and Gemini work as a governed team — not as individual tools.

My focus is **AI management**, not prompt engineering:
- Prompt engineering → how to talk to an AI
- AI management → how to build systems where AI judgment can be trusted, reviewed, and gradually delegated under human oversight

---

## 🔭 What I'm building

**PENSO** — an operating system for AI organizations, built on one idea: *governance by structure*. Oversight, separation of duties, and accountability are implemented as architectural constraints the system cannot bypass — not as policy PDFs or dashboards bolted on afterwards.

- **Agent runtime governance** — permission models, execution boundaries, and decision records for agentic systems
- **Separation of execution and audit** — the component that reviews an action is independent of the one that performs it
- **Human-reviewed AI** — keeping humans meaningfully in the loop without giving up the speed
- **Multi-agent orchestration** — routing, role separation, and quality gates across Claude / Codex / Gemini

More on the thesis — *Separation of Powers as Governance Architecture* — at [governances.ai](https://governances.ai).

---

## 🤝 Open source & standards

Shipping merged code into AI-infra OSS, and contributing to the semantic-convention work that defines how agent runtimes are described — kept implementation-neutral, with producer-owned context left out of scope:

- **[litellm](https://github.com/BerriAI/litellm)** (LLM gateway, ~50k★) — [merged PRs »](https://github.com/BerriAI/litellm/pulls?q=is%3Apr+author%3AAgentGymLeader+is%3Amerged)
- **OpenTelemetry GenAI semconv** — design input on agent telemetry: decision / outcome attributes and opaque, payload-free governance references for agent decision points; an *acting-vs-target* agent framing for multi-agent traces; runtime threat-signal correlation
- **Agent execution-record proposals** — review input on keeping the normative contract in the spec itself, rather than in any single reference implementation, so independent implementations interoperate on equal footing
- **Microsoft Agent Governance Toolkit (AGT)** — telemetry and observability design discussions
- **[`otel-agent-evidence-sample`](https://github.com/AgentGymLeader/otel-agent-evidence-sample)** — a small reference for the opaque `correlation_id` evidence-linking pattern (MIT)

→ *[All merged contributions, always current »](https://github.com/search?q=is%3Apr+author%3AAgentGymLeader+is%3Amerged&type=pullrequests)*

---

## 🔒 Security hardening (selected)

Memory-safety, injection, and trust-boundary fixes proposed into ML / data-infra OSS —
AI-assisted discovery, human-verified before submission. Status shown honestly; most are
under maintainer review.

- **[mongodb/mongo-python-driver#2872](https://github.com/mongodb/mongo-python-driver/pull/2872)** — bounds check for an out-of-range embedded-document length in the BSON C-extension raw-batch path · *under review*
- **[facebookresearch/faiss#5312](https://github.com/facebookresearch/faiss/pull/5312)** — harden the OnDiskInvertedLists mmap reader against malformed list sizes · *under review*
- **[facebookresearch/faiss#5313](https://github.com/facebookresearch/faiss/pull/5313)** — guard against integer overflow in index-deserialization size checks · *under review*
- **[aws/sagemaker-python-sdk#5947](https://github.com/aws/sagemaker-python-sdk/pull/5947)** — use the caller's extract_path (not CWD) as the tar-extraction containment base · *under review*
- **[run-llama/llama_index#21962](https://github.com/run-llama/llama_index/pull/21962)** — fix SQL injection in the MariaDB / DB2 vector stores (sibling of CVE-2025-1793) · *under review*
- **[feast-dev/feast#6512](https://github.com/feast-dev/feast/pull/6512)** — warn operators when the registry server starts with authentication disabled · *under review*

Method: a cross-model find → verify → fix loop (Claude + Codex), every finding adversarially
checked before a PR is opened — no exploit code, regression test where the project's suite allows.

---

## 🧠 Background

- 🎓 Tokyo Institute of Technology — Robotics (graduated top of class)
- 🦅 Human-Powered Aircraft Competition — 1st place, as aircraft architect
- Robotics background, not CS — running a fully AI-native org. The interesting problem isn't *can-build vs. can-deploy*; it's **can-build vs. can-govern**.

---

## 🛠️ Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-D4A27F?style=flat&logo=anthropic&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat&logo=googlecloud&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)

**Daily drivers:** Claude, Codex, Gemini, Python, GitHub Actions, Cloud Run

---

## 💬 Collaboration

Interested in **agent governance**, **human-AI decision systems**, or **AI org design**? Open an issue in this repository to start a conversation.

I don't publish a public email address on GitHub.
