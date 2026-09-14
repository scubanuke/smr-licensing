# Course Note M04-CN-01 — The Safety/Security Interface

**Anchor** — Core / Module 4 · unit 00 *The Design-Basis Threat and Physical Protection* · heading *The safety and security interface*

**Source and locator** — 10 CFR 73.58, "Safety/security interface requirements for nuclear power reactors." [ecfr.gov/current/title-10/chapter-I/part-73/section-73.58](https://www.ecfr.gov/current/title-10/chapter-I/part-73/section-73.58). Source note: 74 FR 13987, 27 March 2009, as amended at 91 FR 15871, 30 March 2026.

**Provenance and use** — Published · public domain (United States government work; reproduced in full)

---

**Excerpt**

> **§ 73.58 Safety/security interface requirements for nuclear power reactors.**
>
> (a) Each operating nuclear power reactor licensee with a license issued under part 50, part 52, or part 53 of this chapter shall comply with the requirements of this section.
>
> (b) The licensee shall assess and manage the potential for adverse effects on safety and security, including the site emergency plan, before implementing changes to plant configurations, facility conditions, or security.
>
> (c) The scope of changes to be assessed and managed must include planned and emergent activities (such as, but not limited to, physical modifications, procedural changes, changes to operator actions or security assignments, maintenance activities, system reconfiguration, access modification or restrictions, and changes to the security plan and its implementation).
>
> (d) Where potential conflicts are identified, the licensee shall communicate them to appropriate licensee personnel and take compensatory and/or mitigative actions to maintain safety and security under applicable Commission regulations, requirements, and license conditions.

Four paragraphs is the entire section. Its brevity is part of what it establishes.

---

**What it establishes**

Three things, inside its own domain and on its own terms.

That a seam between two independently-correct programmes is a hazard in itself. Safety and security are each evaluated against their own criteria, and 73.58 exists because both can be individually satisfied while the combination is worse than either — a barrier sited where it impedes an access route the accident analysis credits, a locking regime that slows a response the safety case assumes.

That the remedy is to **make the interface itself a governed object**, with a named owner and an obligation that bites at a specific moment. Paragraph (b) attaches the duty to the point *before implementing* a change, which is what makes it enforceable rather than aspirational.

And that the scope is deliberately broad and non-exhaustive. Paragraph (c)'s "such as, but not limited to" list reaches procedural changes, operator actions, maintenance and emergent activities — not only physical modification. The drafters were guarding against a reading in which only hardware counts.

The March 2026 amendment extending paragraph (a) to Part 53 licensees is worth noting on its own: when the technology-inclusive framework was finalized, the interface obligation was carried across rather than left behind. That is a signal about how durable the drafters consider the underlying concern.

---

**Where the SMR case departs**

The precedent is exactly right and it does not reach far enough, in three ways this corpus has to construct around.

**It governs a seam between two licensee programmes.** Both safety and security are things the licensee owns, staffs and is inspected against, which is what lets a rule assign a duty and name a moment. The dual design basis of Module 5 has a seam where one side has no regulatory programme at all: there is no artificial-intelligence design basis in Title 10 to interface *with*. So the corpus cannot borrow 73.58's mechanism, only its move — govern the seam — and must then build the governing object itself. That object is the Command Broker, and its three properties are an attempt to do for the autonomy boundary what 73.58 does for the safety/security boundary.

**It is change-triggered, which presumes a correct baseline.** The duty attaches before implementing changes to configuration, conditions or security. A design-basis extension is not a change to a configuration; it changes what the baseline was supposed to have covered. Nothing in 73.58 reaches a case where the two programmes were always in tension because the threat they were each drawn around differs.

**"Plant configurations" is a single-unit noun.** On a campus, a change to shared equipment alters the safety/security interface for every module simultaneously, and the assessment that satisfies the rule for one unit may not be the assessment that matters. That is the same scaling problem as [LI-08](../../register/LI-08-gdc-5-sharing-of-structures.md) and [LI-02](../../register/LI-02-campus-scaled-cda-identification.md), appearing here in a third vocabulary.

---

**Carry-forward**

A seam between two correct programmes is a governed object with an owner and a moment — and where one side of a seam has no programme to own it, the corpus must supply the governing object rather than assume the seam is safe.
