# Course Note M04-CN-03 — Identifying Critical Digital Assets

**Anchor** — Core / Module 4 · unit 01 *Cyber Security under 10 CFR 73.54* · heading *Where the campus breaks the method*

**Source and locator** — Three sources, with three different provenances.

*The scoping guidance.* NEI 10-04, Revision 2, *Identifying Systems and Assets Subject to the Cyber Security Rule*, Nuclear Energy Institute, July 2012. Obtainable through the NRC's ADAMS public document system and through the Institute. Cited here by section number.

*The Commission's scoping determination.* Staff Requirements Memorandum COMWCO-10-0001, *Regulation of Cyber Security at Nuclear Power Plants*, 21 October 2010.

*The definition of adverse impact.* Regulatory Guide 5.71, *Cyber Security Programs for Nuclear Facilities*.

**Provenance and use** — NEI 10-04: published · **CHARACTERIZE ONLY**; no text of it is reproduced in this Note or anywhere on this site. The SRM and the regulatory guide: published · public domain (United States government works). One disclosure about the chain of quotation is made at the excerpt below.

**Companion** — [M04-CN-02](M04-CN-02-the-cyber-security-plan-template.md) covers the programme the cyber security plan establishes. This Note covers how an analyst decides what goes into it.

---

**Excerpt** — the Commission's policy determination on scope.

> The Commission has determined as a matter of policy that the NRC's cyber security rule at 10 CFR § 73.54 should be interpreted to include structures, systems, and components in the Balance of Plant that have a nexus to radiological health and safety at NRC-licensed nuclear power plants.

*Chain of quotation, disclosed.* This Note quotes the determination as it is reproduced in NEI 10-04, Revision 2, which sets it out in its Executive Summary and attributes it to SRM COMWCO-10-0001 of 21 October 2010. The wording has not been checked against the Commission's own copy of the memorandum. A reader relying on the exact phrasing should go to the SRM itself; a reader relying on the substance can rely on this, because the guidance was written to implement it and the industry would not have mischaracterised the instruction it was complying with.

One sentence of Commission policy, and it moves the outer edge of the rule. "Nexus to radiological health and safety" is a consequence test, not an equipment list, and it is the reason the scoping exercise reaches into the turbine hall at all.

---

**Characterization** — NEI 10-04, Revision 2: how the screening actually runs.

**Anchored to documents the licensee already has, in Sections 1.1 and 2.** Scoping is not conducted from first principles. Safety and important-to-safety functions are taken from the plant's current licensing basis — the safety analysis report and technical specifications; security functions from the criteria of 73.55 and the site's physical security plan; emergency-preparedness functions from 50.47(b) and Appendix E and the site's emergency plan. The guidance's contribution is a way of reading those existing documents for a purpose they were not written for.

**A screening questionnaire, in Section 4.** Plant systems are categorized by answering sets of questions. The safety screen turns on whether the system is relied on to remain functional during and following design-basis events to assure the integrity of the reactor coolant pressure boundary, the capability to shut down and hold safe shutdown, or the capability to prevent or mitigate accident consequences against the offsite-dose guidelines. The important-to-safety screen adds six further questions, among them whether a non-safety system's failure could adversely affect any of those three; whether it is in the primary success path for mitigating a transient; whether operating experience or a probabilistic risk assessment has shown its function significant to public health and safety; **whether it provides real-time or near-real-time plant status information to operators for safe operation during transients and accidents**; whether it is a balance-of-plant item that could directly or indirectly affect reactivity and result in an unplanned shutdown or transient; and whether it is required to maintain defense-in-depth and diversity requirements. Separate question sets cover security systems, emergency-preparedness systems, and support systems.

**What counts as *digital*, in Section 5.** A digital asset is a programmable device — the guidance instances erasable programmable memory and microprocessors — using some combination of hardware, firmware and software to execute internally stored programs and algorithms, including arithmetic or logic operations, without operator action. Solid-state devices that carry no firmware or software, the guidance naming electro-mechanical on/off devices, relays, hard-wired logic devices and circuit boards, are **not** digital devices. This is a definitional exclusion, not a judgement call.

