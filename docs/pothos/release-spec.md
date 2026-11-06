# PothOS public release specification

**Current direction:** read the [PothOS community hub](../../POTHOS.md) and
[November 6 release-policy clarification](community-release-policy.md).
Prospective runtime terms are under review; existing documentation licenses remain effective.

Version: November 6, 2026. Status: public documentation and design source.
This specification records the release direction and acceptance evidence required
for each stage. It does not certify an unpublished runtime.

## Purpose and product boundary

PothOS is being opened so people can create their own **ArcheAgents**:
continuing digital representatives with identities, memory continuity and
responsibilities chosen by their operators. ArcheAgents may have customizable roles,
hierarchies and interfaces. The person remains the authority over their
environment.

The reusable framework is the public product. The founder's existing ArcheAgents,
personalities, private voices, memories, relationships and operating environment
are excluded. A new installation must initialize a new operator and empty state.
It must not inherit the developer's accounts, identity, permissions or network.

PothOS software is $0 for individuals and organizations, including businesses.
Its official public software distribution is to remain free. Hardware, optional
hosting, third-party models and paid external services have their own costs and
licenses. Prospective runtime terms are being reviewed under the
[current release policy](community-release-policy.md).

## Release stages

Incomplete software can be useful to contributors. The stage must describe the
actual contents and what they can do.

| Stage | Contents | Required evidence and permitted claim |
| --- | --- | --- |
| Public design source | This README, specification, privacy requirements, roadmap and contribution material | Public files and their scoped license can be read and reused. No runtime installation is claimed. |
| Developer source preview | Reviewed reusable components, relevant tests, dependency manifests and build instructions | File-level rights and privacy review; exact source commit; component-level setup and limitations. Publish useful cleared components without waiting for every product feature. State plainly when they cannot run the complete product. |
| Standalone beta | A coherent local distribution with ArcheAgent identity, basic continuity, permissions and a tested engine path | Clean installation without founder services, one real task, save/restart/recovery, documented network behavior and permission tests. Incomplete optional features remain labeled. |
| Broader platform release | Additional platform packages, adapters, voice paths and migrations | Evidence for each named platform/version; appropriate signing and distribution qualification where applicable. |

The current published stage is public design source. The existing invited web
beta and connection kit are separate deliverables. A plugin, workflow archive,
hosted interface or documentation set must not be described as a complete local
runtime.

## What belongs in the public project

| Publish after review | Keep private |
| --- | --- |
| Generic ArcheAgent identity and role mechanisms | The founder's ArcheAgent roster, personas, personal rules and private relationship history |
| Memory storage interfaces, provenance, correction and recovery mechanisms | Actual memories, conversations, embeddings, search indexes and database contents |
| Permission enforcement, configurable hierarchies and isolation tests | Working credentials, membership grants, access tokens and private tenant maps |
| Local runtime adapters and documented optional integrations | Personal accounts, private endpoints, machine inventory and account-specific bindings |
| Generic voice interfaces and rights-cleared assets | Private voiceprints, voice samples, microphone recordings and personalized voice assets |
| UI, CLI, documented protocols, build files and dependency notices | Personal/family, customer and separate-venture records |
| Synthetic examples and minimal reproducible fixtures | Screenshots, telemetry, logs or backups containing real private material |
| Public roadmap, contribution policy and release evidence | Private Git history, branches, LFS objects, issue exports and CI/release artifacts |

Use an exact reviewed file allowlist and a clean public Git history. Deleting a
secret from the latest file or adding it to an ignore file does not remove old
copies. Review generated bundles, source maps, archives and dependency assets too.
If a needed component cannot be released, remove its required dependency or mark
the affected functionality unavailable.

## ArcheAgent identity, memory and authority

The design separates these concerns:

| Concern | Required behavior |
| --- | --- |
| ArcheAgent identity | A durable identifier and user-defined name, purpose and characteristics survive supported restarts and engine changes. |
| Engine/session | A replaceable execution binding. The model name or current chat is not the ArcheAgent's identity or complete memory. |
| Memory continuity | Stored records retain source, corrections and relevant time information. The operator can inspect and recover the state that actually exists. |
| Role/hierarchy | Responsibilities and coordination chosen by the operator. A hierarchy position does not grant access by itself. |
| Permission | Explicit, scoped grants enforced by the actual file, tool, account or service owner, with revocation and failure behavior. |
| Human decision | The operator can pause, inspect and stop work. Protected decisions and new access remain with the authorized person. |

Synthetic examples may illustrate a study ArcheAgent and a project ArcheAgent coordinated by a
user-chosen companion. They must start with empty memory and no working account
grants. Examples must identify whether they are illustrative design or executable
configuration for a particular released version.

## Minimum standalone-beta demonstration

Record the exact source commit, artifact hash, operating system, hardware,
interpreter, model/runtime versions and commands actually used.

1. Install into an empty environment with the developer's services unavailable.
2. Create a new operator and a new ArcheAgent with a user-chosen identity and role.
3. Run one useful task through a documented local engine. Record any network
   traffic; a local-only selection must not silently fall back to a cloud service.
4. Save a synthetic memory with its source, correct it, restart the application,
   and recover the same ArcheAgent identity and the expected current record.
5. Demonstrate that another ArcheAgent, user or tenant cannot read that record without
   an explicit permitted connection.
6. Grant and revoke a bounded tool permission. A revoked or absent grant must
   prevent the protected operation.
7. Export and recover operator data through the documented mechanism. Explain
   deletion and backup limitations rather than claiming universal erasure.
8. Check that a private support request can be prepared without automatically
   uploading memory, credentials or recordings.

These are focused acceptance examples, not proof of security against every
threat. Review [cognitive privacy](cognitive-privacy.md) for further requirements.

## Voice and device qualification

Native voice work already exists in the project. Public release work includes
separating reusable interfaces from private profiles, reviewing asset rights,
documenting on-device versus external processing, permission prompts, recording
indicators, cancellation and retention, and testing actual microphone/speaker
behavior on each supported device.

Do not infer that a hosted browser stub establishes native voice behavior, or
that a successful build proves physical audio operation. Publish a capability
table with verified, experimental, planned and unavailable states.

## Repository and release contents

A developer source preview should include a clear README, scoped license,
third-party notices, architecture, actual setup/test commands, known gaps,
contribution and security guidance, and exact source/version identity. Include a
dependency inventory appropriate to what is distributed.

A standalone beta additionally needs its tested installation and recovery path,
versioned artifacts and checksums, supported configuration table, migration
notes and observed privacy/network behavior. Verify public read/clone/download
from outside the maintainer's account.

Apache-2.0 currently applies only to the documentation and templates enumerated
in [LICENSE_SCOPE.md](LICENSE_SCOPE.md). The runtime license must be applied to
the actual rights-reviewed export. Preserve all third-party license obligations;
project branding and private identities are separate from code licensing.

## Community feedback and project decisions

Public documentation contributions and reduced engineering reports can start
now through the [contribution guide](contributing.md) and
[support guide](support.md). Automatic community Help Desk intake into the
maintainer's private environment is a separate, unverified integration.

The initial maintainer reviews official project changes and release claims.
Contributors retain their rights under the applicable license. Proposals,
merged source, published packages and tested installations are distinct states.
Record substantive architecture and privacy decisions so contributors can
understand why a change was accepted.

Social benefit, accessibility and personal sovereignty guide the project.
The prospective runtime policy is being defined separately from the
existing documentation license. [Purpose Link](purpose-link.md) is a separate
application of the broader mission.

See the [roadmap](roadmap.md) for current gaps and useful contribution areas.
