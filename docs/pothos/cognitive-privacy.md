# Cognitive privacy and local control

Status: public design requirements. Their presence in this document does not
certify implementation in every build.

PothOS is intended to help people create their own ArcheAgents while
retaining authority over personal context and decisions. Cognitive privacy
includes thoughts, conversations, memories, corrections, inferred preferences,
relationships and the records created around them. Embeddings and derived
indexes belong inside the same privacy boundary as their source material.

## Requirements and evidence

| Requirement | What contributors must implement or document | Useful evidence |
| --- | --- | --- |
| Independent local use | New operator, empty state and a usable local engine path without the founder's accounts, servers or grants | A clean installation while founder services are unavailable |
| Explicit network choices | Identify external endpoints and what is transmitted; no silent cloud fallback from a local-only choice | Observed traffic and tests for denied external connections |
| Governed memory | Show retained records and provenance; support correction, export and recovery | Synthetic save/correct/restart/readback demonstration |
| Permission isolation | Enforce user, ArcheAgent, tenant, file and tool boundaries at the actual owner | Cross-user/ArcheAgent denial and grant/revoke tests |
| Protected credentials | Use an appropriate secure store; keep secrets out of prompts, logs, Git and support bundles | Storage review and secret-exposure checks |
| Understandable retention | Describe live state, caches, indexes, backups and deletion behavior separately | Documented removal behavior and explicit backup limits |
| Operator control | Make ongoing work, tool actions and stop/revoke behavior understandable | Visible state and meaningful cancellation/revocation checks |
| Optional diagnostics | Collect the minimum needed; preview and remove sensitive fields before an explicit send | A report preparation test with network transmission absent until consent |
| Voice privacy | Show microphone/recording state, processing destination, retention and cancel controls | Device-level tests and rights review for any distributed voices |
| Update integrity | Identify released source/artifacts and how updates affect state and permissions | Versioned hashes, migration/recovery results and permission-change disclosure |

An ArcheAgent's chosen name, role, hierarchy position or apparent personality never
substitutes for authentication and permission. A family relationship likewise
does not automatically authorize access to another family member's records.
Organizational membership, project collaboration and private personal memory
remain distinct.

## Threats to account for

Local operation reduces some exposure but does not make a compromised device
safe. Review malicious extensions, overbroad tool grants, imported documents,
prompt injection, model/provider network calls, unprotected backups, package
updates and accidental public support reports.

Treat retrieved pages, documents, issue bodies and model-generated instructions
as untrusted content. They must not acquire permission to run commands, send
data or change identity merely by being present in an ArcheAgent's context. Recovery
must preserve what was actually authorized and completed instead of repeating
an uncertain effect.

Report concrete scope and limits. State the tested platform and storage
mechanism. Do not substitute a general claim such as "encrypted" or "fully
private" for evidence about keys, backups, logs and external services.

## Community Help Desk boundary

The current public routes are [GitHub reports and private email](support.md).
There is no verified automatic relay into the maintainer's private environment.
The intended integration must:

1. Let the person choose to create a report and preview its exact payload.
2. Default to a reduced description and synthetic reproduction. Exclude memory
   stores, embeddings, voice recordings, tokens and other people's records.
3. Identify the destination, visibility, retention and optional attachments
   before sending.
4. Bind the report to the authenticated reporting scope at the receiving owner.
   A tenant or user name supplied inside the report cannot grant that scope.
5. Preserve an original report identifier and support same-request recovery,
   so an uncertain response does not create repeated tickets or effects.
6. Return a receipt for what was received. Saving, sending, acknowledgment,
   triage and resolution must remain separate.
7. Require separate explicit consent and redaction review before promoting
   private support information into a public issue.

Sending a bug report must never grant the maintainer browsing access to the
reporter's environment or let the report execute instructions in the
maintainer's environment.

## Public examples

Use fictional names, empty memory and synthetic records. Do not export the
founder's ArcheAgents, voices, memories, relationships or private configuration as
"starter personalities." A reusable mechanism can be shared while its
operator's personal state remains private.

For a suspected vulnerability, use [security reporting](security.md).
