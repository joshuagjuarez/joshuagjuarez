# Open development: status and help wanted

**Current direction:** read the [PothOS community hub](../../POTHOS.md) and
[November 6 release-policy clarification](community-release-policy.md).
Prospective runtime terms are under review; existing documentation licenses remain effective.

Observed release state: November 6, 2026. This is a contribution map, not a
promise of completion dates or universal compatibility.

## What is available

Public documentation and design source are available under the scoped
[documentation license](LICENSE_SCOPE.md). The invited hosted beta and its
connection kit remain available through the [existing entry points](installation-and-updates.md).
The connection kit is not a standalone local runtime.

## Gaps contributors can help close

| Area | Current public qualification | Useful contribution | Evidence needed to change status |
| --- | --- | --- | --- |
| Independent source distribution | Complete runtime export not published | Review dependency closure, remove required private bindings, prepare a reproducible clean export | Rights/privacy-reviewed source, exact manifest and component or application build result |
| Own ArcheAgent identity and hierarchy | Design documented; independent public implementation not qualified | Clarify durable identity, customizable responsibilities and explicit permissions | New-operator/ArcheAgent setup, hierarchy changes and denial tests without inherited founder state |
| Memory continuity | Central project purpose; standalone public recovery not demonstrated | Document storage/provenance, correction and recovery paths; create synthetic fixtures | Same-record save/correct/restart/recover result with version identity |
| Local model support | No universal local-model compatibility claim | Add and qualify optional adapters within the existing application architecture | Exact model/runtime/hardware/version and real task results |
| Cognitive privacy | Requirements published; configuration-specific evidence pending | Inspect data paths, network defaults, retention and support payloads | Local-only network test, isolation checks and truthful limitations |
| Voice and accessibility | Native implementations exist; public packaging and device acceptance pending | Separate generic voice interfaces from private profiles; test permissions, recording controls and accessibility | Source/asset rights plus real microphone/speaker and cancellation tests per supported platform |
| Community Help Desk | Public email and GitHub reporting available; automatic private-stack intake unverified | Design a consent-based, reduced-data report path using existing support owners | Authenticated scope, original-ID recovery, receipt and redaction/publication tests |
| Free hosted access | Web client no longer initiates new paid activation; native account migration pending | Complete actual free membership and recurring-billing migration through account owners | Real account and payment-provider receipts; no weakened tenant checks |
| Platform packages | Customer distribution requires platform-specific qualification | Reproducible build/install/update documentation for a named configuration | Actual artifacts, installation, migration and recovery results |
| Purpose Link applications | Separate community-resource application; broader integration is a goal | Scoped accessibility, multilingual and local-community prototypes with synthetic data | Partner-defined needs, separate data custody and a working permitted integration |

Developers can contribute useful documentation and design review now. Source
contributions become possible for each reviewed component as it is published.
A safe developer source preview can be incomplete; it must identify its actual
contents and limitations. It does not need to wait for every planned feature,
and it must not be advertised as a finished standalone system.

## Contribution shape

Choose one concrete problem, state the person affected and the desired
behavior, identify the relevant public source, and describe the evidence that
would demonstrate improvement. Preserve existing identities and permission
boundaries. Keep private data out of issues, pull requests and test fixtures.

Use the [contribution guide](contributing.md) and [support routes](support.md).
The maintainer will update status as work is actually reviewed and released.
