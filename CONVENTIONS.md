# Authoring Conventions

These conventions keep the repository predictable as content is authored. They are deliberately close to the conventions of the [AI Governance course](https://scubanuke.github.io/ai-governance-course/), so the two sites read as siblings and an author moving between them does not have to relearn the shape. Where this site departs, the departure is noted and explained.

## The two halves

The site has a **course half** (`core/`, `bridge/`) and a **register half** (`register/`). Neither stands alone. The course teaches the licensing framework; the register holds what is unresolved within it.

The hinge between them is the **Open Issues** block that closes every module — this site's counterpart to the course's *In Your Sector*. It is the same block, same name, same shape, every time. Each module folder contains an `open-issues.md` that names the register entries falling under that module's material, says in one line why each one belongs there, and links into the register. The module carries the framework; the register carries the issue. Nothing is restated in both places.

## The layered opening

Every unit and every register entry opens with a short plain-language account before it goes to practitioner depth. This is a structural requirement, not a stylistic preference, and it is the site's one real departure from the course repository.

The opening explains what is happening in ordinary words — no CFR citation, no acronym that has not been spelled out on that page — and it is allowed to be two or three sentences. Everything after it may assume regulatory literacy. Do not weave the two registers together sentence by sentence; the reader should be able to feel where the primer ends.

## Register entries

Entries live in `register/`, one file per issue. Numbering is flat and sequential across the whole site: `LI-<NN>`. Filenames spell the issue out: `LI-01-counter-uas-defeat-authority.md`.

**Every entry carries the same seven fields, in this order:**

1. **The issue** — one sentence. If it takes two, the entry is really two entries.
2. **Where it surfaces** — the instrument and section where the question is raised: an FC1 section, a Track B or C instrument, a candidate work product. An issue with no locus in the corpus is not yet a register entry.
3. **Regulatory hook** — the provision the issue lives under: the CFR section, regulatory guide, or consensus document. Where there is genuinely no hook, say *none — that is the issue*, because an unhooked question is a different and usually harder problem.
4. **Why it is open** — the diagnosis, and it should fall into one of four kinds: authority is missing, guidance is absent, the threat basis is not calibrated, or the method has not been developed. Naming the kind is what makes the closure vehicle obvious.
5. **Closure vehicle and owner** — what would actually close it, and *who can move it*: NRC, NEI, the interagency, or the applicant. An entry without a named owner is an observation, not an issue.
6. **State of play** — current status, with a date. This field ages; it is expected to be revised.
7. **Reader's stake** — two short paragraphs, one for the practitioner and one for the non-specialist, saying what turns on the answer. This is what carries the layered audience without doubling the page count.

**A register entry states the question, not the answer.** Where the corpus has taken a position, the entry says so and cites the instrument that argues it; it does not re-argue it. Advocacy belongs in the instruments, which are signed and versioned. The register's value is that it can be trusted to say what is genuinely unsettled.

## Course Notes

The supporting-reference apparatus is carried over from the course repository unchanged: Notes live in `resources/course-notes/`, one file per Note, cross-linked from the unit they support, carrying the same seven fields — anchor, source and locator, provenance and use, excerpt or characterization, what it establishes, where the SMR case departs, carry-forward.

Two adjustments for this site. Field 6 is *where the SMR case departs* rather than the AI case, since the departures here are mostly from large-LWR precedent rather than from pre-AI practice. And the **excerptability rule bites harder**: federal regulations, regulatory guides, NUREGs, EPA and NIST material are U.S. government works and reproduce freely, but **NEI guidance documents are copyrighted industry consensus products and are characterize-only**, as are IEEE and ISO standards. A Note on NEI 08-09 or NEI 10-04 states what the section requires in our own words with the section number, and never reproduces it.

## Ownership across the sites

Some material appears on more than one Eclectic Technologies site. The dual design basis, the Bright Line, the Command Broker, the consequence-anchored root and the bounded adversary envelope are all taught in the [AI Governance course](https://scubanuke.github.io/ai-governance-course/) and all appear here. Two written treatments of the same construct will agree on the day they are written and will not stay agreeing, because they get revised on different occasions for different reasons — and nobody notices until a reader finds the seam described two ways.

The rule that prevents that:

**The course owns the method. This site owns its instantiation.**

Where a construct is derived and justified in the course, this site does not re-derive it. A unit here states what is specific to this facility class, this regulator, and this record, says enough for the page to stand on its own, and points to the course for the derivation. The reverse also holds: the course does not import SMR-specific findings, it points here.

The test when writing: *would this paragraph be equally true of a water utility or a data centre?* If yes, it is method and belongs to the course. If it is only true because this is a multi-module light-water campus under NRC review, it is instantiation and belongs here.

This is the same discipline the [Instrument Library](resources/instrument-library.md) applies to versions — one place carries the truth, everything else cites it — extended from versions to arguments.

**Shared terminology is governed series-wide.** "Bright Line" is two words, title case, no hyphen, and names the autonomy boundary only. Neither site may use it for the intent boundary between the design-basis threat and the state-actor layer. A terminology change agreed in the corpus applies to both sites in the same pass.

## Naming and ordering

Module folders are `module-N-slug`. Units carry a two-digit ordering prefix in teaching order, `00-`, `01-`, `02-`. The `90-` prefix is reserved for dated snapshot units that will age faster than the method around them — Module 1's rule-status snapshot is the current instance, and any unit that starts tracking a moving rulemaking should acquire a `90-` sibling rather than letting the volatility leak into the durable text.

Slugs are lowercase, hyphenated, spelled out rather than abbreviated, American English spelling. Every module folder has a `README.md`.

## Learning objectives

Every module README opens with a **Learning Objectives** block immediately after the title, phrased behaviorally: "After this module, a reader will be able to…" followed by three or four objectives, each something a reader can *do* — derive, distinguish, place, trace, argue — not something they will understand or be aware of. Objectives are one of the few places on this site where a list is the correct form.

## Versioning and currency

The site carries a single version at the root, in `README.md` and `course-map.md`. Units do not carry their own version numbers; material changes get a short changelog at the foot of the unit rather than a renamed file.

Instrument versions are a separate matter and a real hazard. The [Instrument Library](resources/instrument-library.md) is the single place where instrument versions and identifiers are recorded; units and register entries cite instruments **by designator without a version number** and let the library carry the version. This is deliberate — it is how the site avoids the drift that has repeatedly overtaken the version citations scattered across the corpus.

## Citations

Citations resolve to a durable target: a `.gov` URL, the publications Git mirror, or a DOI. **Never a cloud-drive link.** Where an instrument has its own standalone DOI, cite that; where it does not, cite the umbrella concept DOI with enough locator to find the piece. Both are listed in the Instrument Library.
