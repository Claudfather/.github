# Claudfather

## What we're building

Persistent teams of specialist AI agents that help people move a business or project forward. A person brings the goal, chooses the team's authority, reviews its work, and supplies direction when a decision needs them. The software keeps the team running and makes its activity understandable.

The first users can be technical. The longer-term aim is to make this accessible to someone with a problem to solve, without requiring them to assemble an agent platform themselves. A useful first team builds web applications with sound engineering and a clear audience and business purpose. Teams for research, content, commerce, and other work fit the same direction.

**Public promise:** Run a fleet of AI workers. Specialist teams on hardware you own.

## Responsibilities

| Part | Owns |
| --- | --- |
| **Claudlobby** | Composition, installation and setup state, integration wiring, permissions, secrets on the host, supervision, operational records, and the canonical Plane display and actions. |
| **clauDNA** | Engineering workflow behavior: the skills, agents, hooks, and procedures a team uses to do and verify work. |
| **Claudron** | Durable reference knowledge: findings, decisions, and runbooks in portable Markdown vaults. Its integration door is the CLI. |
| **Claudosseum** | Skill evaluation and experimentation. Evaluation results inform improvements; an automatic promotion loop across the whole family is not a promise of current behavior. |
| **Claudfather.ai** | The website experience: accounts, workspaces, navigation, connection metadata, and guidance through the core setup and operating flows. This layer is in development. |

The core projects are independently useful. clauDNA can support an individual coding session, and Claudron can serve a project without a fleet. The website consumes the shared core; improvements to Plane belong in Claudlobby and should benefit direct host access as well.

## Principles

- **Work toward an outcome.** A team exists to advance a declared goal. Activity counts are supporting evidence; useful, reviewed work is the measure.
- **Stay understandable.** Leads communicate plainly. The rigor behind tests, reviews, permissions, and evidence remains intact.
- **Keep running, keep context.** Restart continuity and durable knowledge are essential to a team that works over days. Each release must earn those guarantees through observation.
- **Keep authority on the host.** Operational data, credentials used by the fleet, and access decisions remain installation-driven. Website identity, network reachability, and host permissions are distinct.
- **Preserve local operation.** A website outage must not make the fleet depend on a hosted control service to keep operating. Model providers and external integrations still have their own availability and costs.
- **Make responsibility explicit.** Distinct roles do not imply OS isolation, separate GitHub Apps for every bot, or private per-team permissions. State the boundaries the implementation actually enforces.
- **Improve through evidence.** Capture knowledge, review changes, and evaluate workflows. Describe an integration as working only after its path has been exercised.

## Website and host boundary

The website direction is a workspace that can connect multiple authorized deployments. The same canonical Plane frontend serves the website experience and direct host access. Hosts own private reads and actions; the website is not a proxy or store for operational history.

Tailscale on the host and viewing device is the initial connectivity direction. It supplies reachability, not application permission. Owner pairing, trusted caller verification, current grants, and revocation must be proven before the new website path exposes private host data. Independent direct access is part of the intended outage path.

The open-source core and the privately developed website are separate publishing concerns. The current website preview is synthetic. It has no real account sign-in, connected fleet authority, or live bot actions.

## What earns the next milestone

A person can bring a host, launch a new team, connect an authorized project, receive useful reviewed work, give feedback, and return later with its context intact. This requires evidence through the setup and operating journey on macOS and Linux, alongside the supported laptop and phone access paths.

Intermediate prototypes, passing unit tests, and a hosted page each establish only part of that journey. Current implementation status lives in the owning repositories and their releases and pull requests.

## Scope

We build the tools for teams that run on user-controlled machines. We do not promise hosted bot execution, automatic access to every member of a tailnet, or automatic publication of a user's knowledge. Each repository owns its detailed roadmap and contribution process.

The [organization profile](profile/README.md) is the public introduction. The [brand reference](BRAND.md) keeps naming, visual cues, and product descriptions aligned with the website and the Claudlobby page on crog.gg.
