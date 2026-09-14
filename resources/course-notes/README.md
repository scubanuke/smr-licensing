# Course Notes

The supporting-reference apparatus, carried over from the [AI Governance course](https://scubanuke.github.io/ai-governance-course/) unchanged in shape.

A reading list is a burden handed to the reader: a pile of documents and no instruction about what to take from them. A **Course Note** is the alternative — a source placed *in context*, under the heading it serves, with a short account of what it establishes on its own terms and where the small modular reactor case departs from it. It is the handout a professor gives out when the material is too new to have a textbook.

Notes are numbered by module (`M04-CN-01`), anchored to a specific unit and heading, and cross-linked from the module text. They are not woven into the units: the unit carries the frame and the argument; the Note carries the source.

## Excerptability is a selection criterion

Federal regulations, regulatory guides, NUREGs, and Environmental Protection Agency material are United States government works and may be reproduced freely. **Industry consensus documents are copyrighted and may not be excerpted**, and neither may IEEE or ISO standards — those Notes run on characterization and citation only: what the section requires, in our own words, with the section number so the reader can go and read it.

Characterizing accurately requires having read the document, which for industry guidance means obtaining a copy through industry channels. A Note that characterizes a section the author has only read *about* is worse than no Note, and should not be written.

## The collection

| Note | Anchors to | Source |
|---|---|---|
| [`M02-CN-01`](M02-CN-01-sharing-of-structures.md) — Sharing of Structures, Systems and Components | Core / Module 2 · unit 00 · *The General Design Criteria* | Appendix A to Part 50, Criterion 5 |
| [`M03-CN-01`](M03-CN-01-epz-sizing-criterion.md) — The EPZ Sizing Criterion | Core / Module 3 · unit 01 · *What the 2023 rule changed* | 10 CFR 50.160; 50.33(g)(2); cf. 50.47(c)(2) |
| [`M04-CN-01`](M04-CN-01-safety-security-interface.md) — The Safety/Security Interface | Core / Module 4 · unit 00 · *The safety and security interface* | 10 CFR 73.58 |
| [`M04-CN-02`](M04-CN-02-the-cyber-security-plan-template.md) — The Cyber Security Plan Template | Core / Module 4 · unit 01 · *How industry guidance becomes review guidance* | 10 CFR 73.54; NEI 08-09 Rev. 6 (characterized) |
| [`M04-CN-03`](M04-CN-03-identifying-critical-digital-assets.md) — Identifying Critical Digital Assets | Core / Module 4 · unit 01 · *Where the campus breaks the method* | NEI 10-04 Rev. 2 (characterized); SRM COMWCO-10-0001; RG 5.71 |

The pair M04-CN-02 and M04-CN-03 is deliberate. The plan template establishes the programme; the scoping guidance decides what goes into it. Splitting them keeps each Note to one source in context, and it isolates the campus-scaling finding in the document that actually generates it.

Next to write:

Nothing is currently blocked on obtaining a source. The remaining candidates are ranked by what they would settle rather than by what is available: Regulatory Guide 5.71 in its own right, anchored to Module 4 unit 01, which is excerptable throughout and would let the control-set discussion run on primary text; and 10 CFR 73.55 on physical protection, anchored to Module 4 unit 00, where the corpus currently characterizes more than it needs to.

## Template

Copy this shape. If a Note cannot fill field 6, it does not belong on the site.

```markdown
# Course Note M<NN>-CN-<NN> — <Short Title>

**Anchor** — <module / unit / heading it attaches to>

**Source and locator** — <full citation, precise locator, durable link:
.gov URL, Git mirror, or DOI — never a cloud-drive link>

**Provenance and use** — <published | prepublication | working note> ·
<public domain | licensed | CHARACTERIZE ONLY>

---

**Excerpt** — <verbatim and bounded>

> ...

*(Where reproduction is not permitted, replace this field with a
**Characterization**: what the clause requires, in our own words, with
the clause number so the reader can go read it.)*

---

**What it establishes** — <what the source settled, inside its own domain,
on its own terms. No editorializing yet.>

---

**Where the SMR case departs** — <the payload. What has no counterpart for
this facility class, what breaks when the concept is carried across, and
what the corpus therefore has to construct.>

---

**Carry-forward** — <one sentence the reader takes into the next section.>
```
