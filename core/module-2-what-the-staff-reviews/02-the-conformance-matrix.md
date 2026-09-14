# The Conformance Matrix

A Safety Evaluation is written requirement by requirement. So the single most useful thing an applicant can hand a reviewer is a table that runs the same way: here is the provision, here is what it obliges, here is where the record addresses it, here is the statement of how it conforms.

That is the conformance matrix. It looks like administrative apparatus and it is the substance of the filing, because it is the only artifact in the submission organized the way the finding has to be organized.

## The four columns

**The provision.** Cited precisely enough to be looked up — a specific General Design Criterion, a section of Part 73, a regulatory guide position. Not "Appendix A" but the criterion.

**The obligation.** What the provision actually requires, restated in a sentence. This column is where sloppiness shows first, because restating an obligation accurately forces the author to decide what it means before claiming to meet it.

**Where addressed.** The place in the record — a section of the design basis, an inherited instrument, a supporting analysis. A pointer that lands on an *argument*, not merely a chapter heading.

**The conformance statement.** The claim, and its qualifications. This is the column that carries the weight and the one most often written badly.

Group the rows the way a reviewer will approach them: pathway and applicability first, then the design criteria, then security, then the consequence and source-term provisions, then anything specific to the design's novel features. A reviewer who can find their own area quickly forms a good opinion of the document before reading a word of the analysis.

## Writing a conformance statement honestly

Three failure modes recur, and each one costs more than it saves.

**Asserting rather than demonstrating.** "The design conforms" is not a conformance statement. It is a claim with no basis, and the reviewer's only available response is an RAI asking for the basis — so the row has generated work rather than saving it.

**Pointing at a location instead of an argument.** "Addressed in Section 5" tells a reviewer where to go looking but not what they will find or why it settles the question. A cell that says which analysis establishes conformance, and in one clause why, converts a search into a confirmation.

**Claiming unqualified conformance where the envelope has been extended.** This is the subtle one and it is the pattern Module 2's previous unit identified: for most criteria a design-basis extension conforms to the *principle* while extending the *application envelope*. Saying so plainly is stronger than glossing it, because a reviewer who discovers the extension themselves will wonder what else was glossed.

## Where the record does not conform

The rule that makes a matrix usable rather than promotional: **where there is a gap, the matrix records the gap and names the vehicle that would close it.**

This is counter-intuitive to anyone who has written a compliance document in another industry, where an admitted non-conformance is a finding waiting to happen. Here it is the opposite. A reviewer's job is to reach a documented conclusion about every applicable provision, and a matrix that manufactures conformance makes that job harder, not easier — the reviewer has to discover the gap, having now been given reason to doubt every other row.

A gap stated with its closure vehicle does three things at once. It tells the reviewer that the applicant knows. It tells them the applicant has thought about what would resolve it. And it converts an open item from a deficiency into a tracked action with an owner — which is what the register on this site is, generalized.

The corresponding rows in the submittal matrix do exactly this. Where the counter-uncrewed-systems authority is absent the matrix says so and points at the statutory vehicle rather than claiming the physical-protection provision is satisfied. Where the campus cyber-scoping method does not exist the matrix records it and routes to the consensus process. Those are [LI-01](../../register/LI-01-counter-uas-defeat-authority.md) and [LI-02](../../register/LI-02-campus-scaled-cda-identification.md), and they are on the register precisely because the matrix refused to paper over them.

## The complement

A conformance matrix maps **outward**: from the record to the regulation. Its twin maps **inward**: from each requirement to the instrument that carries it and the obligation it satisfies.

Neither alone catches everything. Outward-only can be complete against the regulation while an internal requirement sits in no instrument at all. Inward-only can show every requirement carried while missing a provision nobody mapped. Run both and an **orphan becomes visible** — a requirement with no carrier, or a carrier serving no requirement.

Module 6 develops the pair as a completeness ledger. The thing to carry from here is why two directions are needed rather than one thorough table.

## A note on currency

A matrix cites instruments, and instruments have versions. A matrix that carries version numbers in its cells is a drift hazard: the instruments advance, the matrix does not, and a reviewer eventually finds a row citing a superseded document — which raises a question about the whole table that has nothing to do with the technical case.

This site's answer is the rule in [Conventions](../../CONVENTIONS.md): cite instruments by designator and let one place, the [Instrument Library](../../resources/instrument-library.md), carry versions. A submittal matrix has the same problem and benefits from the same discipline.

## What a reviewer should press on

Whether any conformance statement asserts without a basis.

Whether the extended-envelope pattern is named where it applies, or quietly absent from rows where it clearly does.

Whether stated gaps carry vehicles and owners, or trail off into "will be addressed."

And whether the matrix and the record actually agree — the cheapest useful check being to pick three rows at random and follow them, which is what a reviewer will do in the first hour.

## What to carry forward

The matrix is the spine a Safety Evaluation is built on, and it is substance rather than apparatus. Four columns: provision, obligation, where addressed, conformance statement — with the last one demonstrating rather than asserting. Where the record does not conform, the matrix says so and names the vehicle, because manufactured conformance costs a reviewer's trust in every other row. And it needs its inward-facing twin before an orphaned requirement becomes visible.

Next: [Open Issues](open-issues.md) — three entries, and they are the same question in three vocabularies.
