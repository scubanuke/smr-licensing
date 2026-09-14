# Cyber Security under 10 CFR 73.54

Reactors run on digital equipment, and some of that equipment matters more than the rest. The regulatory approach is to say so explicitly: identify the digital assets whose compromise could hurt safety, security, or emergency preparedness, protect those to a high standard, and demonstrate that you have. Everything in the cyber-security rule follows from that first sorting step.

The sorting step was designed when a site meant one reactor, or two. A small modular campus may run a dozen modules from one control building on shared infrastructure, and an asset that is significant for one module and *decisive for all twelve at once* does not sit comfortably anywhere in the existing method. Most of what is unresolved here traces back to that.

## The structure of the rule

10 CFR 73.54 requires a licensee to protect digital computer and communication systems and networks associated with safety and important-to-safety functions, security functions, emergency preparedness including offsite communications, and the support systems whose compromise would affect any of those.

The obligations it imposes are a programme rather than a control list: identify the assets in scope, analyze them, apply security controls, defend in depth, be able to detect and respond to and recover from an attack, and keep all of that current as the plant changes. The plan is submitted and approved, which makes it enforceable, and it is inspected against.

The pivot in the whole scheme is the **critical digital asset** — the category that determines what gets the full weight of protection. Getting that identification right is the difference between a programme that protects what matters and one that spends its effort evenly across everything and therefore thinly on the parts that count.

## How industry guidance becomes review guidance

Very little of the method for doing this lives in the regulation itself. It lives in industry guidance that the Commission has endorsed, and understanding that mechanism explains a great deal about how the open issues in this module will actually be closed.

The pattern is that the Nuclear Energy Institute develops a guidance document through its consensus process, the Commission reviews it, and if the Commission finds it acceptable it endorses it — typically through a regulatory guide, sometimes with exceptions or clarifications. From that point the endorsed method is an accepted way of complying: an applicant who follows it can say so, and the staff reviews against a known yardstick rather than evaluating a bespoke approach from first principles.

Two documents do the heavy lifting for reactor cyber security. NEI 08-09 is the cyber-security plan template that structures the programme a licensee submits. NEI 10-04 is the scoping guidance that tells an analyst how to work out which digital assets are critical. Regulatory Guide 5.71 sits alongside them describing the security controls and the programme the Commission expects. Each is characterized in its own Course Note: [M04-CN-02](../../resources/course-notes/M04-CN-02-the-cyber-security-plan-template.md) for the plan template, [M04-CN-03](../../resources/course-notes/M04-CN-03-identifying-critical-digital-assets.md) for the scoping method.

**A note on how this site treats those documents.** Industry consensus guidance is copyrighted. This site characterizes what a section requires, in its own words, with the section number, and does not reproduce the text — the rule and its reasoning are in [Conventions](../../CONVENTIONS.md). That constraint is honest rather than merely legal: characterizing a document accurately requires having read it, and a characterization written from secondary description is worse than none. The two Notes above are written from copies of the documents, which is why they are able to say where the corpus's own earlier description of the scoping construct was wrong.

**One correction, stated plainly, because it matters.** The common account of critical-digital-asset scoping holds that connectivity propagates criticality — that anything with a path to a critical asset is swept in, and that campus architecture therefore produces an unmanageable population. That is not what the guidance says. Revision 2 of the scoping document was issued in part to settle exactly this question, and it settles it the other way: a device that merely communicates with a critical asset is not critical for that reason alone; it is critical if its compromise could be used to compromise the critical asset; and where controls remove the attack vector, the classification is discharged. Inclusion by pathway is conditional and dischargeable. An applicant who argues from the alarming version of this will be corrected, and will have spent credibility to no purpose.

## Where the campus breaks the method

The facility-class design basis states three gaps in its cyber treatment, and the useful move — made in the corresponding submittal work product — is to decompose them rather than fold them into a single undifferentiated ask, because they have three different owners.

**Which assets are critical, when criticality scales with module count.** The shared asset is not missed by the existing method — it is plainly critical, and no argument is needed to make it so. The difficulty is that the method has one designation to issue and issues it either way. An asset whose compromise reaches one module and an asset whose compromise reaches all twelve are classified identically, documented identically and protected identically. The one place the scoping guidance contemplates an asset serving several critical systems contemplates several *functions* — safety and emergency preparedness, say — rather than several *units*, so an analyst on a campus has the nearest analogue pointing the wrong way. Stated as a missing gradation rather than a missing rule, this is something the consensus process can be asked to build: [LI-02](../../register/LI-02-campus-scaled-cda-identification.md).

