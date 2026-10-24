# Claudfather brand reference

A shared reference for the GitHub organization, Claudfather.ai, project READMEs, and the Claudfather project page on crog.gg. This records the existing direction; it is not a complete product design system.

## Message

**Headline:** Run a fleet of AI workers.

**Supporting line:** Specialist teams on hardware you own. Open-source tools for solo founders and small teams.

Lead with the person's work and the team that helps do it. Explain manifests, runtimes, and protocol details where they help someone take the next step. Describe capabilities plainly, keep jokes light, and distinguish what works now from what is being built.

The tagline is **“Rise of the machines”**. Keep it secondary to the product explanation.

## Names and roles

| Name | Use |
| --- | --- |
| **Claudfather** | Umbrella brand and GitHub organization. |
| **Claudfather.ai** | Website experience; use `claudfather.ai` when referring to the domain. |
| **Claudlobby** | Host composition, setup, permissions, supervision, and operational data. The Python package and CLI are `claudlobby`. |
| **Plane** | Claudlobby's canonical operational interface, shared by hosted and direct access. It is not a separate privately implemented product. |
| **clauDNA** | Engineering workflow skills, agents, and hooks. Preserve this capitalization; the Claude Code plugin identifier is `claudna`. |
| **Claudron** | Durable knowledge in Markdown vaults, integrated through its CLI. |

crog.gg remains the creator's personal site. Its Claudfather project page explains this work; the whole site is not a Claudfather property or a replacement product homepage.

## Visual reference

Use the existing robot-in-a-fedora mark. The profile's [mark](profile/assets/claudfather-mark.webp) is reused unchanged from the website and matches the crog.gg/GitHub identity. Keep its proportions and provide descriptive alt text; do not redraw it for individual repositories.

The canonical palette matches the GitHub organization mark and the Claudfather project page on crog.gg:

| Token | Value | Use |
| --- | --- | --- |
| Charcoal | `#262627` | Brand panels and header backgrounds |
| Cream | `#FAEDD4` | Type on charcoal |
| Orange | `#E5711F` | Brand emphasis and primary actions |
| Ink | `#171717` | Type on orange |

Use orange as an accent. Native GitHub text and surfaces should follow the reader's theme. Operational status needs its own explicit labels and accessible semantic colors; do not turn every state orange to match the brand. The full application palette remains a later design task.

claudfather.ai currently uses slightly different values (charcoal `#252725`, orange `#DC742A`, ink `#282B27`). Bring the website to this palette, not the reverse.

## Links and current claims

- **Get started:** [Claudlobby setup](https://github.com/Claudfather/Claudlobby/blob/main/documentation/getting-started.md). Link to the owning guide instead of copying commands into every surface.
- **Product explanation:** [Claudfather on crog.gg](https://www.crog.gg/projects/claudfather). The older `/projects/claudlobby` path redirects there; link the current path.
- **Website:** [claudfather.ai](https://claudfather.ai). Describe it as in private development: no sign-up, waitlist, or public demo. Do not present it as launched until public sign-up is verified live. The [Vercel deployment](https://claudfather-ai.vercel.app) serves the same visitor page; prefer the domain.
- **Updates:** each project's changelog: [Claudlobby](https://github.com/Claudfather/Claudlobby/blob/main/CHANGELOG.md), [clauDNA](https://github.com/Claudfather/clauDNA/blob/main/CHANGELOG.md), [Claudron](https://github.com/Claudfather/Claudron/blob/main/CHANGELOG.md). clauDNA and Claudron also publish GitHub releases; Claudlobby does not yet, so do not link its releases page.

The core is open source. The website is privately developed; avoid “everything is open source.” Local hosting does not mean every model or connected service runs offline. Distinct bot roles do not establish OS isolation, a separate GitHub App identity for each bot, or private per-team permissions.

## Keeping the surfaces aligned

When a product name, primary destination, or capability changes, update this reference, the mission, and the organization profile together, along with `SECURITY.md` and `CONTRIBUTING.md` where they name projects. Check the Claudfather.ai shell and the Claudfather content in crog.gg for the same change, following each repository's own release process. Verify the heading anchors linked from the organization profile whenever a linked repository changes its README. When a repository is made private (public visitors then get a 404) or archived, remove it from the profile, the mission, this reference, `SECURITY.md`, and `CONTRIBUTING.md` in the same change. Keep implementation status in the owning repository and link to it; avoid unsourced counts, stale install snippets, and “coming soon” labels on released tools.

Source references: the [Claudfather project page](https://www.crog.gg/projects/claudfather), its [content source](https://github.com/chrisrogers37/crog-gg/blob/main/frontend/src/content/claudfather.ts), and [claudfather.ai](https://claudfather.ai). Reference refreshed 2026-10-24.
