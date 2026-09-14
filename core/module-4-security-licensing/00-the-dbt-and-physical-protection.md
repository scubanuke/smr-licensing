# The Design-Basis Threat and Physical Protection

Safety engineering asks what happens when things break. Security asks what happens when somebody breaks them on purpose, and that turns out to need its own regulatory world with its own logic, its own reviewers, and its own part of Title 10.

The organizing device of that world is a written description of an adversary. Not a warning, not an assessment of who is currently interested in attacking nuclear plants — a defined set of capabilities against which a licensee must demonstrate protection. Everything else in reactor security is calibrated to that description, and the most common confusion in this entire subject comes from mistaking it for a prediction.

## What the design-basis threat is, and what it is for

The design-basis threat lives in 10 CFR 73.1. It is a construct: a specified adversary, characterized well enough that protection against it can be designed, demonstrated, inspected, and enforced.

Two features of it are worth understanding before anything else.

It is **set by the Commission, not by the licensee.** That allocation is deliberate and it does real work. A licensee cannot be asked to divine the threat and then be held to whatever it divined, because that standard is unenforceable and unfair in both directions — too generous and it means nothing, too demanding and it cannot be met. Fixing the description centrally gives every licensee a common target, lets inspection mean something, and makes the level of protection a matter of public policy rather than of private discretion.

It also means, unavoidably, that **where the threat description stops is where private obligation stops.** That is not a loophole. It is the boundary between what a commercial operator is expected to handle and what the government handles, and someone has to draw it. What the boundary should be is a genuine policy question with costs on both sides, and it is the question [LI-04](../../register/LI-04-state-actor-pre-positioning.md) puts on the table.

The corollary that matters most for Module 5 is this: the design-basis threat bounds the licensee's duty, not the universe of things that could happen. A plant that meets it has met its obligation. It has not been shown to be invulnerable, and nobody ever claimed it had.

## The physical-protection programme

10 CFR 73.55 is the requirement to protect against radiological sabotage, and its structure follows a simple logic: keep an adversary out of the places where they could cause a radiological release, notice if they try, and be able to respond in time.

That produces a layered site — successively controlled areas, with barriers and access control between them, the innermost containing the equipment that actually matters. It produces a detection and assessment obligation, because a barrier you do not know has been breached is not doing much. And it produces an armed response capability sized to the threat description.

The concept underneath all of it worth carrying forward is the **target set**: the combinations of equipment whose defeat would cause the consequence the rule exists to prevent. Protection is organized around denying an adversary a complete target set rather than around protecting every item equally, which is both more effective and more honest about where the money should go.

Readers who reach [Correlated-Barrier Cutsets](../module-5-military-action-layer/02-correlated-barrier-cutsets.md) will recognize the shape. A target set and a correlated cutset are close cousins — both ask which combinations of losses matter rather than which single losses do. The military-action extension does not invent that reasoning; it pushes it further, into supports and dependencies that a target-set analysis drawn around the design-basis threat has no particular reason to examine.

## The safety and security interface

> **Course Note [M04-CN-01](../../resources/course-notes/M04-CN-01-safety-security-interface.md)** carries 10 CFR 73.58 in full, with what it establishes and the three ways this case departs from it.

One provision deserves singling out because it is easy to miss and it governs a real hazard. 10 CFR 73.58 requires a licensee to assess and manage the effect of security changes on safety, and vice versa.

The hazard it addresses is specific. A security measure can degrade a safety function — a barrier placed where it impedes access needed in an emergency, a door-locking regime that slows an operator response the safety analysis credits. Neither discipline catches this on its own, because each is evaluating against its own criteria, and both can be individually correct while the combination is worse than either.

The provision's deeper interest is that it makes **the interface itself the governed object** rather than leaving it in the gap between two programmes. That move — govern the seam, not just the things on either side of it — recurs when the dual design basis arrives in Module 5, where the seam between the facility basis and the artificial-intelligence basis needs the same treatment.

## The authority you do not have

The sharpest thing in this module is a gap that no amount of compliance closes.

An uncrewed aircraft over a nuclear plant can be detected, tracked, and assessed. It cannot lawfully be brought down by the licensee. The federal counter-uncrewed-systems authority that permits active defeat was extended to federal departments and not to commercial reactor licensees, and airspace authority sits with the Federal Aviation Administration in any case. So the operator with the sensors, the guard force, and the sabotage-prevention obligation has no authority to act on what the sensors show, while a federal installation down the road has both.

Two asymmetries are worth naming precisely because they get blurred together. **Detect but not defeat** is the licensee's internal problem: a capability that stops one step short of useful. **Federal site yes, commercial reactor no** is the comparative problem: two facilities with comparable consequence, treated differently, for reasons of statutory history rather than of risk.

This is the cleanest example on the whole site of a question that looks regulatory and is not. The Commission cannot grant by regulation a power Congress has not conferred. What the Commission *could* do — write implementing physical-protection requirements — only becomes possible after the authority exists. The full treatment, including the argument that the authority should be grounded in the intent-agnostic sabotage-prevention mission rather than in any determination that an act of war has occurred, is at [LI-01](../../register/LI-01-counter-uas-defeat-authority.md).

## What a reviewer should press on

Whether a submittal treats the counter-uncrewed-systems gap as a licensee performance deficiency, which invites a finding no applicant can satisfy, or as the statutory boundary it is, with a vehicle named.

Whether the target-set analysis accounts for a multi-module configuration, where shared equipment can belong to several target sets at once — the security-side twin of the sharing question at [LI-08](../../register/LI-08-gdc-5-sharing-of-structures.md).

And whether the safety and security interface has been assessed as a live obligation or treated as a form to file.

## What to carry forward

The design-basis threat is a Commission-set construct that bounds licensee obligation rather than predicting events, and where it stops is where private duty stops. Physical protection is organized around denying complete target sets, not around protecting everything equally. The interface between safety and security is itself a governed object. And the counter-uncrewed-systems gap is a statute problem wearing a regulation's clothes.

Next: [Cyber Security under 10 CFR 73.54](01-cyber-security-under-73-54.md), where the same threat basis meets a campus that shares nearly all of its digital infrastructure.
