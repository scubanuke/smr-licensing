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

Two documents do the heavy lifting for reactor cyber security. One is the cyber-security plan template that structures the programme a licensee submits. The other is the scoping guidance that tells an analyst how to work out which digital assets are critical. A regulatory guide sits alongside them describing the security controls and the programme the Commission expects.

**A note on how this site treats those documents.** Industry consensus guidance is copyrighted. This site characterizes what a section requires, in its own words, with the section number, and does not reproduce the text — the rule and its reasoning are in [Conventions](../../CONVENTIONS.md). That constraint is honest rather than merely legal: characterizing a document accurately requires having read it, and a characterization written from secondary description is worse than none. Where this site's treatment of the guidance is thinner than it should be, that is why, and closing it means working from actual copies.

## Where the campus breaks the method

The facility-class design basis states three gaps in its cyber treatment, and the useful move — made in the corresponding submittal work product — is to decompose them rather than fold them into a single undifferentiated ask, because they have three different owners.

**Which assets are critical, when criticality scales with module count.** Single-unit scoping handles an asset that is critical for the unit it serves. It does not obviously handle an asset that is significant for one module and simultaneously consequential across twelve, and an analyst applying the existing method to a campus is improvising. This is a scoping-method question and it belongs to the consensus process: [LI-02](../../register/LI-02-campus-scaled-cda-identification.md).

**How you implement controls once you know.** Separate question, separate answer. Defense in depth for shared safety data paths, segmentation between enterprise information technology and safety instrumentation and control, common-cause treatment for a shared architecture, and the integrity of the historian and alarm streams that operators rely on. No campus-level implementation guidance exists. Also a consensus-process item: [LI-03](../../register/LI-03-shared-digital-ic-guidance.md).

**Whether the threat basis covers the adversary you are actually worried about.** State-actor pre-positioning — quiet access established long in advance — is not what the design-basis threat was drawn around. This one cannot go through the consensus process at all, because the threat basis is not industry's to set: [LI-04](../../register/LI-04-state-actor-pre-positioning.md).

The sequencing recommendation matters as much as the decomposition. Run the two tractable items in parallel and put the threat-basis calibration on a separate, slower track. A submittal that couples all three has effectively deferred all three.

## The backstop, stated carefully

There is a reassuring fact here and it has to be stated precisely, because both overclaiming and underclaiming do damage.

A cyber compromise of shared instrumentation and control does not by itself defeat the credited passive safety function. Reactor trip and engineered safety actuation are engineered to operate on plant conditions through deterministic logic, independent of the digital and generative layer — they sit below the autonomy boundary that [The Dual Design Basis](../module-5-military-action-layer/03-the-dual-design-basis.md) calls the Bright Line. An attacker who owns the business network does not thereby own the trip.

The residual that does exist is different in kind and easy to underrate: **common-cause blinding.** Corrupted monitoring, falsified alarms, a compromised historian, against a shift complement already stretched across many modules. The plant still protects itself; the people responsible for it can no longer see what is happening or trust what they are told. In the bounding cyber-kinetic event the corpus postulates, that blinding is the enabling first move rather than the damaging one.

Overclaiming the threat invites a reviewer to demand protection the physics does not require. Underclaiming it leaves the blinding residual undocumented. The defensible position is the narrow one: the trip is not defeated, and situational awareness very much can be.

## What a reviewer should press on

Whether the critical-digital-asset identification addresses campus scaling explicitly or quietly applies single-unit scoping to a configuration it was not written for.

Whether any credited operator action depends on a display, an alarm, or a historian that the cyber analysis concedes could be corrupted — the question that turns the blinding residual from an abstraction into a finding.

And whether the three gaps arrive with three vehicles and three owners, or as one ask addressed to nobody.

## What to carry forward

The rule turns on identifying critical digital assets, and the method for doing so lives in endorsed industry guidance rather than in the regulation. A shared campus breaks that method in two separable ways — which assets are critical, and how to implement controls on a shared architecture — and raises a third question about the threat basis that only the Commission can answer. The trip survives a cyber compromise; the operators' picture of the plant may not.

Next: [Safeguards Information](02-safeguards-information.md), which decides how much of any of this can appear on a public docket.
