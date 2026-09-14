# LI-15 — Simultaneous Multi-Module Trip Reliability

A reactor's automatic shutdown is among the most thoroughly demonstrated functions in engineering, and its reliability is well characterized — for one reactor. When a dozen modules are commanded to shut down at the same instant, on a shared signal, through shared support systems, the relevant question is not the reliability of one trip but the reliability of all of them together. The facility-class instrument states outright that this has not been evaluated.

**The issue** — The reliability of simultaneous protective actuation across all modules on a campus, against shared signals and shared supports, has not been evaluated.

**Where it surfaces** — DBA-MA-SMR-FC1 §7.3, stated as unevaluated. It is picked up in the anticipated-request-for-information document as a question a reviewer should be expected to ask.

**Regulatory hook** — The General Design Criteria on protection-system reliability, testability and independence; IEEE 603 for safety-system criteria; and the sharing criterion of [LI-08](LI-08-gdc-5-sharing-of-structures.md).

**Why it is open** — **The method has not been developed.** Single-unit trip reliability is established; the campus-simultaneous case introduces correlation that the single-unit demonstration does not address, and no accepted method exists for demonstrating it.

**Closure vehicle and owner** — An applicant reliability demonstration for the simultaneous case, addressing common signals, shared actuation supports, and the correlated cutsets that make the modules' trips non-independent. **Owner: the applicant**, with the Commission accepting or not on the record. Unlike most entries here, nothing prevents this being answered — it simply has not been.

**State of play** — *As of September 2026.* Open and honestly flagged. The corpus's discipline is visible here in a useful way: rather than asserting that trip reliability carries over from single-unit practice, the instrument records that §7.3 is unevaluated and the anticipated-RAI document pre-poses the question against itself.

## Reader's stake

*For the practitioner* — A reviewer will ask this, and an applicant who has pre-answered it has bought schedule. The demonstration has to be a correlation argument, since simply multiplying single-unit reliabilities assumes exactly the independence that shared signals and shared supports remove.

*For everyone else* — Shutting a reactor down automatically is one of the most reliable things in the industry. Doing it for twelve reactors at once, through equipment they share, is a slightly different question, and the honest answer in the record right now is that it has not been worked out yet.
