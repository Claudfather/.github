# Claudfather

The place where Claude Code agents are raised, equipped, and continuously improved.

Claudfather is an open-source ecosystem of four interlocking repositories for building, distributing, and evolving Claude Code agent infrastructure. Run a fleet of distinct, cooperating bots on cheap hardware — no hosted dependencies required.

## The Ecosystem

```
┌───────────────────────────────────────────────────────────────┐
│                         Claudfather                           │
│                                                               │
│   ┌───────────┐    promotes    ┌──────────────┐               │
│   │  clauDNA  │ ◄────────────  │ Claudosseum  │               │
│   │ (plugin)  │                │   (arena)    │               │
│   └─────┬─────┘                └──────▲───────┘               │
│         │ installed                   │ telemetry,            │
│         │ on bots                     │ scenarios             │
│         ▼                             │                       │
│   ┌─────────────┐    queries    ┌─────┴─────────┐             │
│   │ Claudlobby  │ ────────────► │   Claudron    │             │
│   │   (fleet)   │ ◄──────────── │  (knowledge)  │             │
│   └─────────────┘    writes     └───────────────┘             │
│                                                               │
└───────────────────────────────────────────────────────────────┘
```

| Repo | Role | Status |
|------|------|--------|
| [**Claudlobby**](https://github.com/Claudfather/Claudlobby) | Fleet compositor. Transforms `fleet.yaml` + a shared library into runnable bot directories with isolated identities, MCP servers, skills, and systemd/launchd supervision. | Active development |
| [**clauDNA**](https://github.com/Claudfather/clauDNA) | Canonical skills, hooks, and agents for Claude Code. The shared genome that bots inherit. | Active development |
| [**Claudosseum**](https://github.com/Claudfather/Claudosseum) | Promotion engine. An arena where skills are evaluated and evolved, deciding what earns a place in clauDNA. | Design phase |
| [**Claudron**](https://github.com/Claudfather/Claudron) | Markdown-based knowledge graph. Bots write findings during operation; future bots query before acting. Plain files, git-backed, locally owned. | Design phase |

## How They Work Together

**Promotion loop:** Skills enter Claudosseum, battle in the arena with real-world telemetry contributing to their score, and champions get promoted into the next clauDNA release.

**Knowledge loop:** Claudlobby bots write findings to Claudron during operation. Future bots query Claudron before acting. Recurring patterns become candidates for new skills.

**Grounding loop:** Claudosseum battles draw scenarios from Claudron content, so skills are evaluated against problems bots have actually encountered.

## Principles

- **Local-first.** Run the entire ecosystem on your own hardware. No hosted dependencies for basic use.
- **Tight repo boundaries.** Each repo has one job. clauDNA distributes, Claudosseum evaluates, Claudlobby runs, Claudron stores.
- **Bots are distinct entities.** Each bot gets its own identity, state, and isolation. The system never collapses them into one.
- **Open source.** Everything is OSS. Hosted infrastructure is opt-in and replaceable.

## Getting Started

Start with [Claudlobby](https://github.com/Claudfather/Claudlobby) to run your first bot fleet, or [clauDNA](https://github.com/Claudfather/clauDNA) to install champion skills on a single Claude Code instance.

See [PROJECT_MISSION.md](https://github.com/Claudfather/.github/blob/main/PROJECT_MISSION.md) for the full vision, open questions, and design decisions.
