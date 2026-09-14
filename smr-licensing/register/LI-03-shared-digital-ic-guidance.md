# LI-03 — Shared Digital Instrumentation and Control Guidance

Once several reactor modules share the same digital instrumentation and control architecture, a weakness in that architecture is a weakness in all of them at the same moment. Traditional plant design handles failure by having more than one of everything; that works when failures are independent, and works much less well when one shared thing fails for all units at once because somebody made it fail. There is no implementation guidance written for that configuration.

**The issue** — No campus-level implementation guidance exists for the defense-in-depth, segmentation, and common-cause treatment of digital instrumentation and control shared across reactor modules.

**Where it surfaces** — DBA-MA-SMR-FC1 §7.4, second of the three stated gaps. The technical treatment sits in the Three Threads cyber-security instrument; candidate work product 1B routes it.

**Regulatory hook** — 10 CFR 73.54, implemented through the endorsed industry cyber-security plan guidance.

**Why it is open** — **Guidance is absent.** Distinct from [LI-02](LI-02-campus-scaled-cda-identification.md), which asks *which* assets are critical; this asks how you implement controls once you know. Separating the two is the point of 1B — the undifferentiated single ask in FC1 §9.5 routed to nobody in particular.

**Closure vehicle and owner** — A campus addendum to the industry cyber-security plan guidance, organized around the three-domain structure the corpus uses — structures, systems and components; software applications; target set — covering defense in depth for shared safety data paths, segmentation between enterprise information technology and safety instrumentation and control, common-cause failure treatment, and the integrity of historians and alarm streams. **Owner: the Nuclear Energy Institute**, developing; Commission endorsing.

**State of play** — *As of September 2026.* Open. Candidate 1B is drafted at v0.1. The corpus states a design backstop and states it carefully: a cyber compromise of shared instrumentation and control does not by itself defeat the credited passive safety function, because reactor trip and passive actuation are engineered independent of the digital layer. The residual it does identify is common-cause *blinding* — corrupted monitoring, alarms, and historians against an overextended shift complement — which is the enabling first move in the bounding cyber-kinetic event rather than the damaging one.

## Reader's stake

*For the practitioner* — The honest framing matters more here than anywhere else on the register. Overclaiming the threat invites a reviewer to ask for protection the physics does not require; underclaiming it leaves the blinding residual undocumented. The instrument's position — trip and passive actuation sit below the autonomy boundary and are not defeated by the digital layer, while situational awareness is — is the defensible middle and should be stated as such.

*For everyone else* — Sharing control equipment among a dozen small reactors is efficient and it concentrates risk. The reassuring part is that the reactors' automatic shutdown does not depend on the computers an attacker would target. The unresolved part is that the operators could be left unable to see what is happening, and no one has written the rules for guarding against that at this scale.
