# LI-10 — Deterministic Intent under a Risk-Informed Rule

Modern reactor regulation increasingly asks how *likely* things are, not only how bad they would be. Probabilistic risk assessment is very good at this for equipment failures and natural hazards, where frequencies can be estimated from data. Deliberate attacks have no such frequency. An adversary decides, and a decision is not a failure rate. So a framework that wants everything expressed as risk meets a hazard that cannot honestly be expressed that way.

**The issue** — How a deterministic adversarial postulate relates to the plant's probabilistic risk assessment under an increasingly risk-informed framework, without being assigned a frequency it does not have.

**Where it surfaces** — Developed in candidate work product 3C, which carries its own citable identifier; the underlying correlated-failure treatment is in the defense-in-depth instrument.

**Regulatory hook** — 10 CFR Part 53 and its risk-informed structure; the defense-in-depth and safety-margin principles it carries forward.

**Why it is open** — **The method has not been developed.** There is no accepted way to place a deterministic postulate inside a risk-informed case. The tempting move — treat the attack as another initiating event with an assumed frequency — is available and, the corpus argues, wrong.

**Closure vehicle and owner** — The corpus proposes borrowing the *conditional* machinery of risk assessment while refusing its initiator frequency. The adversary enters as a deliberate common-cause failure and a correlated-barrier cutset; the adversarial tiers act as conditioning variables; the result is a conditional consequence measure **given** the postulate, not a frequency-weighted aggregate. It enters the rule as a defense-in-depth and margin principle rather than as a risk contributor. **Owner: the Commission**, since this is an interpretation of how Part 53 accommodates a non-probabilizable hazard; **the applicant** for presenting it that way in the first campus case.

**State of play** — *As of September 2026.* Open. Candidate 3C is drafted and argues the position. The failure mode it is written against is specific and worth naming: assigning a low frequency to a deliberate act launders a deterministic requirement into a diluted average, after which the requirement quietly disappears into the noise of a risk total.

## Reader's stake

*For the practitioner* — Expect pressure to fold this in as a probabilized initiator, because it makes the case arithmetically tidy. Resisting it requires having the alternative ready: conditional core-damage and large-release measures given the postulate, tiers as conditioning variables, and the result presented as margin rather than as risk. Without that alternative in hand, the tidy answer wins by default.

*For everyone else* — Safety analysis usually asks "how often might this happen, and how bad would it be?" You can answer the first question for a pump failing. You cannot answer it for somebody deciding to attack. The argument here is about not pretending you can — because a made-up number, once averaged in with real ones, makes a serious hazard look small.
