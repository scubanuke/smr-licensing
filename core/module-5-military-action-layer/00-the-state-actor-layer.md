# The State-Actor Layer

A nuclear plant is designed against a written list of things that could go wrong. Pipes break, pumps stop, the grid fails, the ground shakes. Each one is postulated, analyzed, and designed for, and the whole apparatus of reactor safety is the discipline of writing that list honestly and then meeting it.

Security adds a second list of a different kind. Instead of a failure, a person — a defined adversary with defined capabilities, described by the regulator, against whom the plant must be able to defend. That description is what the security programme is measured against.

Neither list contains a national military. Nobody proposes that it should: a commercial operator with a guard force is not going to hold off a state. But radioactive material does not care what category of event released it, and a regulator whose entire purpose is preventing radiological consequence cannot simply declare the question out of scope. This unit is about the narrow, defensible thing that can be said instead.

## Three tiers, and where the boundary sits

The adversarial basis in this corpus has three tiers. The lower tiers live inside the design-basis threat of Part 73 and are the licensee's to defend against in the ordinary way. Above them sits a layer the regulation does not reach: deliberate action by a state actor, conducted with military means, for reasons that have nothing to do with the plant's own vulnerabilities.

Two things about that boundary need stating precisely, because almost every misunderstanding of this material comes from blurring one of them.

The first is that the boundary is about *who*, not about *how bad*. A very large non-state attack still sits below it; a modest state action sits above. What distinguishes the layer is the actor and the intent behind the act, not the magnitude of the consequence — which is why an escalating list of worse and worse scenarios never arrives at it.

The second is that the layer is a **postulate, not a probability**. The design-basis threat is also a postulate, and that is its strength: nobody is asked to estimate how often a defined adversary will attack a given plant, only to demonstrate that the plant can withstand one that does. The state-actor layer works the same way and must be held to the same discipline. As soon as anyone asks how likely it is, the argument is lost — see [LI-10](../../register/LI-10-deterministic-intent-under-part-53.md), which is about exactly that failure mode.

This is also the point where the corpus's terminology has to be used carefully. The boundary between the Part 73 threat world and the state-actor layer above it **is not the Bright Line**. That term is reserved for the autonomy boundary in [The Dual Design Basis](03-the-dual-design-basis.md), and using it here — however natural it feels — collapses two distinct constructs that the corpus depends on keeping apart.

## The four characteristics

What makes deliberate action different from accident is not that it is worse. It is that it has four properties no accident has, and each one breaks a specific assumption that safety analysis quietly relies on.

**Intentionality.** An accident does not choose. An adversary does, and chooses the barrier whose loss hurts most. Safety analysis postulates the failure of one component and demonstrates that the design copes; it does not usually ask what happens if something selects the worst component to fail. That is the assumption intentionality removes.

**Persistence.** An accident is an event; it happens, and then the plant is coping with the aftermath. An adversary continues. A demonstration that shows a system reaching a stable condition has shown something less useful if the conditions can be re-disturbed at a time of someone else's choosing.

**Precision.** Accidents are indiscriminate, and defense in depth exploits that: with enough independent barriers, an indiscriminate insult is unlikely to defeat all of them. Precision is what makes that arithmetic stop working, and it is the property that [Correlated-Barrier Cutsets](02-correlated-barrier-cutsets.md) is entirely about.

**Denial.** This is the one most often left out, and it is the most consequential. An adversary can prevent the things a safety case assumes will be available — off-site power for longer than the analysis assumed, outside assistance, road access, the arrival of portable equipment, in some scenarios the operators themselves. Every credited action that depends on somebody arriving has to be re-examined under denial, and most of the interesting results in this corpus come from doing that.

## Supplements, does not replace

The single most important structural claim in this module is that the military-action layer **supplements the design basis rather than replacing it**. It is worth being explicit about what that means and what would break if it were otherwise.

It means the existing design basis stands, unaltered, and remains the thing the licensee is held to. The existing accident analyses are still valid; the existing security programme is still the measure of adequacy for the adversary it was drawn around; nothing in the licensee's obligations expands. What the layer adds is an additional analysis, over the top, that asks a different question: given a credited barrier set, which of those barriers survive a deliberate actor with the four characteristics, and what remains when the ones that do not survive are removed?

If the layer replaced the design basis instead, two things would go wrong immediately. The licensee would be held to a standard no commercial operator can meet, which turns the whole exercise into an argument nobody can win and therefore nobody will have. And the existing analyses — which are good, and which took decades to get right — would be reopened for no benefit, because the state-actor layer does not change how a reactor behaves when a pipe breaks.

There is a third reason, less obvious and more important. A supplementary layer can state a residual honestly. A replacement layer cannot, because a replacement implies that everything above it has been handled, and the whole value of this method is that it writes down what has *not* been handled.

## Where the licensee's obligation stops, and what fills the gap

If the licensee is not obliged to defend against a military, the natural question is who is. The corpus's answer has three parts, and each one lands somewhere different in the register.

Some of what is needed is authority the licensee should have and does not, of which the counter-uncrewed-aircraft case in [LI-01](../../register/LI-01-counter-uas-defeat-authority.md) is the clearest instance — a plain statutory gap wearing a regulation's clothes.

Some of it is threat characterization the regulator could make and has not, which is [LI-04](../../register/LI-04-state-actor-pre-positioning.md) — and it is worth noticing that raising pre-positioning inside the design-basis threat is a *different and smaller* move than the state-actor layer, not a version of it.

And some of it is not the plant's business at all but the government's, of which the warning pathway in [LI-11](../../register/LI-11-the-warning-pathway-and-who-decides.md) is the sharpest example. What the licensee owns there is narrow and real: the capability to receive a warning and act on it, distributed so that no single act removes the authority to act.

Naming which of the three a given problem belongs to is most of the analytical work. The rest of this module is the machinery for doing it.

## What to carry forward

The state-actor layer is a postulate above the design-basis threat, distinguished by actor and intent rather than magnitude, characterized by intentionality, persistence, precision and denial. It supplements the design basis rather than replacing it, which is what allows it to state a residual instead of implying there is none. And it is never assigned a probability, because the moment it acquires one it stops being a requirement and becomes a rounding error.

Next: [The Consequence-Basis Conditionality Check](01-the-conditionality-check.md), which is the method that turns all of this into something a reviewer can actually check.
