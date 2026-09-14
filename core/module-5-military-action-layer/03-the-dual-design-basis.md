# The Dual Design Basis

When artificial intelligence shows up in an industrial facility, the usual instinct is to treat it as another component: qualify it, put controls around it, add it to the list. That instinct produces governance that looks thorough and holds nothing, because the thing being governed is not a component. It is a participant — something that observes, decides, and acts, on a schedule nobody approved in advance.

The claim in this unit is that a facility where artificial intelligence participates has **two design bases, not one**, and that the seam between them is the object that has to be governed.

> **Where this is derived.** The two-design-basis construct, the inherit-and-diverge argument, and the merge as a managed interface are developed sector-agnostically in the [AI Governance course](https://scubanuke.github.io/ai-governance-course/), Module 3 units 04 and 05, with the governance primitives in its Module 4. Per [Conventions](../../CONVENTIONS.md), the course owns the method and this site owns its instantiation. What follows states the construct compactly and then spends its length on what is specific to this facility class — which is the part the course does not carry.

## Why two, in one paragraph

Both bases share a **consequence root**, because artificial intelligence creates no new consequence set: whatever the plant could do to the world, it could already do. The artificial-intelligence basis therefore inherits that root, which is what keeps it anchored to something that matters rather than to an invented severity scale of its own. Where the two **diverge is the adversary envelope** — the facility basis is drawn around failures, hazards and a defined human adversary, while the artificial-intelligence basis has to be drawn around a system that can be manipulated through its inputs, whose behavior outside a bounded domain does not follow from its behavior inside it, and which can be induced to act wrongly without anything on the plant having failed at all. Same root, different envelope: that is the argument for two bases, and the reason the second cannot be folded into the first, which has no vocabulary for an envelope of that shape.

## The seam, and what the Bright Line is

The two bases meet. Where they meet is the **Bright Line** — the boundary that artificial intelligence may not cross into safety-critical action.

This term is reserved. It means the autonomy boundary and nothing else. In particular it does **not** name the boundary between the design-basis threat and the state-actor layer discussed in [The State-Actor Layer](00-the-state-actor-layer.md), which is a different distinction that the corpus deliberately keeps separate. Reviewers reading across instruments should treat any use of Bright Line for the intent boundary as an error.

What sits below the line is the part of the plant that acts without asking anything: reactor trip, engineered safety actuation, the protective functions that fire on plant conditions through deterministic logic. What sits above it is everything advisory, optimizing, monitoring, and assisting. The line is not a statement about how good the artificial intelligence is. It is a statement about what the safety demonstration is allowed to depend on.

This has a consequence that matters more than it sounds: because the credited protective functions sit below the line, a compromise of the digital and generative layer does not by itself defeat them. That is the design backstop in [LI-03](../../register/LI-03-shared-digital-ic-guidance.md), and stating it precisely is what keeps the cyber argument honest in both directions — the trip is not defeated, and the operators' situational awareness very much can be.

## The merge, and why it is not a hierarchy

A seam is a picture; what makes it operable is the answer to what happens when the two bases give conflicting answers.

The course settles that question and the answer is worth restating because everything below depends on it: **what is inherited is consequence, not authority.** The artificial-intelligence basis inherits the facility's consequence root without thereby becoming subordinate to the facility basis, so at the seam the two are co-equal and neither resolves a collision by outranking the other. The merge is therefore a **managed interface** — an assignable duty to detect a conflict before acting, plus a named arbiter when one surfaces at runtime — rather than a hierarchy. The derivation is in the course's Module 3 unit 05.

The arbiter is the Command Broker, and how it behaves at a nuclear facility class is where this site takes over.

## The Command Broker

The Command Broker is what enforces the Bright Line in operation rather than on paper. Three properties define it, and a submittal should be checkable against each.

**A locked deterministic envelope under denial.** When conditions degrade — communications lost, operators unavailable, the situation unrecognizable — the system does not get more autonomous to compensate. It locks into a bounded, deterministic envelope whose behavior is fully specified in advance. The temptation runs exactly the other way, because a degraded situation is when flexible automation looks most valuable, and that is the temptation the lock exists to remove.

**An independent hardware reset.** A path out of the locked state that does not run through the software being locked. If the only way to restore normal authority is through the system whose trustworthiness is in question, the lock is decorative.

**Arbitration that fails to a safe default.** When the two bases collide and the Broker cannot resolve it, the outcome is the deterministic safe action, not the artificial-intelligence-preferred one and not an indefinite hold.

One detail is easy to get wrong and worth stating explicitly: the **lock endurance is keyed to the seventy-two-hour class floor**, not to the family-specific coping duration. The plant may be able to hold itself safe for considerably longer than seventy-two hours, and the envelope is nonetheless specified against the floor. This is deliberate conservatism — the governance commitment should not vary with a thermal-hydraulic number that is itself under discussion in [LI-07](../../register/LI-07-assc-duration-on-aggregate-demand.md).

## The operational payoff

There is a practical reason to insist on a written artificial-intelligence design basis that has nothing to do with regulators, and it is the argument that usually persuades people who find the rest of this abstract. It is a general point rather than a nuclear one — the course develops it in Module 3 unit 05 — but it is the reason an applicant should want this document rather than merely accept it.

The artificial-intelligence design basis is the **source document for procurement**. The contract requirements for an artificial-intelligence-enabled system are derived from it, as is the spine of the acceptance test plan the customer runs at delivery, and the re-test trigger that says which supplier changes are significant enough to require requalification rather than being absorbed as a routine update.

Without it a facility negotiates acceptance criteria from scratch with each vendor, at the worst possible moment, against whatever the datasheet asserts. With it, the facility knows what it is buying before it asks for a price.

## What a reviewer should press on

Whether the envelope is provably bounded rather than merely described. Whether the reset is genuinely independent of the locked software. Whether arbitration fails to the deterministic safe default in every branch, including the ones nobody expects to reach. And whether anything credited in the safety demonstration sits above the line — which is the admissibility question taken up in the next unit.

## What to carry forward

Two design bases, sharing a consequence root and diverging on the adversary envelope. The Bright Line is the seam and the term is reserved for it. What is inherited is consequence, not authority, so the merge is a managed interface rather than a hierarchy, with the Command Broker as arbiter: locked deterministic envelope under denial, independent hardware reset, arbitration failing safe. And the artificial-intelligence basis is the document procurement and acceptance testing are built from.

Next: [Verification and the PRA Bridge](04-verification-and-the-pra-bridge.md), which asks what it would take to credit something above the line, and how a deterministic postulate relates to a probabilistic case.
