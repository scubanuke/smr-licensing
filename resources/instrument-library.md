# Instrument Library

This is the single source of truth for instrument versions and citable identifiers on this site. Units and register entries cite instruments **by designator without a version number**; the version lives here and only here. That rule exists because version citations scattered through a corpus drift, and this corpus has drifted before.

*Compiled 14 September 2026.*

## How the identifiers work

The package has one **umbrella concept DOI** covering the whole deposit, which resolves to its newest version: **10.5281/zenodo.21430410**. Six instruments additionally carry their own standalone identifier, on a stated criterion: an instrument earns a standalone DOI when it is a freestanding technical basis or methodology that an outside paper or docket could cite without the rest of the package. Package-internal plumbing — a glossary, a request-for-information compilation, a transmittal cover — rides under the umbrella.

A Zenodo record is a deposit of a specific version. Where the working version on this site is ahead of the deposited one, the table says so, and the DOI still resolves to what was deposited.

## Core design basis

| Designator | Instrument | Version | Identifier |
|---|---|---|---|
| **B1** | DBA-MA-SMR-FC1 — SMR facility-class design basis | v0.9 working | [10.5281/zenodo.21894261](https://doi.org/10.5281/zenodo.21894261) *(deposited at v0.8)* |
| **B2** | DBA-MA-ST — source term under military action | v0.1 | umbrella |
| **B3 / TB1** | Multi-module coping adequacy technical basis | v0.1 | [10.5281/zenodo.21894606](https://doi.org/10.5281/zenodo.21894606) |
| **B4** | DBA-MA-DiD — defense in depth under military action | v0.1 | umbrella |
| **B5** | Command Broker nuclear annex | v0.3 working | umbrella |

B1 is the instrument under review; the other four are inherited, which is what makes them core rather than supporting. B1 does not redefine them, it names them.

## Orientation and transmittal

| Designator | Instrument | Version |
|---|---|---|
| **00A** | Reviewer's Guide and transmittal map | v0.2 |
| **00B** | Cover letter and transmittal | v0.2 |
| **A1** | DBA-MA introduction | v1.12 working |
| **A2** | United States Level 1 regulatory case | v2.6 |

## Supporting instruments

| Designator | Instrument | Version |
|---|---|---|
| **C1** | Use case 1 — spent fuel pool thermal progression | v1.0 |
| **C2a** | DBA-UxS — uncrewed systems, cross-sector parent | v1.1 |
| **C2b** | DBA-MA-UxS-NA — nuclear annex | v1.1 |
| **C3a** | United States Level 2 — accident description | v1.0 |
| **C3b** | United States Level 3 — trigger framework | v1.0 |
| **C3c** | United States Level 4 — monitoring guidance | v1.0 |
| **C4** | DBA-MA transition architecture | v1.0 |
| **C5a** | DBA-MA-PPA — physical proximity attack | v1.1 |
| **C5b** | Three threads of cyber security | v1.1 |
| **C6** | Tiered assessment framework — nuclear sector application guide | v0.3 working |
| — | DBA-MA-SITE — geopolitical siting methodology | v0.5 |

## Candidate work products

Twelve, from the submittal development plan's menu, all drafted. Tier 1 closes the two Commission-directed findings; Tier 2 supplies standard submittal components; Tier 3 strengthens the technical case.

| Designator | Work product | Version | Identifier |
|---|---|---|---|
| **1A** | Counter-UAS Part 73 reframing | v0.1 | umbrella |
| **1B** | Campus cyber-security gap closure path | v0.1 | umbrella |
| **2A** | Topical-report wrapper and conformance matrix | v0.1 | umbrella |
| **2B** | Requirements-traceability matrix | v0.1 | umbrella |
| **2C** | Anticipated requests for additional information | v0.1 | umbrella |
| **2D** | Glossary, acronyms and reference index | v0.1 | umbrella |
| **2E** | Classification and docket-handling plan | v0.1 | umbrella |
| **3A** | Reduced emergency planning zone — technical basis | v0.1 | [10.5281/zenodo.21894508](https://doi.org/10.5281/zenodo.21894508) |
| **3B** | Formal-methods verification and validation methodology | v0.1 | [10.5281/zenodo.21894692](https://doi.org/10.5281/zenodo.21894692) |
| **3C** | Risk-informed / PRA bridge | v0.1 | [10.5281/zenodo.21894740](https://doi.org/10.5281/zenodo.21894740) |
| **3D** | Military threat coordination protocol | v0.2 | [10.5281/zenodo.21895916](https://doi.org/10.5281/zenodo.21895916) |
| **3E** | ACRS briefing summary | v0.1 | umbrella |

## Anticipated and not yet written

Named in the corpus and not drafted: a campus consequence-trace use case; a spent-fuel use case for this facility class; and the under-frequency load shedding position paper that [LI-14](../register/LI-14-under-frequency-load-shedding.md) records.

## A standing note on currency

The assembled review package holds its own copies of several instruments at the versions current when it was assembled, and the working copies have since moved ahead — B1 most notably. This is normal for a package that is version-controlled as a set, and it is also exactly how stale citations propagate. When this site and the package disagree, this table is what the site means.
