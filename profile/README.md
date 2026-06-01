# Superfield

**Autonomous Software Research Lab**

Superfield is an open research lab exploring the infrastructure
required for a world where software is designed, built, and maintained
by **autonomous AI systems**.

We study how constellations of agents can collaborate to produce
software, operate infrastructure, and evolve systems faster than
traditional development models allow.

Our work focuses on **autonomous software systems**, **AI-native
infrastructure**, and **post-human development models**.

------------------------------------------------------------------------

## Our Research

<div align="center">

| **PLATFORM** | **ARCHITECTURE** |
|:---:|:---:|
| [![Superfield IDE](https://img.shields.io/badge/SUPERFIELD_IDE-Supergreenfield-7b2fff?style=for-the-badge&logo=rocket)](https://github.com/superfield-ai)<br><br>The **Supergreenfield Platform**.<br>Build entirely new applications<br>with autonomous AI systems. | [![Alien Stack](https://img.shields.io/badge/ALIEN_STACK-Post--Human_Arch-00ff88?style=for-the-badge&logo=linux)](https://github.com/superfield-ai/alien-stack)<br><br>The **Post-Human Stack**.<br>Software ecosystems designed<br>for AI authorship and evolution. |
| **MEMORY** | **FACTORY** |
| [![Facet](https://img.shields.io/badge/FACET-Context_Layer-ff00ff?style=for-the-badge&logo=rust)](https://github.com/superfield-ai/facet)<br><br>The **Memory Layer** for AI systems.<br>Separates persistent knowledge<br>from model inference. | [![Nightshift](https://img.shields.io/badge/NIGHTSHIFT-Agent_Ops-00ffff?style=for-the-badge&logo=github)](https://github.com/superfield-ai/nightshift)<br><br>The **Autonomous Factory**.<br>Agents collaborate on development<br>tasks around the clock. |
| **BROWSER** | **INFERENCE** |
| [![Robert](https://img.shields.io/badge/ROBERT-Agent_Browser-ffff00?style=for-the-badge&logo=google-chrome)](https://github.com/superfield-ai/robert-browser)<br><br>The **AI-Native Browser**.<br>Agents interact with the web<br>and integrate external systems. | [![Inferno](https://img.shields.io/badge/INFERNO-Inference_Cloud-ff4400?style=for-the-badge&logo=rust)](https://github.com/superfield-ai/inferno)<br><br>The **Inference Platform**.<br>High-performance, reliable LLM<br>deployment for autonomous systems. |

</div>

---

### Superfield IDE

```text
   _____                       _____      __    __   ________  ______
  / ___/__  ______  ___  _____/ __(_)__  / /___/ /  /  _/ __ \/ ____/
  \__ \/ / / / __ \/ _ \/ ___/ /_/ / _ \/ / __  /   / // / / / __/
 ___/ / /_/ / /_/ /  __/ /  / __/ /  __/ / /_/ /  _/ // /_/ / /___
/____/\__,_/ .___/\___/_/  /_/ /_/\___/_/\__,_/  /___/_____/_____/
          /_/
```

Superfield IDE is a method, toolset, and reference implementation for building
**supergreenfield applications** — software designed from the ground up
for autonomous AI development.

The core premise: *N* smart AIs across *N* vendor data silos will always
produce worse outcomes than a single AI over fused, coherent, owned data.
Superfield IDE replaces fragmented SaaS stacks with applications that are:

-   **Fused** --- one AI over coherent, owned data
-   **Tree-shaken** --- only the 5% of features you actually use
-   **Correct by construction** --- every line verified, no mocks, no ORMs
-   **Self-improving** --- the agent has live access to logs and telemetry,
    and enters hardening mode when there is nothing left to build

The reference implementation uses Bun, React, Tailwind,
and SQLite/PostgreSQL — no Docker, no ORMs, no SaaS auth vendors.

### [Alien Stack](https://github.com/superfield-ai/alien-stack)

```text
  _   _ _             ___ _           _
 /_\ | (_)___ _ __   / __| |_ __ _ __| |__
/ _ \| | / -_) '  \  \__ \  _/ _` / _| / /
/_/ \_\_|_\___|_|_|_| |___/\__\__,_\__|_\_\
```

Alien Stack is a research program investigating **agent-native software
architecture** — what the software stack looks like when humans are fully
out of the development loop.

The central idea: agents don't need human-readable source code. Alien
Stack explores generating and optimizing **Proof-Carrying Functions (PCFs)**
directly in LLVM IR, compiled to WebAssembly, with text serving only as
a navigational view. The architecture rests on three pillars:

-   **Isomorphic architecture** --- LLVM IR maps 1-to-1 to the WASM
    deployment artifact, with no transpiler mangling
-   **AI-native development** --- code annotated with structural tags
    (`@module`, `@fn`, `@calls`) so agents navigate via `grep`, not
    language servers; proofs of behavior verified at link time
-   **Microkernel client** --- the browser treated as a dumb hardware
    substrate; zero frameworks, all logic in the Wasm module

Demos show agent-authored LLVM IR **outperforming equivalent Rust Hyper
servers** on TechEmpower plaintext benchmarks — built in under 15 minutes,
no internet searches, no build tool setup.

### [Inferno](https://github.com/superfield-ai/inferno)

```text
 _ __ _ ____ ____ ____ __ _ ____
 | | \| |--- |=== |--< | \| [__]
```

Inferno is a **self-healing cloud platform for AI inference**, built
end-to-end in Rust with an emphasis on performance and reliability.

A dual-server architecture separates the load-balancing proxy (Pingora)
from the inference backend (Hyper), with SWIM protocol for self-healing
node discovery. Performance targets: under 1ms P99 latency, over 100,000
requests per second, under 1KB memory per concurrent connection.

The **Enterprise Edition** adds Governator AI — automatic GPU profiling,
optimal model placement, and real-time load distribution adjustments.

### [Nightshift](https://github.com/superfield-ai/nightshift)

```text
   _  ___      __   __      __   _ _____
  / |/ (_)__ _/ /  / /____ / /  (_) _/ /_
 /    / / _ `/ _ \/ __(_-</ _ \/ / _/ __/
/_/|_/_/\_, /_//_/\__/___/_//_/_/_/ \__/
       /___/
```

Nightshift is a methodology and toolset for **autonomous software
factories** — structured so agents can build, maintain, and document
large software projects without catching fire.

Core concepts:

-   **Git-Brain** --- commits as a Reasoning Ledger; prompt and intent
    stored in hidden metadata for perfect replayability
-   **Deep Context** --- a Documentation Fractal anchored by
    `docs/README.md` that lets agents orient themselves without RAG or
    vector stores
-   **Nags** --- mandatory quality gates agents must pass before marking
    tasks complete
-   **Semantic Worktrees** --- branches named like file paths
    (`ns/session/option-a`) to show lineage and intent

Available as a **methodology** (installs `.nightshift/` templates and git
hooks into any repo) or a **service** (standalone CLI/TUI managing
multiple agents, API costs, and background runs). Supports Claude Code,
Cursor, Gemini CLI, and Codex.

### [Facet](https://github.com/superfield-ai/facet)

```text
  ___            _
 | __|_ _ __ ___| |_
 | _/ _` / _/ -_)  _|
 |_|\__,_\__\___|\__|
```

Facet is the **Context OS** for AI — a neutral, trusted memory layer that
separates knowledge management from model inference, giving users full
control over what data influences AI outputs.

The core insight mirrors how the browser unbundled the OS from the web:
Facet unbundles memory from the model. A three-layer architecture keeps
encryption keys on the user's device, sync and computation in Facet's
cloud, and reasoning providers receiving only anonymized context.

GraphRAG provides entity-relationship mapping with temporal reasoning and
hierarchical memory tiers (hot/warm/cold), enabling features like
Reactive Pruning — excluding stale documents from generation without
deleting them.

### [Robert](https://github.com/superfield-ai/robert-browser)

```text
 +-+-+-+-+-+-+
 |R|o|b|e|r|t|
 +-+-+-+-+-+-+
```

Robert is a **WebDriver library for AI-driven browser automation**, giving
agents the infrastructure to hook into browser workflows headlessly or
visually.

Two components: **robert-webdriver**, a Rust CLI and library for
connecting agents to browser drivers; and **robert-browser**, a Tauri
desktop GUI demonstrating the capabilities in an accessible interface.
Supports headless and visual modes, built for reliability and performance
in Rust.

------------------------------------------------------------------------

## A Moment of Opportunity

Software is entering a new era.

For decades, the limiting factor in software quality has been **human
time**. Testing, verification, documentation, and security review are
all expensive processes that teams must constantly trade against
deadlines.

Autonomous systems change that constraint.

AI agents can read every line of a codebase, trace every dependency,
explore every edge case, and continuously refine systems at a scale that
human teams cannot realistically sustain.

If used correctly, this enables something new:

-   deeper testing
-   stronger verification
-   better documentation
-   more resilient infrastructure
-   faster iteration with higher confidence

In other words, **software that is more reliable, more understandable,
and more maintainable than what we can build today.**

Superfield explores the infrastructure required to make that future
practical.

Our goal is not to replace software engineers.

Our goal is to build systems where humans and autonomous agents
collaborate to produce **the most robust software systems ever
created.**

------------------------------------------------------------------------

## Research Areas

Our research explores several emerging domains:

**Autonomous Software Factories**\
Systems where AI agents design, write, test, and deploy software.

**Multi-Agent Orchestration**\
Coordinating specialized AI systems across providers and reasoning
models.

**Vendor-Neutral AI Infrastructure**\
Architecture that avoids lock-in to any single model provider.

**AI-Native Tooling**\
Browsers, memory systems, and operational frameworks designed for agents
rather than humans.

**Post-Human Software Architecture**\
Exploring what software engineering becomes when AI is the primary
author of code.

------------------------------------------------------------------------


## License

All Superfield projects are available under a **dual license**:

-   Non-Commercial: Apache 2.0 or MIT
-   Commercial: Requires a commercial license for proprietary
    operational deployments
