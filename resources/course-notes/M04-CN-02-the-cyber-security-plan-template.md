# Course Note M04-CN-02 — The Cyber Security Plan Template

**Anchor** — Core / Module 4 · unit 01 *Cyber Security under 10 CFR 73.54* · heading *How industry guidance becomes review guidance*

**Source and locator** — Two sources, with different provenance, which is why this Note is shaped the way it is.

*The rule.* 10 CFR 73.54, "Protection of digital computer and communication systems and networks." [ecfr.gov/current/title-10/section-73.54](https://www.ecfr.gov/current/title-10/section-73.54).

*The guidance.* NEI 08-09, Revision 6, *Cyber Security Plan for Nuclear Power Reactors*, Nuclear Energy Institute, April 2010. Obtainable through the NRC's ADAMS public document system and through the Institute. Cited here by appendix and section number.

**Provenance and use** — The rule: published · public domain (United States government work; excerpted below). The guidance: published · **CHARACTERIZE ONLY**. No text of NEI 08-09 is reproduced in this Note or anywhere on this site. What follows is a description in our own words, with section numbers, written from a copy of the document rather than from secondary description of it.

**Companion** — [M04-CN-03](M04-CN-03-identifying-critical-digital-assets.md) covers the scoping methodology proper. This Note covers the programme the plan template establishes; that one covers how an analyst decides what goes into it. Read them in that order.

---

**Excerpt** — 10 CFR 73.54, bounded to the paragraphs this Note turns on.

> Each licensee currently licensed to operate a nuclear power plant … shall provide high assurance that digital computer and communication systems and networks are adequately protected against cyber attacks, up to and including the design basis threat as described in § 73.1.
>
> (a)(1) The licensee shall protect digital computer and communication systems and networks associated with:
>
> (i) Safety-related and important-to-safety functions;
>
> (ii) Security functions;
>
> (iii) Emergency preparedness functions, including offsite communications; and
>
> (iv) Support systems and equipment which, if compromised, would adversely impact safety, security, or emergency preparedness functions.
>
> (b)(1) [The licensee shall] Analyze digital computer and communication systems and networks and identify those assets that must be protected against cyber attacks to satisfy paragraph (a) of this section.
>
> (e)(1) The cyber security plan must describe how the requirements of this section will be implemented and must account for the site-specific conditions that affect implementation.

Read (a)(1) and (b)(1) together and the division of labour is already visible. The rule names four function categories and imposes an obligation to *identify*. It does not say how to identify. That sentence is the hinge of this Note and the next.

---

**Characterization** — NEI 08-09, Revision 6: what the plan template establishes.

**Two defined terms, in Appendix B.** A *Critical System* is defined functionally: a system associated with or providing the safety, security and emergency-preparedness functions the rule lists, or a support system whose compromise would adversely affect them. A *Critical Digital Asset* is defined as a digital computer, communication system or network that is a component of a Critical System — the definition reaching, expressly, assets that support, protect, or provide a **pathway to** a Critical System — together with support-system assets whose failure or compromise from a cyber attack would adversely affect one of those functions. Criticality is inherited from function; it is never asserted of the technology on its own. What the pathway clause means in practice is not settled in this document, and is the reason the companion guidance exists.

**A two-step funnel, in Appendix A, Section 3.1.3.** The licensee identifies Critical Systems first and then identifies the Critical Digital Assets within each one. For each Critical System examined, the documentation records the digital devices playing direct or supporting roles in its function — protection, control, monitoring, reporting, communications — the assets identified within it, and a description of the consequence to that system and to the regulated functions should one of those assets be compromised.

**A team with a tracing obligation, in Section 3.1.2.** The work is assigned to a Cyber Security Assessment Team drawn from three knowledge domains: digital systems and networks, plant operations and nuclear safety, and physical security and emergency preparedness. The operations member's role is described in terms worth noticing — to trace the impact of a vulnerability outward through plant systems and subsystems until the effect on the regulated functions can be evaluated.

**Validation by walk-down, in Section 3.1.5.** Tabletop review is confirmed physically. Where practical, connections and configuration are inspected directly and communication pathways traced to their termination points; where a physical trace is impractical, electronic validation is substituted with a documented justification, conducted during scheduled outage where there is risk of operational disruption. Interdependencies and trust relationships between assets, and dependencies on infrastructure such as electrical power, environmental control and fire suppression, are examined in the same pass.

**Three dispositions, in Section 3.1.6.** For each asset the licensee either implements the technical, operational and management controls catalogued in Appendices D and E; or implements alternative countermeasures, documenting the basis and an analysis confirming the substitute affords protection at least equal to the control it replaces; or does not implement a control, either by analysis of that specific control for that asset or by documenting that the attack vector is not applicable. A control is also withheld where applying it would itself adversely affect a regulated function, in which case alternates are used. The plan commits the licensee to a *process for reaching and recording those judgements* rather than to a fixed control list.

**A concentric architecture, in Appendix A, Section 4.3.** Defensive levels are separated by boundary devices at which digital communication is monitored and restricted, with the assets requiring the greatest protection sitting behind the greatest number and strength of boundaries. The guidance supplies the shape and requires the licensee to supply the specifics: where its safety and security assets sit, what the boundaries are, what the data-flow rules between levels are, and how those rules are enforced — with a lighter description permitted where a deterministic device enforces the boundary and a fuller one required where a non-deterministic device does.

**Provenance of the control catalogues, in Section 1.1.** Appendices D and E are tailored for nuclear use from NIST SP 800-82, then a final public draft dated September 2008, and NIST SP 800-53, Revision 2.

---

**What it establishes**

The rule sets an objective and an obligation to identify; the guidance supplies the programme; the endorsement makes that programme a yardstick a reviewer can hold an applicant to. That is the architecture of reactor cyber-security licensing, and it explains why a method-level question cannot be answered by reading Title 10 more carefully.

Within it, two properties do most of the work. Criticality flows from function through system to asset, so the analyst is never asked to judge a device on its own merits — which is what keeps the exercise anchored to the licensing basis rather than to a technology inventory. And disposition is analytical: a licensee may substitute or decline a control, and what is reviewable is the documented reasoning, not the mere presence of the control. A cyber security plan is a commitment to a method of judgement.

The construct is also, on its own terms, complete. Every digital asset on a site either falls inside the funnel or is shown not to. There is no category of asset the programme fails to reach.

---

**Where the SMR case departs**

Not by escaping the funnel. That is worth getting right, because the loose way of describing this gap — that campus assets fall outside critical-digital-asset scoping — is wrong, and an applicant who says it will be corrected. The departures are about what the programme records and at what level, not about what it catches.

**"The plant" is the undefined term.** Section 3.1.2 describes tracing a vulnerability outward until its impact on the regulated functions *of the plant* can be evaluated. On a single- or dual-unit site the phrase needs no definition. On a twelve-module campus it has two readings, the module and the campus, and the guidance never chooses because in 2010 it did not have to. Every campus-scaling question below inherits that ambiguity.

**Consequence is recorded per system and never summed.** Section 3.1.3 asks for the consequence to *the* Critical System under examination — one at a time, by construction, since the documentation is organized per Critical System. No field asks what follows when a single compromise takes several Critical Systems simultaneously. This is structurally the same defect Module 3 identifies in the source term: a per-unit demonstration with no aggregation step, carried onto a configuration where aggregation is the whole question. See [Aggregate Inventory](../../core/module-3-consequence-and-source-term/02-aggregate-inventory.md). The parallel is worth putting in front of a reviewer, because it shows the campus problem is one problem appearing in several vocabularies rather than several unrelated complaints.

**The validation regime assumes states a campus does not have.** Walk-downs tracing pathways to termination points, with electronic validation substituted during scheduled outage where disruption is a risk, presume a site that can be taken to a quiet state. A campus with staggered refuelling has no campus-wide outage, and a shared pathway terminates in many places at once. The method does not break here; it multiplies. That makes it a completeness and schedule problem rather than a conceptual one — precisely the kind of finding that arrives late in a review.

**"The attack vector does not exist" is a claim with no stated scope.** Section 3.1.6 permits declining a control on documented non-applicability. On shared architecture, non-applicability is a campus-level assertion: a vector absent at one module may be reachable through a shared path from another. The guidance gives no instruction about the level at which such a disposition is made, and none about re-testing it when the campus grows. On a build-out staged over years, a disposition documented when three modules existed is still relied upon when twelve do. The honest answer today is that this is governed by the licensee's change process rather than by the scoping method, and an applicant should expect to be asked.

**The ceiling is set by the rule, not the guidance.** Appendix A scopes the programme to cyber attacks up to and including the design-basis threat of 73.1. NEI 08-09 is doing exactly what was asked of it, and nothing in it reaches above that boundary — nor should it. This is why [LI-04](../../register/LI-04-state-actor-pre-positioning.md) cannot be closed in the consensus process while [LI-02](../../register/LI-02-campus-scaled-cda-identification.md) and [LI-03](../../register/LI-03-shared-digital-ic-guidance.md) can: industry cannot raise a ceiling the Commission set. Stating that correctly is a matter of fairness to the document as much as accuracy about the gap.

**And the vintage is a live question.** The control catalogues descend from a 2008 draft of NIST SP 800-82 and Revision 2 of NIST SP 800-53. For an operating fleet that lineage is managed through the change process and the periodic programme review. For a first-of-a-kind campus application filed in 2026 it invites a question an applicant should be ready for, and it suggests the campus work [LI-03](../../register/LI-03-shared-digital-ic-guidance.md) asks for may be better framed as a refresh of the guidance than as an appendix bolted to it.

---

**Carry-forward**

The rule says identify; the plan template says what a programme that identifies must contain; and it records consequence one Critical System at a time. What it does not settle is how an analyst decides which assets are in — which is the companion document's job, and where the campus question actually bites.
