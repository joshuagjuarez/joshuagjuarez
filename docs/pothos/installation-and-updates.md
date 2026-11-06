# Installation and updates

## Open-source beta status

The [public design, AA charter and release specification](README.md) are available
now under the [scoped documentation license](LICENSE_SCOPE.md). They do not
contain a standalone runtime installer.

The standalone open-source PothOS beta is being prepared. Its public repository,
license, supported platforms and verified installation commands will be published
together when the release is ready. This guide does not yet offer a complete
self-hosted installer.

PothOS software is **free, always**, including personal, nonprofit and commercial
use. There is no charge per ArcheAgent, device or seat. Hardware, optional hosting,
AI-provider subscriptions, metered APIs and model licenses are separate.

## Current hosted entry point

The existing [PothOS web beta](https://pothos.joshops.ai) requires an invitation
and your own account. Free-access migration is in progress. If an older screen
still requests payment for PothOS software, use [support](support.md) rather than
starting a new paid subscription.

The [download page](https://joshops.ai/download) identifies currently available
artifacts. The connection kit contains plugin source, setup instructions and host
configuration examples. It does not contain the standalone native runtime,
model weights or a model installer.

Native customer packages and store distribution remain subject to their actual
release qualification. Internal development installations are not public
downloads.

## Independent local installations

The open-source release is being prepared to start with empty user state and to
use the operator's own hardware, model runtime and explicitly selected services.
It must not require the developer's account, server, credentials, private network
or personal workspace.

Installation instructions must identify supported operating systems, architecture,
runtime and dependency versions, the exact tested commands, and known limits.
A working connection on one model or host is not proof that every local AI is
compatible.

## One product across supported devices

Each operating system needs a compatible build. Installing on a second device
must preserve the operator's chosen account and scope without copying someone
else's credentials or workspace.

| Interface | Intended delivery and update path |
| --- | --- |
| Web | Existing invited hosted beta; account and service scope apply. |
| Local source | Public source, license and verified build/run instructions when the beta is released. |
| iPhone and iPad | App Store or TestFlight only after the relevant distribution qualification. |
| Mac | Signed and notarized release or approved store distribution after qualification. |
| Android | Google Play or a documented verified package after release qualification. |
| Windows and Linux | Platform packages and a documented update channel after qualification. |

These native paths are release work. They do not claim that every package is
available today.

## Accounts, permission and updates

Free access removes the PothOS software payment requirement. It does not grant
access to another person's data, a private hosted service, an administrator role
or a device. Released configurations must document credential storage and keep
credentials outside conversation logs and public repositories.
Configuration-specific storage evidence is still pending.

A pull request proposes a source change. A release checks the selected source,
builds the artifacts and publishes versioned installation and update guidance.
Source availability, package availability and a successful installation are
distinct facts. Use the release notes for the actual supported path.
