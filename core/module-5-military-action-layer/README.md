# Module 5 — Where the Military-Action Layer Enters

## Learning Objectives

After this module, a reader will be able to:

- State precisely where the state-actor layer sits relative to the design-basis threat, and why it supplements rather than replaces it.
- Apply the Consequence-Basis Conditionality Check to a claimed consequence relaxation and state the residual it leaves.
- Explain why a deliberate adversary is a correlated common-cause failure rather than an additional random one.
- Say what would have to be true for machine-learning-provenance logic to be admissible on a safety path, and why deterministic intent must not be folded into a probabilistic risk assessment as a frequency.

## What this module does

The previous module ended at a boundary: the design-basis threat bounds a defined adversary, and a licensee is expected to defend to it. A state actor conducting deliberate military action sits above that boundary. No one seriously proposes that a commercial licensee defend against a military, and the corpus does not propose it either.

What the corpus proposes instead is narrower and harder to dismiss. If a consequence relaxation — a smaller planning zone, a coping duration, a credited barrier — was earned by an argument that assumes accident conditions, then the relaxation does not automatically survive an adversary who can choose which barrier to defeat first. Saying so out loud, and writing down what residual remains, is the whole of the method.

This is also the module where the second design basis arrives: a facility where artificial intelligence participates in operations has two design bases, not one, and the seam between them has to be governed rather than assumed away.

## Units

**[The State-Actor Layer](00-the-state-actor-layer.md)** — the three-tier adversarial basis, the four characteristics of deliberate action that distinguish it from accident (intentionality, persistence, precision, denial), and the structural point that this layer is a *postulate* rather than a probability. Why the extension supplements the design basis and what it would break if it replaced it.

**[The Consequence-Basis Conditionality Check](01-the-conditionality-check.md)** — three steps: declare the credited barriers, test each against the four characteristics, state the residual. The scaling corollary — the largest relaxation carries the largest residual — and the reason a residual is barrier-set-specific, which is why the design family chosen in Module 0 matters here.

**[Correlated-Barrier Cutsets](02-correlated-barrier-cutsets.md)** — redundancy protects against independent failure. An adversary is not independent; shared supports, shared bays, shared feeds, and shared paths let a single deliberate act defeat several redundant trains. The adequacy question therefore becomes which correlated cutsets exist and whether any credited function survives their loss.

**[The Dual Design Basis](03-the-dual-design-basis.md)** — the facility-class basis and the artificial-intelligence basis inherit the same consequence root and diverge on the adversary envelope. The Command Broker governs the seam: a locked deterministic envelope under denial, with an independent hardware reset, and arbitration that fails to a safe default. *The term Bright Line is reserved for this autonomy boundary and is not used for the intent boundary of Module 4.*

**[Verification and the PRA Bridge](04-verification-and-the-pra-bridge.md)** — the two verification questions. A conjunctive admissibility gate for machine-learning-provenance logic: frozen artifact, declared credible input domain, proof where it scales with bounded coverage or explicit exclusion where it does not, and a runtime envelope closing the residual — all four, or the artifact is advisory only. And the risk-assessment bridge: borrow the conditional consequence machinery, refuse the initiator frequency, because a deliberate act has no defensible frequency and assigning one launders the deterministic case into a diluted average.

**[Open Issues](open-issues.md)** — what this module's material leaves unresolved. This module governs more of the register than any other.
