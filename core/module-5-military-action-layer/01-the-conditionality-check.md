# The Consequence-Basis Conditionality Check

Every safety claim is earned under assumptions. That is not a criticism; it is what makes a claim checkable. The trouble starts when a claim earned under one set of assumptions gets carried into a situation where those assumptions no longer hold, and nobody notices because the claim itself is still sitting there in the record, looking settled.

The reduced emergency planning zone is the clearest case. It is a real result, properly earned: smaller reactors with more retentive barriers release less, so the dose falls below the protective-action threshold at a shorter distance, so the zone can be smaller. Every step of that is defensible. All of it assumes the barriers hold. A deliberate actor can defeat specific barriers on purpose — which does not make the zone wrong, but does mean the zone does not cover everything people will assume it covers.

The Conditionality Check is the three-step discipline for handling that, and it is deliberately simple enough that a reviewer can apply it to any consequence relaxation in any sector.

## The three steps

**Declare the credited barriers.** Take the relaxation — the smaller zone, the longer coping duration, the reduced protection requirement, whatever it is — and write down explicitly what it depends on. Not the design in general: the specific barriers whose performance produces the favorable number. This step sounds trivial and is not, because a great deal of the credit in a mature safety case is implicit, distributed across analyses that were each individually reasonable.

**Test each barrier against the four characteristics.** For each declared barrier, ask whether it survives intentionality, persistence, precision and denial. A barrier that only fails under one of them is still a finding. The test is not whether the barrier is strong; it is whether its strength was ever meant to hold against something that chooses.

**State the residual.** Whatever the second step removed, name what is left unprotected and write it down in the record. This is the step that gives the method its value, and it is the step that is hardest to get past a reviewer, a management chain, or a communications department — which is precisely why it has to be a required step rather than a recommended one.

## Two corollaries that do most of the work

**The scaling corollary.** The largest relaxation carries the largest residual. This follows directly — the more favorable the number a barrier set buys you, the more there is to lose when the barrier set is defeated — and it is useful because it tells a reviewer where to look first. A design that has claimed modest relief in several places is a smaller problem than one that has claimed dramatic relief in one place, even when the two look comparable in the aggregate.

**Barrier-set specificity.** A residual belongs to a barrier set, not to a reactor type in general. This is where the design family chosen in Module 0 stops being bookkeeping. A residual that arises from a drained shared pool belongs to the pool-immersed family and is meaningless for a dry air-cooled design; a residual that arises from shared makeup to several condenser pools belongs to that architecture and to no other. A Conditionality Check performed generically produces generic conclusions, which is to say none.

## Where it sits in the corpus

The Check originates in the source-term instrument and was first worked at facility-class level in the SMR design basis, where the reduced zone is its first real instance. It is now registered at series level as a mandatory cross-sector requirement — the second such requirement, alongside the applicability determination that decides whether the military-action extension applies to a given facility at all.

That registration carries an inheritance obligation worth stating plainly: it runs from the source-term instrument, through the sector framework, into the facility-class instrument, and thence into any derivative. A sector framework that claims a consequence relaxation without performing the Check has not inherited properly, and a reviewer working through the traceability matrix should be able to see that.

What it does *not* have is regulatory standing. Nothing in the emergency-preparedness framework requires it, nothing endorses it, and nothing makes its output reviewable. Making it binding would take Commission action. That is the substance of [LI-05](../../register/LI-05-reduced-epz-conditionality.md), and it is the reason an applicant performing the Check voluntarily is doing something more useful than it may appear: a voluntarily declared residual on a public docket is the precedent that makes the requirement thinkable.

## The reduced zone, worked

Running the Check on the emergency planning zone produces the corpus's sharpest result, and it is worth following the whole way through because the shape recurs everywhere else.

The declared barriers are the ones that produce the small source term: the integral primary system with its reduced inventory, the containment, the passive and slow accident progression that buys time, and — depending on family — the scrubbing or retention mechanism that holds material up before release.

Tested against the four characteristics, several of these are conditional in ways the accident analysis never had to consider. Timing that is generous against a slowly developing accident is a different proposition against persistence. Retention that depends on an intact inventory of water is a different proposition against precision. And the analysis's assumption about what arrives and when is a different proposition against denial.

The residual is therefore real and has to be written down. But the honest version has a second half that is easy to miss and that the corpus insists on stating: because a contracted zone is what permits siting nearer to population, the favorable source term **slightly raises the consequence of its own residual**. The people nearest the plant are nearer because the accident arithmetic was good. That is the proximity coupling, and eliding it would make the whole method decorative.

The disposition follows from all of this and is the part most likely to be misread. The reduced zone **stays**. It was earned on accident-domain terms and those terms are unaffected. The residual is carried separately, as a military-action input, with protective action scaled and coupled to the tier triggers — not by re-enlarging the accident planning zone, which would be the wrong instrument applied to the wrong problem and would also destroy the reduced zone's legitimate basis in the process.

## What a reviewer should press on

Three things, in order of how often they are missed.

Whether the barrier declaration is complete, because an undeclared barrier is an undeclared residual. Whether the residual is stated on the public record or has migrated into a protected annex, which is the fairness question at the centre of [LI-12](../../register/LI-12-public-docket-and-safeguards-split.md). And whether the demonstration ran on aggregate campus inventory or on a single module's, which is a different failure entirely and has its own entry at [LI-06](../../register/LI-06-aggregate-inventory-in-the-epz-demonstration.md).

## What to carry forward

Declare the barriers, test them against the four characteristics, state the residual. The largest relaxation carries the largest residual; the residual belongs to a barrier set rather than to a reactor. A relaxation earned in the accident domain survives on its own terms and is not enlarged to cover the adversarial one — the residual is carried separately, and said out loud.

Next: [Correlated-Barrier Cutsets](02-correlated-barrier-cutsets.md), which is what the second step looks like when the barriers in question are supposed to be redundant.
