# Awesome-AI-Telemetry-Observability-Stacks

## Top AI Telemetry & Observability Stacks Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Agent Tracing, Evaluation & Production Monitoring*  

**Last updated: March 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Telemetry & Observability**. These tools give teams high-granularity loggers tracing exact agent decision chains, model calls, tool usage, and API failures—turning opaque LLM behavior into inspectable, debuggable traces.



**Examples** include Langfuse, Arize AI, Helicone, LangSmith, OpenLIT, Traceloop, HoneyHive, Braintrust, Weights & Biases Weave, and Comet Opik (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, OpenTelemetry-native instrumentation, and open evaluation frameworks—ideal for AI engineers, platform teams, and developers seeking transparent, vendor-independent agent observability.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[LangSmith](https://smith.langchain.com/)**  

  LangChain's first-party observability and evaluation platform. Deepest LangChain/LangGraph integration with annotation queues, Polly AI debugging, and prompt management. Processes 1B+ events/day and serves ~35% of Fortune 500. Closed platform with open MIT SDK—enterprise self-hosting only .



- **[Arize AI (AX)](https://arize.com/)**  

  Enterprise AI monitoring with production-scale telemetry and 50+ research-backed eval metrics. Arize Phoenix is the open-source counterpart under Elastic 2.0 license (source-available, not OSI-approved). Unified ML + LLM observability .



- **[Braintrust](https://www.braintrust.dev/)**  

  Eval-first observability with CI/CD quality gates. $124M raised, used by Notion, Stripe, and Vercel. Treats prompts as CI artifacts. Closed platform with open SDKs .



- **[Weights & Biases Weave](https://wandb.ai/site/weave/)**  

  LLM tracing and eval unified with W&B's ML experiment tracking heritage. $50/user/month. Auto-instruments major frameworks. SaaS backend with Apache-2.0 SDK .



- **[HoneyHive](https://www.honeyhive.ai/)**  

  AI observability and evaluation platform with tracing, datasets, and automated scoring for production LLM applications.



- **[Helicone](https://www.helicone.ai/)**  

  YC W23. Proxy-first observability—change `api.openai.com` to `oai.helicone.ai` for zero-code logging. Also supports async SDK mode. Features caching, 100+ models, and growing eval/prompt capabilities. **Note: Acquired by Mintlify in March 2026 and in maintenance mode** .



- **[Traceloop](https://www.traceloop.com/)**  

  Built around OpenLLMetry (Apache-2.0), the leading OpenTelemetry instrumentation library for LLMs. Emits standard `gen_ai` spans portable to any OTel backend. Hosted platform adds monitoring, evals, and CI/CD. **Traceloop announced joining ServiceNow in 2026—confirm roadmap during evaluation** .



- **[Aporia](https://www.aporia.com/)**  

  AI observability and guardrails platform with real-time monitoring, custom metrics, and investigation workflows for ML and LLM systems.



- **[Fiddler AI](https://www.fiddler.ai/)**  

  Enterprise AI observability and model performance monitoring with explainability, bias detection, and LLM evaluation.



## Open-Source GitHub Projects



- **[Langfuse](https://github.com/langfuse/langfuse)**  

  The open-source default for LLM engineering (MIT core, enterprise extras commercially licensed). **35,000+ GitHub stars** as of October 2026 . Covers tracing, evaluations, prompt management, datasets, and cost tracking in one self-hostable platform. Framework-agnostic—integrates across LlamaIndex, CrewAI, OpenAI Agents SDK, Claude Agent SDK, and coding agents like Claude Code, Codex, Goose, and Pi . **Acquired by ClickHouse in January 2026 with commitment to keep it open source under existing license** . Self-hosted is free, unlimited. Cloud from $29/month. Accepts OpenTelemetry data; SDK built on OpenTelemetry client .



- **[Comet Opik](https://github.com/comet-ml/opik)**  

  The closest fully-permissive rival to Langfuse (Apache-2.0, **22,000+ GitHub stars**). Full platform—backend included—free to self-host. Covers AI agent tracing, LLM evaluation, prompt optimization, production monitoring, and **Opik Guardrails** for responsible AI . **Extensive integration catalog**: Google ADK, Autogen, AG2, Flowise AI, CrewAI, LangGraph, LlamaIndex, OpenAI Agents, Anthropic, Bedrock, Gemini, Groq, Dify, DSPy, LiteLLM, Ollama, OpenTelemetry, and more . Docker Compose for local, Kubernetes Helm for production. Non-root containers for security .



- **[Arize Phoenix](https://github.com/Arize-ai/phoenix)**  

  Open-source LLM and ML observability built on OpenTelemetry and OpenInference conventions. **2.5M+ monthly downloads**, **10,800+ GitHub stars**. Runs locally (notebook, Docker) with zero external dependencies. Strong RAG debugging with nested spans and multimodal support (image previews). Built-in evaluator catalog, dataset management, and LLM-judge. **License: Elastic 2.0 (source-available, not OSI-approved)**—restricts offering it as a competing hosted service .



- **[OpenLLMetry (Traceloop)](https://github.com/traceloop/openllmetry)**  

  Apache-2.0 OpenTelemetry instrumentation for LLM providers, vector DBs, and frameworks. **7,300+ GitHub stars**. Emits standard `gen_ai` spans portable to any OTel backend—Datadog, Grafana Tempo, Jaeger, or a self-hosted collector. The cleanest standards story: no lock-in, pure instrumentation. Pair with any backend .



- **[OpenLIT](https://github.com/openlit/openlit)**  

  Apache-2.0, OpenTelemetry-native AI engineering platform. **60+ integrations**. Uniquely combines **LLM + GPU + VectorDB observability** under one roof. Runs on ClickHouse, free to self-host. Adds guardrails and prompt hub to tracing and cost tracking. Essential when GPU spend monitoring matters .



- **[MLflow Tracing](https://github.com/mlflow/mlflow)**  

  Apache-2.0. Brings LLM tracing and evaluation to MLflow, which many data teams already run. OpenTelemetry compatible. Natural choice if your ML platform is built on MLflow or Databricks—less operational change than introducing another platform .



- **[Laminar](https://github.com/lmnr-ai/lmnr)**  

  Younger Apache-2.0 project focused on tracing AI agents. Built on OpenTelemetry and ClickHouse. **3,200+ GitHub stars** .



- **[agent-xray](https://pypi.org/project/agent-xray/)**  

  Open-source agent decision inspector that **reconstructs the full decision surface** for each step—system prompt hash, conversation history, tool set, model metadata, browser cues, and prior corrections. Grades tasks against JSON rulesets (default, browser_flow, coding_agent, research_agent). Supports generic JSONL, OpenAI Agents, Anthropic, LangChain/LangGraph, CrewAI, and OTel GenAI spans. Commands: `analyze`, `surface`, `reasoning`, `diff`, `grade`, `root-cause`. Includes task-bank-aware grading for curated expectations .



- **[agenttracer](https://pypi.org/project/agenttracer-ai/)**  

  Open-source SDK for tracing agent decision chains with first-class **fork/merge support for multi-agent orchestration**. Logs model calls, tool calls, and **branching decisions with reasoning** (`log_decision`). Fork into parallel branches (`search`, `analysis`, `writing`), log each subagent linked by fork_span, then merge back. Dashboard shows interactive DAG visualization. Token usage tracking with auto-estimation or exact counts. Export to JSON or Markdown. CLI: `agenttracer dashboard`, `list`, `export` .



- **[auditable](https://github.com/yzhao062/auditable)**  

  Open-source agent decision auditor that builds **one typed graph** across execution (control flow) and dependency (what each step relied on) edges. Identifies the **keystone**—the step that most of the run transitively rests on. Binds three spans per decision (Data, Model, Harness) into a signed, hash-chained record. **`replay()`** re-derives whether an action still holds under live dependency state, returning `ALLOW`, `ROLLBACK` (stale-state), `BLOCK`, or `HUMAN_REVIEW`. Post-commit rollback via `rail.compensate(receipt)` .



- **[DeepEval](https://github.com/confident-ai/deepeval)**  

  Apache-2.0 evaluation framework. LLM-as-a-judge metrics for hallucination, RAG assessment, and safety.



- **[Evidently](https://github.com/evidentlyai/evidently)**  

  Apache-2.0. Data and model drift detection for ML and LLM systems.



- **[Promptfoo](https://github.com/promptfoo/promptfoo)**  

  MIT. LLM testing and red-teaming framework. **20,000+ GitHub stars**. OpenAI announced acquisition in March 2026 with commitment to keep the open-source project going .



- **[LiteLLM](https://github.com/BerriAI/litellm)**  

  Apache-2.0 AI gateway. Tracks spend per key, user, and team. Forwards logs to observability backends. 100+ models .



### Additional Strong Open-Source Options



- **[OpenTelemetry GenAI Semantic Conventions](https://github.com/open-telemetry/semantic-conventions-genai)** — Vendor-neutral standard attribute names for model calls, agents, and tool use. Still in development but most tools are moving toward them. Building on them now makes switching tools later much easier .

- **[AgentOps](https://github.com/AgentOps-AI/agentops)** — Session replay and fast time-to-first-trace for agent monitoring .

- **[Logfire (Pydantic)](https://github.com/pydantic/logfire)** — MIT SDK but closed server. Python-native observability with OTel foundations.

- **[openllmetry](https://github.com/traceloop/openllmetry)** — Community instrumentations for LLM providers and vector DBs (Apache-2.0).

- Community **n8n** workflows for observability alerting and trace-driven automation.



**Frameworks for building custom systems**: Combine **Langfuse** or **Comet Opik** as the full observability platform with **OpenLLMetry** for OTel-native instrumentation, **agent-xray** or **agenttracer** for deep agent decision inspection, **auditable** for dependency-graph keystone analysis and rollback, and **ClickHouse/PostgreSQL** for trace storage—creating a fully self-hosted, enterprise-grade agent telemetry stack.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- AI observability stacks handling prompts and traces must comply with data protection regulations (GDPR, CCPA, etc.), especially when traces contain PII or regulated data.

- **Self-hosting is a hard requirement when prompts or traces carry regulated data.** If they do, the field collapses to Langfuse, Opik, OpenLLMetry, and OpenLIT—LangSmith and Braintrust cannot self-host, and Weave's backend is SaaS .

- **"Open source" means four different things in this category** : Apache-2.0 (Opik, OpenLLMetry, OpenLIT) is genuinely permissive. Open core (Langfuse) means the core is MIT but governance features—RBAC, audit logs, SCIM, SSO, retention, masking—are commercially licensed. Source-available (Phoenix, Elastic 2.0) lets you read and modify but restricts offering it as a service, and is not OSI-approved. Closed (LangSmith, Braintrust) publishes only client SDKs. **Check the LICENSE file, not the marketing page** .

- **Observability is not evaluation.** Tracing tells you what happened; evaluation tells you whether it was good. Most tools ship both—which makes it easy to buy one and never configure the other. Tracing alone will not catch quality drift .

- **Ownership changes are part of the picture.** Three tools changed owners in 2026: Langfuse acquired by ClickHouse (January), Helicone acquired by Mintlify (March, now maintenance mode), Traceloop joining ServiceNow. A tool with an active community and clear long-term owner is a safer foundation .



---



**Made for AI engineers, platform teams, and developers building transparent agent observability solutions.**  

Let's make AI Telemetry & Observability more open, data-driven, and debuggable.
