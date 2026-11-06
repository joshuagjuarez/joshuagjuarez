# Contributing to PothOS

**Current direction:** read the [PothOS community hub](../../POTHOS.md) and
[November 6 release-policy clarification](community-release-policy.md).
Prospective runtime terms are under review; existing documentation licenses remain effective.

PothOS welcomes people who want to make personal AI more useful, understandable,
accessible and accountable to its operator.

**ArcheAgent** is the product term. Use **ArcheAgents** in the plural.
Preserve PothOS and PothOS Orb naming. The public framework is for users to
create their own ArcheAgents; the founder's private ArcheAgents and personal state are not
public fixtures.

## What you can contribute now

This repository currently publishes documentation and design source, not the
complete runtime. Documentation corrections, accessibility feedback, privacy
review, architecture questions and reduced reproducible reports are welcome.
See [the roadmap](roadmap.md) for bounded work areas.

Use [public GitHub issues](https://github.com/joshuagjuarez/joshuagjuarez/issues)
for nonprivate engineering discussion and pull requests for proposed changes.
Use [private support](support.md) for account, billing or confidential concerns.
An issue is public; never paste a memory export or personal case record into it.

## A useful proposal

Explain who encounters the problem, what happens, what should happen, and how
the proposed change could be checked. Link the relevant public file or version.
Search existing issues before creating a duplicate. Use a small synthetic
example instead of a real person's data.

For changes to ArcheAgent identity, memory, permissions, hierarchies, public interfaces
or network behavior, explain the data flow and authority boundary. Discuss
substantial changes before replacing an existing mechanism. Role names and
hierarchy positions must never become implicit grants.

## Pull requests

Keep one bounded problem per change and preserve unrelated work. Explain the
resulting behavior, tests or checks actually performed, and remaining limits.
For documentation, check links, terminology and the distinction between a
design requirement and verified behavior.

When runtime components become public, follow their actual build instructions.
Include the exact platform/runtime/model versions and commands used where
relevant. A successful adapter test does not establish support for every model
or device. Never report an execution that was not performed.

Do not commit credentials, tokens, session cookies, real memories, embeddings,
voice recordings, tenant records or private machine configuration. Preserve
third-party notices and contribute only material you have the right to share.
The [scoped documentation license](LICENSE_SCOPE.md) describes the current
published material. Runtime contribution terms will accompany the actual
runtime release; this guide does not relicense private or third-party code.

## Review and project governance

Joshua Gustafson-Juarez is the initial project maintainer. Official project
releases and substantive architecture decisions are recorded by the maintainer
and designated reviewers. Contributors are welcome to propose improvements;
contribution does not grant access to private systems or appoint a project role.

Accepted source, a published package, a successful installation and an adopted
design decision are separate outcomes. Release notes should make those
distinctions visible. Use reproducible evidence and respectful technical
discussion. Do not harass others or expose their private information.

Response times, acceptance and release dates depend on capacity. The project
does not promise unlimited individual support. Report vulnerabilities through
[security reporting](security.md).
