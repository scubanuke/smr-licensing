# Glossary

Plain-language first, precise second. Where a term has a regulatory definition, the regulation governs and the [Regulatory Index](regulatory-index.md) points at it.

**ACRS — Advisory Committee on Reactor Safeguards.** An independent committee that reviews the staff's safety conclusions and reports to the Commission. It can and does disagree with the staff, which is the point of it.

**Aggregate inventory.** The total radioactive material on a site rather than in one reactor. The distinction is central to [LI-06](../register/LI-06-aggregate-inventory-in-the-epz-demonstration.md).

**Applicant.** The party asking for permission to build or operate. Becomes the licensee if permission is granted.

**ASSC — autonomous safe shutdown condition.** A state the plant can reach and hold without operators and without off-site power. How long it can hold is the coping duration.

**Bright Line.** In this corpus, the boundary that artificial intelligence may not cross into safety-critical action. **The term is reserved for that autonomy boundary and is not used for the intent boundary** between the design-basis threat and the state-actor layer, which is a different distinction discussed in Module 4.

**CDA — critical digital asset.** Digital equipment whose compromise could adversely affect safety, security or emergency preparedness, and which therefore receives the highest level of cyber protection.

**Command Broker.** The mechanism governing the autonomy boundary: it holds an artificial-intelligence system inside a bounded, deterministic envelope under denial conditions, provides an independent hardware reset, and fails to a safe default when it cannot arbitrate.

**Conditionality Check — Consequence-Basis Conditionality Check.** Three steps: declare the barriers a consequence relaxation credits, test each against the four characteristics of deliberate action, and state the residual. Its purpose is to stop a relaxation earned against accidents from being silently assumed to hold against an adversary.

**Conformance matrix.** A requirement-by-requirement table: the provision, the obligation, where the record addresses it, and how it conforms. The spine a Safety Evaluation is built on.

**Coping duration.** How long a plant can hold itself safe without operator action or power. The industry floor is seventy-two hours; designs claim more. For a campus, see [LI-07](../register/LI-07-assc-duration-on-aggregate-demand.md).

**Correlated-barrier cutset.** A set of barriers that a single deliberate act can defeat together, because they share supports, bays, feeds or paths. Redundancy protects against independent failure; a cutset is what defeats it.

**Credible input domain.** The set of inputs a safety-relevant artifact could physically encounter — the realizable sensor space, not every mathematically possible input. Bounding and declaring it is one of the four conditions in the admissibility gate of [LI-09](../register/LI-09-ml-provenance-safety-logic.md).

**DBA — design basis accident.** The set of postulated accidents a plant must be designed to withstand. **DBA-MA** extends the same discipline to deliberate military action.

**DBT — design-basis threat.** The adversary a licensee must be able to protect against, defined by the Commission in 10 CFR 73.1. It bounds licensee obligation; it is not a prediction of what could happen.

**Derivative.** A site-specific instrument descending from a class-level one. Derivatives carry the detail that is designated before docketing; see [LI-12](../register/LI-12-public-docket-and-safeguards-split.md).

**Docket.** The official record of a licensing proceeding. Mostly public, which is what makes public participation possible.

**Dual design basis.** A facility where artificial intelligence participates has two design bases — the facility-class basis and the artificial-intelligence basis — sharing a consequence root and diverging on the adversary envelope, with the Bright Line as the seam.

**EPZ — emergency planning zone.** The area around a plant where protective actions are planned in advance. It is a planning boundary, not a danger line.

**Facility class.** A category of facility sharing a consequence profile and a barrier set, for which one design basis can be written. The small modular reactor class is the first facility class in this corpus.

**Four characteristics of military action.** Intentionality, persistence, precision and denial — the properties that distinguish a deliberate adversary from an accident, and the tests a barrier is checked against in the Conditionality Check.

**GDC — General Design Criteria.** The minimum design requirements of 10 CFR Part 50 Appendix A.

**Mechanistic source term.** A calculated account of what would be released and when, based on the actual barriers of a specific design, rather than a prescribed fraction.

**PAG — protective action guideline.** The projected dose at which a protective action becomes warranted. The early-phase guideline is one rem, set by the Environmental Protection Agency.

**Proximity coupling.** A favorable source term permits a smaller planning zone, a smaller zone permits siting nearer to population, and so the population exposed to the adversarial residual is nearer than it would otherwise have been. Stated openly in the corpus rather than elided.

**RAI — request for additional information.** A formal question from the staff to the applicant during review. Volume of RAIs is usually the real schedule risk.

**Residual.** What remains unprotected after the credited barriers have been tested against deliberate action. The Conditionality Check exists to make it explicit rather than implicit.

**Safeguards Information.** A protection category under 10 CFR 73.21 and 73.22 for security-sensitive material that is not classified but is withheld from the public record.

**Source term.** How much radioactive material could be released in a given scenario. The first link in the chain that ends at a planning zone.

**Topical report.** A document reviewed once on its own merits and, if found acceptable, referable by later applicants. The mechanism that makes first-of-a-kind regulatory effort an asset rather than a sunk cost.

**Tearline.** A version of an intelligence product carrying the conclusion without the sources. The mechanism that lets a warning be shared with a party that cannot see how it was derived.
