# Course Note M03-CN-01 — The EPZ Sizing Criterion

**Anchor** — Core / Module 3 · unit 01 *From Dose to Zone* · heading *What the 2023 rule changed*

**Source and locator** — 10 CFR 50.160, "Emergency preparedness for small modular reactors, non-light-water reactors, and non-power production or utilization facilities," which refers the sizing determination to 10 CFR 50.33(g)(2). [ecfr.gov/current/title-10/chapter-I/part-50/section-50.160](https://www.ecfr.gov/current/title-10/chapter-I/part-50/section-50.160) and [/section-50.33](https://www.ecfr.gov/current/title-10/chapter-I/part-50/section-50.33). Both sections: 88 FR 80075–80076, 16 November 2023, as amended at 91 FR 15787, 30 March 2026. Compare 10 CFR 50.47(c)(2) for the legacy basis.

**Provenance and use** — Published · public domain (United States government work)

---

**Excerpt**

The legacy position, at 50.47(c)(2):

> Generally, the plume exposure pathway EPZ for nuclear power plants shall consist of an area about 10 miles (16 km) in radius and the ingestion pathway EPZ shall consist of an area about 50 miles (80 km) in radius. … The exact size and configuration of the EPZs surrounding a particular nuclear power reactor shall be determined in relation to local emergency response needs and capabilities as they are affected by such conditions as demography, topography, land characteristics, access routes, and jurisdictional boundaries. The size of the EPZs also may be determined on a case-by-case basis for gas-cooled nuclear reactors and for reactors with an authorized power level less than 250 MW thermal.

The route the 2023 rule opened, at 50.33(g)(2):

> Small modular reactor, non-light-water reactor, or non-power production or utilization facility applicants complying with § 50.160 who apply for a construction permit or an operating license under this part, or small modular reactor or non-light-water reactor applicants complying with § 50.160 who apply for a combined license or an early site permit under part 52 of this chapter, must submit as part of the application the analysis used to determine whether the criteria in § 50.33(g)(2)(i)(A) and (B) are met and, if they are met, the size of the plume exposure pathway EPZ.

And the criterion that analysis is run against, at 50.33(g)(2)(i), which turns on whether public dose

> is projected to exceed 10 mSv (1 rem) total effective dose equivalent over 96 hours

from radioactive releases.

---

**What it establishes**

Read the two together and the change is visible in the grammar rather than in any statement of policy.

The legacy provision **states a size**. Ten miles, fifty miles, generally — with configuration adjusted for local conditions and a narrow case-by-case opening for gas-cooled reactors and reactors under 250 megawatts thermal. An applicant outside that opening seeking a different size is seeking relief from a stated number.

The 2023 route **states a criterion and requires an analysis**. There is no number to be relieved from. The applicant submits the analysis, the analysis is run against a dose threshold, and the EPZ is whatever satisfies it. The provision does not say the zone will be smaller; it says the zone is an output.

Three details in the criterion are worth fixing in mind, because each one is a place an argument can go wrong. The threshold is expressed in **dose, not distance**. It is **projected** dose, so it is a calculation about a postulated release rather than a measurement. And it is integrated **over 96 hours**, which bounds the exposure period the analysis must cover and is not a figure an author should leave implicit.

Note also that both sections were amended on 30 March 2026 — the same day Part 53 was finalized — extending the route to the technology-inclusive framework. The same conforming-amendment pattern as [M04-CN-01](M04-CN-01-safety-security-interface.md).

---

**Where the SMR case departs**

The criterion is complete, checkable, and silent on the thing this corpus exists to say.

**It is an accident-domain criterion and contains nothing that could make it otherwise.** "Projected to exceed 1 rem over 96 hours" presupposes a postulated release; the postulate comes from the design-basis accident set; and that set is populated by failures and natural hazards. Nothing in the provision asks whether the barriers producing the favorable projection survive an actor who selects which one to defeat. The rule is not wrong about this — it is answering the question it was written to answer.

**There is no place in the provision to record a conditionality.** The applicant submits an analysis and a size. There is no field for *this size holds provided the following barriers hold, and here is what remains if they do not.* So the Conditionality Check of [Module 5](../../core/module-5-military-action-layer/01-the-conditionality-check.md) has no home in the regulatory artifact, which is the whole of [LI-05](../../register/LI-05-reduced-epz-conditionality.md).

**The criterion is silent on inventory basis.** It says public dose from radioactive releases, without stating whether the release is postulated from one module or from a campus. For a single-unit plant the question does not arise. For a shared-barrier campus it is the most consequential input in the analysis, and the provision does not settle it — [LI-06](../../register/LI-06-aggregate-inventory-in-the-epz-demonstration.md).

**And the legacy provision's case-by-case opening is instructive by contrast.** It is bounded by reactor type and by power level — proxies for consequence. The 2023 route replaces the proxies with the consequence itself, which is better, and in doing so removes the only place where a physical characteristic of the reactor was doing gatekeeping work. What replaces it is the honesty of the analysis.

---

**Carry-forward**

The zone is an output of a dose criterion — 1 rem total effective dose equivalent, projected, over 96 hours — and not a distance granted or relieved; the criterion is complete for the domain it was written for, and has no field in which to record what that domain excludes.
