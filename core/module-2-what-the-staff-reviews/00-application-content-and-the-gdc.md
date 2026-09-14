# Application Content and the General Design Criteria

An application to build and operate a reactor is not a proposal. It is an evidentiary submission: a claim that a specific design, at a specific site, operated a specific way, provides reasonable assurance of adequate protection — accompanied by enough analysis for a federal agency to test the claim and write down whether it agrees.

That framing explains the volume. Nobody produces thousands of pages because thoroughness is a virtue in itself. They produce them because every requirement that applies has to be addressed on the record, and because the reviewer's written finding has to survive an independent committee and, potentially, a hearing.

## What actually goes in

The centre of gravity is the safety analysis report: the design described in enough detail to be evaluated, the accident analyses, the demonstration that the consequences of postulated events stay within limits. Around it sit the plans that govern how the plant will actually be run and protected — the security plan, the emergency plan, the quality assurance programme, the technical specifications that become enforceable operating limits — and, separately, the environmental report that drives the environmental review running in parallel with the safety review.

For an applicant relying on a topical report, part of the substance sits outside the application entirely, incorporated by reference. That is the whole point of the mechanism described in Module 1, and it is also why the wrapper and applicability statement discussed later in this module carry more weight than their page count suggests.

## The General Design Criteria

Appendix A to Part 50 contains roughly sixty General Design Criteria: the minimum design requirements for water-cooled nuclear power plants. They are grouped by concern — overall requirements, protection by multiple barriers, protection and reactivity control systems, fluid systems, containment, and the control of fuel and radioactivity.

The thing to understand about them is that they are **criteria, not specifications.** They state what must be achieved, not how to achieve it. A criterion requires that a protection system be highly reliable and testable; it does not say what the system is made of. That is what has let them survive fifty years of changing technology, and it is also why applying them to a genuinely new architecture is a matter of argument rather than of checking.

A reader coming to this from a standards background should resist the instinct to treat them as a checklist. The interesting work is always in the second step — not *does this criterion apply* but *what does satisfying it mean for this design*.

The criteria doing the most work for a multi-module campus are worth knowing by name.

The criterion on **sharing of structures, systems and components** requires that where units share equipment important to safety, the sharing must not significantly impair the ability to perform safety functions, including during an accident in one unit while the others keep running. Course Note [M02-CN-01](../../resources/course-notes/M02-CN-01-sharing-of-structures.md) carries it in full — it is a single sentence, which is part of what it establishes. Written for a two-unit station sharing a few systems. A campus shares nearly everything, and what the criterion demands at that degree of sharing has never been settled — see [LI-08](../../register/LI-08-gdc-5-sharing-of-structures.md), which is load-bearing for several other register entries.

The criteria on **protection against natural phenomena** and on **environmental and dynamic effects** are where external hazards land, and where a reviewer's attention goes when a design claims a small site footprint.

The criterion on **electric power systems** governs the interface with the grid, including what the plant does when the grid misbehaves. The campus behaviour during a frequency excursion is undefined, which is [LI-14](../../register/LI-14-under-frequency-load-shedding.md).

The criterion on **protection system reliability and testability** requires high functional reliability and inservice testability for the systems that shut the reactor down and actuate engineered safety features. It carries two of this site's open questions at once: whether simultaneous actuation across a whole campus meets it, [LI-15](../../register/LI-15-simultaneous-multi-module-trip.md), and what would be required to credit logic of machine-learning provenance against it, [LI-09](../../register/LI-09-ml-provenance-safety-logic.md).

The criteria on **residual heat removal** and **cooling water** are where the passive-safety case gets tested, and they connect directly to the coping-duration question in [LI-07](../../register/LI-07-assc-duration-on-aggregate-demand.md).

## A note on which framework applies

The criteria in Appendix A are written for water-cooled plants, and an applicant proceeding under the older pathways addresses them directly. The technology-inclusive framework finalized in 2026 is built differently — it does not simply restate the criteria — so which set of requirements an applicant is answering depends on the pathway chosen back in Module 1.

Two things hold regardless. The near-term integral light-water class still speaks the language of the criteria, because that is the vocabulary its designs and its reviewers grew up in and because the underlying safety concerns did not change when the framework did. And the analytical habit the criteria teach — state the safety function, state what could defeat it, demonstrate the margin — is the habit every framework is trying to formalize. A reader who learns the criteria has learned the questions, whichever rule ends up asking them.

## The pattern worth internalizing

Run a design-basis extension against the criteria and the same result recurs so often that it is worth stating as a finding rather than rediscovering each time.

For most criteria, the design **conforms to the principle and extends the application envelope.** The principle — defense in depth, redundancy, independence, testability — is satisfied. What changes is the range of demands over which it must hold: from natural and accidental to deliberate and adaptive, from a single unit to an aggregate campus.

Saying exactly that is a stronger position than claiming unqualified conformance, for a reason that is not obvious until you have watched a review go badly. Unqualified conformance invites a reviewer to find the one case where it does not hold, and having found it, to distrust the rest. A conformance statement that names the extended envelope up front has already conceded the interesting point and can then argue the margin — which is the argument the applicant actually wants to have.

## What a reviewer should press on

Whether the sharing criterion has been addressed as a campus question or answered with language written for a two-unit station.

Whether each criterion's conformance statement points to a specific analysis or merely asserts that the matter is addressed somewhere.

And whether the application and the incorporated topical report together cover every applicable criterion, or whether the seam between them has swallowed one — the failure mode the traceability matrix in Module 6 exists to make visible.

## What to carry forward

An application is an evidentiary submission, not a proposal. The General Design Criteria state what must be achieved rather than how, so applying them to a new architecture is argument rather than checking. Sharing, electric power, and protection-system reliability are where a campus design attracts the hardest questions. And the honest conformance posture is almost always *conforms to the principle, extends the application envelope*.

Next: [Requests for Additional Information, the Safety Evaluation, and ACRS](01-rais-the-se-and-acrs.md) — what the staff actually does with all of this.
