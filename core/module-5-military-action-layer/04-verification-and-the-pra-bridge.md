# Verification and the PRA Bridge

Two questions close this module, and they look unrelated until you notice they are the same question asked about different things: what does it take to *credit* something in a safety case?

The first asks it about machine learning. Could a component whose behavior was learned rather than specified ever be relied on for a safety action, and if so, on what showing?

The second asks it about intent. Modern reactor regulation increasingly wants safety expressed as risk — how likely, times how bad. A deliberate attack has no honest likelihood. So how does a deterministic postulate enter a framework built to average things?

Both are answered the same way: by being precise about what has actually been demonstrated, and refusing to accept a proxy for it.

## Part one — what it would take to credit a learned artifact

### The bar, and what it is actually about

The temptation is to argue about the label. Is this machine learning? Is it artificial intelligence? Is it "just" a neural network doing curve-fitting? None of that is the question, and submittals that fight on that ground lose regardless of which side they take.

The properties that matter for a safety function are determinism and formal verifiability over a bounded domain. A component that has them is admissible whatever produced it. A component that lacks them is not admissible however conventional it looks. Machine-learning provenance is neither disqualifying in itself nor, obviously, qualifying.

### The conjunctive gate

What the corpus proposes is an admissibility gate with four conditions, and the word that does the work is **conjunctive** — all four, or the artifact is advisory only, below the Bright Line, with nothing in the safety demonstration depending on it.

**The artifact is frozen, and its specification is written independently of it.** No continuous learning, no silent updates, and — critically — the deterministic specification is written separately rather than reverse-engineered from the artifact's observed behavior. A specification derived from the thing it is meant to check is not a check.

**The credible input domain is bounded and declared.** This is the condition most often fudged. The domain is the set of inputs the artifact could *physically encounter* — the realizable sensor space, given the instruments, their ranges, their failure modes and the physics of the plant — not every mathematically possible combination of numbers. Bounding it honestly is what makes verification tractable; bounding it optimistically is how a verification result becomes meaningless.

**Formal proof where it scales, with declared bounded coverage or explicit exclusion where it does not.** Proof by model checking, satisfiability solving, or sound abstract interpretation is what earns the phrase "verified deterministic logic." Where proof does not scale, the honest alternatives are declared coverage — boundary and equivalence-class testing, robustness bounding, a stated statistical basis — or outright exclusion of that region from the credited domain. What is not permitted is treating an unexamined region as benign.

**A runtime envelope closes the residual.** The artifact holds authority only inside the verified domain; outside it, control reverts to deterministic protective action. This is the Command Broker lock from the previous unit, and it is the answer to the objection that the domain can never be fully bounded — it does not have to be, provided the boundary is enforced at runtime rather than assumed at design time.

To which is added a fifth, procedural condition that is really the first one restated over time: **requalification on retraining**. A retrained artifact is a new artifact and re-enters the gate at the top.

### The honest posture

The corpus states plainly that **no near-term credited protective action depends on any machine-learning artifact**. Reactor trip and engineered safety actuation are deterministic already, by design and by long practice, and nothing in the current work proposes changing that.

Which makes this methodology **prophylactic**: it is the gate a future artifact would face, written now, while nobody is under commercial pressure to get a specific product through it. That ordering is worth defending explicitly, because it is unusual and because it is the whole reason the gate can be strict. A qualification standard written against a product that already exists tends to describe that product.

It also keeps the safety demonstration independent of anything unverifiable, which is the property a reviewer actually cares about. The open question — what an accepted methodology would look like and who would accept it — is [LI-09](../../register/LI-09-ml-provenance-safety-logic.md).

## Part two — the risk-assessment bridge

### What cannot be done

Probabilistic risk assessment is one of the genuine achievements of nuclear safety. Given failure rates grounded in operating experience, it produces defensible statements about how often core damage or a large release should be expected, and it has improved regulatory decision-making enormously.

It runs on frequencies. A deliberate act does not have one. Not "has one we cannot estimate well" — does not have one. An adversary's decision is not a random process with a hidden rate; treating it as one is a category error dressed up as conservatism.

The available and wrong move is to assign a plausible-looking number anyway and enter the attack as an initiating event. The result is arithmetically tidy and analytically corrosive: a small assumed frequency multiplied through the model produces a small risk contribution, the contribution disappears into the total, and a deterministic requirement has been **laundered into a rounding error**. Nobody decided to drop it. It simply stopped being visible.

### What can be done

The bridge the corpus proposes borrows the conditional machinery of risk assessment while refusing its initiator frequency. Three moves.

The adversary enters as a **deliberate common-cause failure** and a correlated-barrier cutset, in the sense developed in [Correlated-Barrier Cutsets](02-correlated-barrier-cutsets.md). Risk assessment already knows how to propagate a common-cause failure through a fault tree; what it gets here is a cutset selected rather than sampled.

The adversarial tiers act as **conditioning variables**, not as scenarios with weights. The question posed is what follows *given* tier activation, which is a question the model can answer honestly.

The output is therefore a **conditional** measure — conditional core damage or large-release frequency given the postulate — rather than a frequency-weighted aggregate. It sits alongside the probabilistic results rather than inside their sum, and it is read as margin rather than as risk.

Under a risk-informed rule, that is how it enters: as a defense-in-depth and safety-margin principle. Defense in depth already exists in the framework precisely to handle what the probabilistic model does not capture well, and a deterministic adversarial postulate is exactly the kind of thing it exists for. The open question of whether the framework will actually accommodate it this way is [LI-10](../../register/LI-10-deterministic-intent-under-part-53.md).

### What a reviewer should press on

Whether the presented result is conditional on the postulate or averaged over an assumed frequency — one number looks much like another on a slide, and only one of them means anything here. Whether the correlated cutsets were selected adversarially or sampled. And whether the deterministic requirement still appears anywhere in the conclusion, or has quietly become a contribution to a total.

## What to carry forward

Credit requires demonstration, and a proxy for demonstration is not demonstration. For a learned artifact: frozen with an independent specification, a bounded and declared credible input domain, proof where it scales with declared coverage or explicit exclusion where it does not, and a runtime envelope — all four, requalified on retraining, and stated prophylactically because nothing credited depends on such an artifact today. For deterministic intent: borrow the conditional machinery, refuse the frequency, report margin rather than risk, and keep the requirement visible.

That closes the module's machinery. Next: [Open Issues](open-issues.md) — the five register entries this module governs, which is more than any other.
