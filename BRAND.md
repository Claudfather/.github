# Claudfather brand reference

A shared reference for the GitHub organization, Claudfather.ai, project READMEs, and Claudfather project pages on crog.gg. This records the existing direction; it is not a complete product design system.

## Message

**Headline:** Run a fleet of AI workers.

**Supporting line:** Specialist teams on hardware you own. Open-source tools for solo founders and small teams.

Lead with the person's work and the team that helps do it. Explain manifests, runtimes, and protocol details where they help someone take the next step. Describe capabilities plainly, keep jokes light, and distinguish what works now from what is being built.

The established informal signature is **“Rise of the machines. And really bad puns.”** Keep it secondary to the product explanation.

## Names and roles

| Name | Use |
| --- | --- |
| **Claudfather** | Umbrella brand and GitHub organization. |
| **Claudfather.ai** | Website experience; use `claudfather.ai` when referring to the domain. |
| **Claudlobby** | Host composition, setup, permissions, supervision, and operational data. The Python package and CLI are `claudlobby`. |
| **Plane** | Claudlobby's canonical operational interface, shared by hosted and direct access. It is not a separate privately implemented product. |
| **clauDNA** | Engineering workflow skills, agents, and hooks. Preserve this capitalization; the Claude Code plugin identifier is `claudna`. |
| **Claudron** | Durable knowledge in Markdown vaults, integrated through its CLI. |
| **Claudosseum** | Skill evaluation and experimentation. |

crog.gg remains the creator's personal site. Its Claudlobby project page explains this work; the whole site is not a Claudfather property or a replacement product homepage.

## Visual reference

Use the existing robot-in-a-fedora mark. The profile's [mark](profile/assets/claudfather-mark.webp) is reused unchanged from the website preview and matches the crog.gg/GitHub identity. Keep its proportions and provide descriptive alt text; do not redraw it for individual repositories.

The current website shell and Claudlobby project hero use:

| Token | Value | Use |
| --- | --- | --- |
| Charcoal | `#262627` | Brand panels and header backgrounds |
| Cream | `#FAEDD4` | Type on charcoal |
| Orange | `#E5711F` | Brand emphasis and primary actions |
| Ink | `#171717` | Type on orange |

Use orange as an accent. Native GitHub text and surfaces should follow the reader's theme. Operational status needs its own explicit labels and accessible semantic colors; do not turn every state orange to match the brand. The full application palette remains a later design task.

## Links and current claims

- **Get started:** [Claudlobby setup](https://github.com/Claudfather/Claudlobby/blob/main/documentation/getting-started.md). Link to the owning guide instead of copying commands into every surface.
- **Product explanation:** [Claudlobby on crog.gg](https://www.crog.gg/projects/claudlobby).
- **Website development preview:** [claudfather-ai.vercel.app](https://claudfather-ai.vercel.app). Label it synthetic and in development. Do not present the custom domain as launched until it is verified live.
- **Updates:** [Claudlobby releases](https://github.com/Claudfather/Claudlobby/releases).

The core is open source. The website is privately developed; avoid “everything is open source.” Local hosting does not mean every model or connected service runs offline. Distinct bot roles do not establish OS isolation, a separate GitHub App identity for each bot, or private per-team permissions. Arena-driven promotion is an integration to verify, not a blanket claim about every shipped skill.

## Keeping the surfaces aligned

When a product name, primary destination, or capability changes, update this reference, the mission, and the organization profile together. Check the Claudfather.ai shell and the Claudlobby content in crog.gg for the same change, following each repository's own release process. Verify the heading anchors linked from the organization profile whenever a linked repository changes its README. Keep implementation status in the owning repository and link to it; avoid unsourced counts, stale install snippets, and “coming soon” labels on released tools.

Source references: the [Claudlobby project page](https://www.crog.gg/projects/claudlobby), its [content source](https://github.com/chrisrogers37/crog-gg/blob/main/frontend/src/content/claudlobby.ts), and the website preview. Reference refreshed 2026-10-07.