**The pathway rule, which is what Revision 2 was issued to supply.** The revision history records that Section 5 was enhanced specifically to address the consideration of pathways as the term is used in the asset definition. The rule it lands on has three parts. A digital device that merely communicates with a critical asset is **not** a critical asset by reason of the connectivity alone. If compromise of that device could be used to compromise the critical asset, it **is** one. And where the cyber security controls applied under the plan's Section 3.1.6 address the threats associated with the pathway — such that the attack vector to the critical asset no longer exists — the device need not be classified. Inclusion by pathway is conditional and dischargeable, not transitive.

**A four-limb test, in Section 5.** A digital device should be identified as a critical asset if it performs regulated functions or its compromise would adversely affect one; or important-to-safety functions in the balance of plant whose compromise would produce an unplanned reactor shutdown or transient; or support functions such as primary and backup power, ventilation and fire protection whose compromise would adversely affect a regulated function; or the network boundary isolation, protection and detection functions described in the plan's defense-in-depth section. The fourth limb is worth pausing on: **the devices enforcing the defensive architecture are themselves in scope.**

**Adverse impact, and its carve-out, from Regulatory Guide 5.71 as Section 5 reproduces it.** Adverse impact means a direct deleterious effect on a critical asset — loss or impairment of function, reduced reliability, reduced ability to detect, delay, assess or respond, reduced ability to summon offsite assistance, reduced emergency-response ability to implement protective measures. The carve-out: where compromise causes a safety, important-to-safety, security, emergency-preparedness or support system to actuate or fail safe — to actuate properly in response to established parameters and thresholds — and does not result in radiological sabotage, that is not an adverse impact within the meaning of 73.54(a).

**Two notes to licensees, at the close of Section 5.** First, nothing in the guidance prevents a licensee from designating a component containing several digital devices, or a network containing several, as a **single** critical asset — provided the licensee justifies that the plan's protective requirements are satisfied for that configuration. Second, a licensee may find a single digital device type associated with **more than one Critical System, where those Critical Systems perform different regulated functions** — the example given being safety and emergency preparedness.

**Worked examples, in Appendices A and B.** Two tables categorize the systems of a generic pressurized-water reactor and a generic boiling-water reactor across the five columns the method uses. Both are watermarked as examples, are stated to derive principally from maintenance-rule documentation, and are stated not to be comprehensive; the guidance is emphatic that a site must perform its own analysis.

---

**What it establishes**

That scoping is a screening exercise run against the licensing basis, not an inventory exercise run against the plant. The questions in Section 4 are the method; everything downstream is consequence.

That "digital" has a bright definitional edge. Programmability is the test, and hard-wired logic is out — not argued out, defined out.

That the pathway clause is a valve rather than a net. This is the single most commonly misdescribed feature of reactor cyber scoping, and the misdescription runs in the direction of alarm: people assume connectivity propagates criticality transitively, so that anything touching anything critical is swept in. Revision 2 says it does not, and it gives the discharge condition — controls that remove the vector. That makes the identified population bounded and it makes the boundary architecture load-bearing, because the boundary devices are what discharge the pathways.

And that the outer edge of the whole exercise was set by Commission policy rather than by industry: the nexus-to-radiological-health-and-safety test in the SRM is what pulled balance-of-plant equipment into a rule that reads, on its face, as being about safety systems.

---

**Where the SMR case departs**

**Multiplicity is contemplated in exactly one direction — and it is the wrong one.** The second licensee note in Section 5 anticipates a single device type associated with more than one Critical System *where those systems perform different regulated functions*: safety and emergency preparedness, say. That is multiplicity of **function**. The campus case is a single asset associated with many Critical Systems performing the **same** function on different modules. The one place in the scoping guidance where an asset serving several Critical Systems is addressed points the other way, and offers the analyst no instruction for the case they actually have.

This is the precise statement of [LI-02](../../register/LI-02-campus-scaled-cda-identification.md), and it is a better one than "the method does not handle campuses." The method handles the campus asset perfectly well — it is unambiguously a critical asset. What it cannot express is that this critical asset is critical *twelve times over*, and it issues the same designation and points at the same control set either way. A gap stated as an absence invites the answer that the rule already covers it. A gap stated as **a designation with no gradation** names something a consensus process can actually build.

