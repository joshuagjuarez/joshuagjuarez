# Installation and updates

## Available entry point

Start at [pothos.joshops.ai](https://pothos.joshops.ai) with your own account.
The [availability page](https://joshops.ai/docs) identifies which interfaces are
open to customers. As of 3 November 2026, native customer store packages have not
been published. Internal development installations are not public downloads.

## One product across devices

The master app means the shared PothOS product and its capabilities. Each operating
system receives a compatible build. Installing on a second device should let you
sign into the same permitted account; it does not copy somebody else's account,
credentials or private workspace.

Customers do not need the founder to connect to their device through Xcode.
The native distribution work targets these ordinary delivery paths:

| Interface | Intended delivery and update path |
| --- | --- |
| Web | Sign in to the hosted app; services and web assets are updated centrally. |
| iPhone and iPad | App Store installation and updates after review. TestFlight is for prerelease testing. |
| Mac | Signed and notarized download with signed app updates, or an approved Mac App Store release. |
| Android | Google Play installation and updates after release qualification. |
| Windows and Linux | Platform packages and a verified update channel after qualification. |

These native paths are release work, not a claim that all packages are available
today. The download page must identify the platform, version and release channel.

## Your account and connections

PothOS account access, subscription entitlement, device enrollment and external
provider connections are separate checks. A provider connection requests selected
permissions and can be disconnected. Private credentials belong in the appropriate
secure credential store, outside conversation history and public repositories.

GitHub and Tailscale accounts are not prerequisites for the browser entry.
Optional developer or fleet connections may need their own authorization. A
PothOS account does not automatically enroll a device in the founder's private
network or grant access to another person's devices.

## Source updates versus installed updates

A pull request proposes a source change. A release process checks it, builds the
platform packages, signs them and publishes an eligible version. The app store or
approved updater then delivers that version. Customer devices should never have
to compile the repository to receive an ordinary update.

This is the release model being completed for PothOS. For present access or an
installation problem, use [support](support.md).
