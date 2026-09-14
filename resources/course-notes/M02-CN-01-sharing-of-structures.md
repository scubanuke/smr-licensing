# Course Note M02-CN-01 — Sharing of Structures, Systems and Components

**Anchor** — Core / Module 2 · unit 00 *Application Content and the General Design Criteria* · heading *The General Design Criteria*

**Source and locator** — General Design Criterion 5, Appendix A to 10 CFR Part 50, "General Design Criteria for Nuclear Power Plants." [ecfr.gov/current/title-10/chapter-I/part-50/appendix-Appendix A to Part 50](https://www.ecfr.gov/current/title-10/chapter-I/part-50/appendix-Appendix%20A%20to%20Part%2050)

**Provenance and use** — Published · public domain (United States government work; reproduced in full)

---

**Excerpt**

> **Criterion 5—Sharing of structures, systems, and components.** Structures, systems, and components important to safety shall not be shared among nuclear power units unless it can be shown that such sharing will not significantly impair their ability to perform their safety functions, including, in the event of an accident in one unit, an orderly shutdown and cooldown of the remaining units.

One sentence. That is the entire criterion.

---

**What it establishes**

A default and an exception, in that order, which is the first thing to notice: **sharing is prohibited unless shown to be acceptable.** The burden sits with the applicant, and a criterion drafted the other way round — permitted unless shown to be harmful — would put it on the staff. That allocation is doing real work.

The test is that sharing "will not **significantly impair**" the ability to perform safety functions. Not that it will not affect them; a degree of interaction is contemplated and tolerated. The word doing the work is *significantly*, and the criterion supplies no metric for it.

The final clause is the most specific thing in the sentence and the most revealing. The demonstration must include **an accident in one unit while the remaining units shut down and cool down in an orderly way**. So the drafters had a concrete scenario in view: one unit in trouble, the others fine but dependent on something the troubled unit is also using, and the question of whether the others can get safely to cold shutdown anyway.

That is a two-unit station. It is a good criterion for a two-unit station.

---

**Where the SMR case departs**

Three ways, each of which turns the one-sentence criterion into a research problem.

**Degree.** The criterion contemplates *some* shared items among otherwise independent units. A small modular campus may share the control building, service water, electrical distribution, the ultimate heat sink, and the operating staff. At some point along that continuum the units stop being units-that-share and become one facility with several cores, and the criterion says nothing about where that point is or what changes when it is passed.

**Number.** "An accident in one unit … the remaining units" scans naturally for two. For twelve it raises a question the phrasing does not answer: does an orderly shutdown of eleven modules, simultaneously, through shared support systems, resemble the demonstration the criterion is asking for? The reliability of that simultaneous actuation is separately unevaluated in the corpus, at [LI-15](../../register/LI-15-simultaneous-multi-module-trip.md).

**Demand rather than availability.** The scenario in the clause is about *availability* — will the shared item still be there for the healthy units. A campus raises the different question of *aggregate demand*: the shared heat sink is available to all twelve and is being asked to absorb all twelve at once. That is the coping-duration question at [LI-07](../../register/LI-07-assc-duration-on-aggregate-demand.md), and the criterion's language does not reach it.

**And the criterion is a safety criterion, drawn around accident.** Its shared-item concern is that a failure in one place propagates. The corpus's concern is that a shared item is a **correlated barrier an adversary can select** — the cutset analysis of [Module 5](../../core/module-5-military-action-layer/02-correlated-barrier-cutsets.md). The criterion's principle covers it; its application envelope does not, which is the recurring pattern Module 2 names. This is the cleanest instance of that pattern on the site, because the criterion is short enough to see whole.

What the corpus must construct is therefore not a replacement but a method: how to demonstrate no significant impairment when sharing is pervasive, the unit count is high, the governing question is aggregate demand, and the failure of interest is selected rather than random. That is [LI-08](../../register/LI-08-gdc-5-sharing-of-structures.md), and it is load-bearing for several other entries.

---

**Carry-forward**

Sharing is prohibited unless shown not to significantly impair safety functions — the burden is the applicant's, the metric is unstated, and the scenario the drafters had in view was one accident among two units rather than aggregate demand across twelve shared ones.
