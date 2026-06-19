# AgentGymLeader 👋

Hey, glad you wandered in. The handle's half a joke and half the actual thesis.

In that world, a Gym Leader is the boss at the end of the gym. But here's the twist — they're on your side: the whole job is to push a team until it's strong and resourceful enough to get past you, to recognize them when their setup genuinely holds up, and to raise the level of the whole region, not just the few who walk in.

My type is AI agent governance. Same shape of work: take a team of agents (Claude, Codex, Gemini), push them until they're trustworthy enough to actually delegate to, and treat "it holds up" as something you build toward — for everyone, not just yourself.

So most of the work happens in the open, lifting the tools people already build on:

- **[Microsoft Agent Governance Toolkit](https://github.com/microsoft/agent-governance-toolkit)** — [merged prompt-injection defense rules](https://github.com/microsoft/agent-governance-toolkit/pull/3069)
- **[Meta Faiss](https://github.com/facebookresearch/faiss)** — [merged search-index hardening](https://github.com/facebookresearch/faiss/pull/5312)
- **[OpenTelemetry GenAI](https://github.com/open-telemetry/opentelemetry-python-genai)** — [merged vendor-neutral agent telemetry](https://github.com/open-telemetry/opentelemetry-python-genai/pull/111)

→ *[All merged contributions, always current »](https://github.com/search?q=is%3Apr+author%3AAgentGymLeader+is%3Amerged&type=pullrequests)*

---

## 🔭 The through-line

It all points at one project: **PENSO**, an operating system for AI organizations built on *governance by structure* — permission models, separation of execution and audit, and decision records implemented as constraints the system can't bypass, not policy PDFs bolted on afterward. Same idea as the gym: a team earns real autonomy *because* the structure around it is sound. More at [governances.ai](https://governances.ai).

---

## 🤝 More open source & standards

Beyond the headline merges, I work the semantic-convention layer that defines how agent runtimes get described — kept implementation-neutral, with producer-owned context left out of scope:

- **[litellm](https://github.com/BerriAI/litellm)** (LLM gateway, ~50k★) — [merged PRs »](https://github.com/BerriAI/litellm/pulls?q=is%3Apr+author%3AAgentGymLeader+is%3Amerged)
- **Agent execution-record proposals** — review input on keeping the normative contract in the spec itself, rather than in any single reference implementation, so independent implementations interoperate on equal footing
- **[`otel-agent-evidence-sample`](https://github.com/AgentGymLeader/otel-agent-evidence-sample)** — a small reference for the opaque `correlation_id` evidence-linking pattern (MIT)

---

## 🔒 Security hardening (selected)

Memory-safety, injection, and trust-boundary fixes proposed into ML / data-infra OSS —
AI-assisted discovery, human-verified before submission. Status shown honestly; most are
under maintainer review.

- **[MongoDB BSON driver](https://github.com/mongodb/mongo-python-driver/pull/2872)** — bounds check for an out-of-range embedded-document length in the BSON C-extension raw-batch path · *under review*
- **[Faiss](https://github.com/facebookresearch/faiss/pull/5313)** — guard against integer overflow in index-deserialization size checks · *under review*
- **[AWS SageMaker Python SDK](https://github.com/aws/sagemaker-python-sdk/pull/5947)** — use the caller's extract_path (not CWD) as the tar-extraction containment base · *under review*
- **[LlamaIndex](https://github.com/run-llama/llama_index/pull/21962)** — fix SQL injection in the MariaDB / DB2 vector stores (sibling of CVE-2025-1793) · *under review*
- **[Feast](https://github.com/feast-dev/feast/pull/6512)** — warn operators when the registry server starts with authentication disabled · *under review*

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
