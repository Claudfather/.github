# Security policy

Claudfather tools run AI agents on your machine with the credentials you give them, so we treat security reports as a priority. This policy applies to every public Claudfather repository that does not publish its own.

## Report a vulnerability privately

Use GitHub's private vulnerability reporting on the affected repository:

- [Claudlobby](https://github.com/Claudfather/Claudlobby/security/advisories/new)
- [clauDNA](https://github.com/Claudfather/clauDNA/security/advisories/new)
- [Claudron](https://github.com/Claudfather/Claudron/security/advisories/new)

Do not open a public issue, pull request, or discussion for a suspected vulnerability. If you are unsure which repository is affected, report it to the one you were using; we will move it.

A useful report includes the affected repository and version or commit, the host operating system, steps to reproduce, and the impact you observed. Remove real tokens, chat IDs, and vault contents from logs before you attach them.

## Scope

In scope: code, install scripts, hooks, and default configuration in the public Claudfather repositories, including anything that exposes a host's secrets, operational data, or shell to someone the operator did not authorize.

Out of scope:

- Access an operator explicitly granted, such as a token's own scope or the members of a Telegram group the fleet accepts. Claudlobby's [safety model](https://github.com/Claudfather/Claudlobby#safety-model) describes those boundaries.
- Vulnerabilities in Claude Code, model providers, or third-party plugins and services. Report those to their maintainers.

## Supported versions

The projects are in early alpha. Fixes land on each repository's `main` branch and its next changelog entry; earlier versions are not patched separately.

## What to expect

A small team maintains these projects. We acknowledge reports as soon as we can, keep you updated in the private advisory, and coordinate disclosure there once a fix is available. We credit reporters in the advisory unless you ask us not to.