**The grouping mechanism is the nearest available handle, and its burden is undefined at this scale.** The first licensee note permits treating a network of devices as a single critical asset where the licensee justifies that the plan's protective requirements are met for the configuration. On a campus the natural grouping *is* the shared network, so the mechanism a campus applicant would reach for already exists. But the justification then has to hold for every module simultaneously, which is a far heavier claim than a note written for a single-unit cabinet contemplates. The vehicle exists; the standard for satisfying it does not. An applicant proposing to group at campus scale should expect to be asked what "the protective requirements are satisfied" means when the configuration spans twelve licensed units, and should propose the answer rather than wait for the question.

**Pathway discharge becomes a claim with a much larger surface.** Because classification can be discharged by showing that controls remove the attack vector, and because a campus multiplies both the vectors and the modules each vector reaches, the discharge argument has to hold against every reachable module. Nothing in Section 5 says so, because nothing in Section 5 imagined it. This is the same defect as the disposition-scope problem in [M04-CN-02](M04-CN-02-the-cyber-security-plan-template.md), arriving one level earlier in the analysis — at classification rather than at control selection — and it is the more consequential of the two, because an asset discharged at this step never reaches the control step at all.

**The digital-asset definition is a gift to the corpus's backstop argument and should be used as one.** Module 4 states, carefully, that a cyber compromise of shared instrumentation and control does not by itself defeat the credited passive safety function. Section 5's definitional exclusion of solid-state devices carrying no firmware or software supplies a regulatory basis for that claim rather than merely an engineering one: to the extent reactor trip and engineered safety actuation are implemented in hard-wired logic, they are outside the rule's scope **as a matter of definition**. That is a far stronger place to argue from, and an applicant should say it in those terms. The same precision cuts the other way and must be stated in the same breath: the claim holds only for the portions actually implemented that way, and a design that implements trip logic in a programmable device — however simple, however qualified — has no access to this argument at all. The corpus should not let the backstop drift into a general assurance about passive designs.

**The blinding residual already has a hook, and naming it changes the ask.** The important-to-safety screen in Section 4 asks whether a non-safety system provides real-time or near-real-time plant status information to operators for safe operation during transients and accidents. That question already reaches displays, alarms and the historian path — which is to say the corpus's common-cause blinding concern is **not a new category needing a new hook**. It is an existing screening question whose consequence analysis has never been run for a shift complement spread across a dozen modules. Reframing [LI-03](../../register/LI-03-shared-digital-ic-guidance.md) that way makes it markedly easier to close: the ask is not "write a new criterion," it is "run the existing criterion at campus scale and say what falls out."

**And the fail-safe carve-out has a campus edge worth raising as a question.** Proper actuation in response to established parameters is not an adverse impact. Per module that is plainly right. Twelve modules actuating correctly and simultaneously, because a shared input was manipulated to present each of them with parameters that genuinely warrant actuation, is not a safety event at any module and may be a substantial event on the grid — which sits across the jurisdictional seam described in [LI-14](../../register/LI-14-under-frequency-load-shedding.md). This is offered as a question the per-unit frame does not ask rather than as a finding; it has not been analyzed, and the corpus should not assert a consequence it has not demonstrated.

**Finally, the worked examples do not resemble the plant.** Appendices A and B categorize the systems of a generic large pressurized-water and boiling-water reactor. An applicant for a pool-immersed integral design or a dry passive-air design will find systems on those lists that do not exist in their plant and, more importantly, will find the lists silent on the ones that do. The guidance is explicit that the tables are illustrative and that site-specific analysis is required, so this is not a defect. It is a statement about effort: the screening questions transfer, the worked answers do not, and a first-of-a-kind applicant is doing from scratch the work an operating licensee does by analogy.

---

**Carry-forward**

The campus asset is not missed by the scoping method; it is flattened by it. One designation, one control set, and the only place the guidance contemplates an asset serving several Critical Systems contemplates several *functions* rather than several *units*. Naming the gap as a missing gradation — rather than as a missing rule — is what makes it something the consensus process can be asked to build.
