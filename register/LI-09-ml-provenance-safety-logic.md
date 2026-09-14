# LI-09 — Machine-Learning-Provenance Safety Logic

Nuclear safety systems are required to be predictable: given the same inputs, the same output, every time, and demonstrably so. Machine-learning systems are trained rather than specified, which makes them hard to characterize that way. The question is not whether artificial intelligence is allowed near a reactor — it is already used for monitoring and advice. It is whether a component that *came from* machine learning could ever be credited for a safety action, and what would have to be proved first.

**The issue** — What admissibility conditions would allow a frozen artifact of machine-learning provenance to be credited on a safety instrumentation-and-control path rather than confined to an advisory role.

**Where it surfaces** — DBA-MA-SMR-FC1 §6.2 states the bar; the Command Broker nuclear annex governs the runtime side; the tiered assessment framework sets the programme-level verification frame. Candidate work product 3B develops the artifact-level methodology and carries its own citable identifier.

**Regulatory hook** — The General Design Criterion on protection-system reliability and testability; IEEE 603 for safety-system criteria; 10 CFR 73.54 for frozen-artifact integrity and provenance, which links this to [LI-03](LI-03-shared-digital-ic-guidance.md).

**Why it is open** — **The method has not been developed.** No accepted qualification methodology exists at the artifact level. The instruments that surround the question each govern something adjacent — the bar, the runtime envelope, the programme frame — and none of them tells a reviewer how to qualify the artifact itself.

**Closure vehicle and owner** — The corpus proposes a **conjunctive admissibility gate**: the artifact is frozen and its specification written independently of it; the credible input domain is bounded and declared as the physically realizable sensor space rather than all mathematically possible inputs; formal proof is applied where it scales, with declared bounded coverage or explicit exclusion where it does not; and a runtime envelope confines the artifact's authority to the verified domain, reverting to deterministic protective action outside it. All four conditions, plus requalification on retraining — fail any one and the artifact is advisory only. **Owner: the Commission** for acceptance of a methodology; **standards bodies and industry** for the consensus form; **the applicant** for any specific artifact.

**State of play** — *As of September 2026.* Open, and deliberately **prophylactic**. The corpus states plainly that no near-term credited protective action depends on any machine-learning artifact — reactor trip and engineered safety actuation are already deterministic — so this is the gate a future artifact *would* face rather than a claim being made now. That honesty is what keeps the safety demonstration independent of anything unverifiable.

## Reader's stake

*For the practitioner* — The most common failure here is arguing about the word rather than the property. The bar is determinism and formal verifiability over a bounded domain; whether the artifact's provenance is machine learning is not itself disqualifying, and is not itself qualifying either. A submittal that says "no credited action uses machine learning today, and here is the gate any future one would pass" is far stronger than one that argues the label.

*For everyone else* — Nothing that automatically shuts a reactor down today depends on artificial intelligence, and the corpus says so rather than leaving it vague. What is being worked out in advance is what would have to be proved before anything like that could be trusted with a safety job — which is the right order to do it in.