**How you implement controls once you know.** Separate question, separate answer. Defense in depth for shared safety data paths, segmentation between enterprise information technology and safety instrumentation and control, common-cause treatment for a shared architecture, and the integrity of the historian and alarm streams that operators rely on. No campus-level implementation guidance exists. Also a consensus-process item: [LI-03](../../register/LI-03-shared-digital-ic-guidance.md).

**Whether the threat basis covers the adversary you are actually worried about.** State-actor pre-positioning — quiet access established long in advance — is not what the design-basis threat was drawn around. This one cannot go through the consensus process at all, because the threat basis is not industry's to set: [LI-04](../../register/LI-04-state-actor-pre-positioning.md).

The sequencing recommendation matters as much as the decomposition. Run the two tractable items in parallel and put the threat-basis calibration on a separate, slower track. A submittal that couples all three has effectively deferred all three.

## The backstop, stated carefully

There is a reassuring fact here and it has to be stated precisely, because both overclaiming and underclaiming do damage.

A cyber compromise of shared instrumentation and control does not by itself defeat the credited passive safety function. Reactor trip and engineered safety actuation are engineered to operate on plant conditions through deterministic logic, independent of the digital and generative layer — they sit below the autonomy boundary that [The Dual Design Basis](../module-5-military-action-layer/03-the-dual-design-basis.md) calls the Bright Line. An attacker who owns the business network does not thereby own the trip.

That claim has a regulatory footing and not merely an engineering one, which is worth knowing because it is the stronger ground to argue from. The scoping guidance defines a digital asset by programmability, and excludes solid-state devices carrying no firmware or software — relays, hard-wired logic, bare circuit boards — from the category outright. To the extent trip and actuation logic is implemented that way, it is outside the rule's scope by definition rather than by argument. The precision cuts both ways and has to be stated in the same breath: the argument is available only for the portions actually implemented in hard-wired logic, and a design that puts trip logic in a programmable device, however simple and however qualified, cannot reach for it at all. This is a claim about a specific implementation, never a general assurance about passive designs.

The residual that does exist is different in kind and easy to underrate: **common-cause blinding.** Corrupted monitoring, falsified alarms, a compromised historian, against a shift complement already stretched across many modules. The plant still protects itself; the people responsible for it can no longer see what is happening or trust what they are told. In the bounding cyber-kinetic event the corpus postulates, that blinding is the enabling first move rather than the damaging one.

Overclaiming the threat invites a reviewer to demand protection the physics does not require. Underclaiming it leaves the blinding residual undocumented. The defensible position is the narrow one: the trip is not defeated, and situational awareness very much can be.

## What a reviewer should press on

Whether the critical-digital-asset identification addresses campus scaling explicitly or quietly applies single-unit scoping to a configuration it was not written for.

Where an applicant has grouped several devices or a whole shared network into a single critical asset — a move the guidance permits on a documented justification — whether that justification is shown to hold for every module at once, or only for the configuration in the abstract.

Whether any pathway classification has been discharged on the ground that controls remove the attack vector, and if so whether the discharge was tested against every module the pathway reaches rather than the one being analyzed.

Whether any credited operator action depends on a display, an alarm, or a historian that the cyber analysis concedes could be corrupted — the question that turns the blinding residual from an abstraction into a finding.

And whether the three gaps arrive with three vehicles and three owners, or as one ask addressed to nobody.

## What to carry forward

The rule turns on identifying critical digital assets, and the method for doing so lives in endorsed industry guidance rather than in the regulation. A shared campus does not escape that method — it flattens against it, because the method has one designation to issue and no way to say that an asset is critical twelve times over. That is the first of two separable gaps; the second is how controls are implemented on a shared architecture once the assets are known. A third question, about whether the threat basis reaches the adversary that matters, only the Commission can answer. The trip survives a cyber compromise, and by definition rather than by argument where the logic is hard-wired; the operators' picture of the plant may not.

Next: [Safeguards Information](02-safeguards-information.md), which decides how much of any of this can appear on a public docket.
