# Security policy

Claudfather tools can run AI agents on your machine with the credentials you give them. This policy covers Claudlobby, clauDNA, and Claudron, and any other Claudfather project that does not publish its own.

## Report a vulnerability privately

Use GitHub's private vulnerability reporting on the affected repository:

- [Claudlobby](https://github.com/Claudfather/Claudlobby/security/advisories/new)
- [clauDNA](https://github.com/Claudfather/clauDNA/security/advisories/new)
- [Claudron](https://github.com/Claudfather/Claudron/security/advisories/new)

If you cannot use GitHub reporting, email [security@claudfather.ai](mailto:security@claudfather.ai) instead.

Do not open a public issue, pull request, or discussion for a suspected vulnerability. If you are unsure which project is affected, report it to the one you were using; we will route it to the right project.

A useful report includes the affected repository and version or commit, the host operating system, steps to reproduce, and the impact you observed. Remove tokens, chat IDs, and private vault content from anything you share.

## Scope

In scope:

- Code, install scripts, hooks, and default configuration in the projects above, including anything that exposes a host's secrets, operational data, or shell to someone the operator did not authorize.
- Prompt injection: untrusted content, such as an issue, pull request body, web page, message, or vault note, that makes an agent get past a documented guard such as permissions, hooks, allowlists, or secret handling.

Out of scope:

- Access the operator's configuration allows, such as a token's own scope, or any member of a Telegram group the fleet's bots are in. Claudlobby's [safety model](https://github.com/Claudfather/Claudlobby#safety-model) explains these boundaries, including why every group member can instruct a bot.
- Persuading a model to say or do something that crosses no documented guard.
- Vulnerabilities in Claude Code, model providers, or third-party plugins and services. Report those to their maintainers.
- Forks of third-party projects in the Claudfather organization, such as `claude-plugins-official`. Report those upstream.

## Supported versions

The projects are in early alpha. Fixes land on each repository's `main` branch and its next changelog entry; earlier versions are not patched separately.

## What to expect

We aim to acknowledge reports within 7 days. We keep you updated in the private advisory and coordinate disclosure there once a fix is available. We credit reporters in the advisory unless you ask us not to.
