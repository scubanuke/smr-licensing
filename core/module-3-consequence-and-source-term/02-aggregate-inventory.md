# Aggregate Inventory

The selling point of a small modular reactor is in the adjective. Less fuel, less decay heat, less radioactive material, and therefore a smaller consequence and a smaller planning zone. Every step of that is true of *a module*.

A campus is not a module. Twelve of them on one site, sharing a control building, a service water system, an electrical distribution and often the heat sink itself, hold a great deal of radioactive material and are not twelve independent plants that happen to be adjacent. Whether the safety demonstration is done for one of them or for all of them together is the single most consequential input in this module, and the guidance does not unambiguously say which governs.

## Two questions, often run together

Separating them is most of the analytical work.

**How much material is at stake?** If an event can affect more than one module, the inventory available for release is the aggregate rather than a single unit's. This is arithmetic, and it is the easier half.

**Are the barriers credited per-module or shared?** This is the harder half and the one that decides the first. If each module has its own independent containment, its own heat sink, its own everything, then an event that defeats one module's barriers says little about the other eleven, and a per-module analysis is closer to defensible. To the extent the barriers are shared — one pool, one ultimate heat sink, one set of support systems — then defeating the barrier once affects every module that depends on it, and the modules were never independent in the way the arithmetic assumed.

Real designs sit between these poles and the position differs by family. That is why the choice made in Module 0 keeps returning: a shared immersion pool is a shared barrier by construction, while per-module condenser pools are independent right up to the point where they need makeup from a common source.

## Why per-module does not carry

The temptation is to argue that a per-module analysis is adequate because a simultaneous multi-module event is unlikely. There are two problems with that.

The first is that **shared barriers make the modules correlated whether or not anyone intended them to be.** Reliability arithmetic that multiplies independent probabilities is not available when the items share a dependency, and a campus is built on shared dependencies for perfectly good economic reasons. This is the same structure as the correlated cutsets in [Module 5](../module-5-military-action-layer/02-correlated-barrier-cutsets.md), arriving here through consequence rather than through adequacy.

The second is that **the adversarial case selects for exactly this.** Something choosing where to act will choose the shared thing, for the same reason an engineer designing the campus chose to share it: because it serves everything. A demonstration resting on the unlikeliness of simultaneity is a demonstration that has assumed the absence of the one actor the military-action layer postulates.

So the corpus takes the aggregate position outright: the emergency-planning demonstration runs on **aggregate campus inventory under correlated defeat of shared barriers**, not on a single module's favorable arithmetic. The open form — because no endorsed guidance states it — is [LI-06](../../register/LI-06-aggregate-inventory-in-the-epz-demonstration.md).

## The same question in three vocabularies

Worth noticing, because seeing it once makes the other two easier.

Asked about **inventory**, it is this unit: does the dose calculation use one module's source term or the campus total?

Asked about **duration**, it is [LI-07](../../register/LI-07-assc-duration-on-aggregate-demand.md): does the passive coping window hold when every module demands the heat sink at once, rather than when one does?

Asked about **regulation**, it is [LI-08](../../register/LI-08-gdc-5-sharing-of-structures.md): what does the criterion on sharing structures, systems and components require when a site shares nearly everything?

One underlying question — what does sharing do to a demonstration built for a single unit — wearing three different sets of clothes. If the aggregate basis is settled once, all three move together, which is a reason to argue it on its merits rather than to concede it three times separately.

## The practical consequence for an applicant

Demonstrating on per-module inventory carries a specific risk, and it is a schedule risk rather than a safety one. If the first serious request for additional information forces a redemonstration on aggregate, it arrives late, after the site layout and the emergency plan have been built around a zone that may not survive. Redoing the calculation is cheap; redoing the siting is not.

Demonstrating on aggregate from the start is more conservative, more defensible, and — because this will be among the first genuine campus reviews — likely to become the referable precedent whichever way it is decided. An applicant who establishes the aggregate basis has shaped the ground everyone else will stand on.

## What a reviewer should press on

Which inventory basis the demonstration used, stated in one sentence near the front rather than reconstructable from an appendix.

Which barriers are shared across modules and which are genuinely per-module, as an enumeration rather than an assurance — and whether the analysis treats the shared ones as correlated.

And whether an argument from the unlikeliness of simultaneity is doing load-bearing work anywhere, since that argument is unavailable in the adversarial domain and its presence usually means the two domains have been quietly blended.

## What to carry forward

A campus is not a module, and the per-module source term does not carry to it. Two questions have to be separated: how much material is at stake, and whether the credited barriers are shared or per-module — the second decides the first. Shared barriers correlate the modules whether or not anyone intended it, and a deliberate actor selects for exactly the shared thing. The demonstration therefore runs on aggregate inventory under correlated defeat. And this is one question in three vocabularies: inventory here, duration at LI-07, regulation at LI-08.

Next: [Open Issues](open-issues.md) — the two entries this module governs, tightly coupled.
