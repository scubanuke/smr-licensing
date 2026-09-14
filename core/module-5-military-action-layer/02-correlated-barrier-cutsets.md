# Correlated-Barrier Cutsets

Nuclear plants are built on a simple and powerful idea: if one of something can fail, have several, and arrange them so that whatever kills one does not kill the others. Two pumps on different power supplies in different rooms. Three instrument channels voting. A backup for the backup. The arithmetic is what makes reactor safety work — if each barrier fails rarely and independently, all of them failing together is vanishingly unlikely.

The arithmetic depends entirely on the word *independently*. An adversary is not independent. An adversary looks at the same design, finds the one thing all three pumps quietly have in common, and takes that.

## The adversary as a common-cause failure

Safety engineering already knows about dependent failure. Common-cause failure — a single condition defeating several redundant items at once — is a recognized category, and a good deal of effort goes into finding and eliminating it: diversity in components, separation in space, independence of support systems.

The right way to place a deliberate adversary in that framework is as a **deliberate common-cause failure**. Not a new and exotic category, but the familiar one with its selection mechanism changed. Ordinary common-cause failure arises from shared design defects, shared environments, shared maintenance errors — conditions that happen to be shared. A deliberate adversary searches for what is shared and acts on it.

That reframing is worth more than it first appears, because it means the analytical machinery already exists. Common-cause analysis knows how to look for shared dependencies. What changes is the selection rule: instead of asking which shared dependency is likely to manifest, you ask which one an intelligent actor would choose.

## Cutsets, and why they are the right unit

A cutset is a set of failures that, taken together, defeats a function. A minimal cutset is one with nothing spare in it — remove any member and the function survives. Reliability analysis uses cutsets routinely; what this module adds is the question of which cutsets are *selectable*.

A **correlated-barrier cutset** is a cutset whose members share something a single act can reach. Four kinds recur often enough to be worth looking for by name.

**Shared supports.** Redundant trains that both depend on the same service water header, the same instrument air, the same direct-current supply. The trains are independent; their supports are not.

**Shared bays.** Physical co-location. Two divisions separated electrically and functionally, and then installed on either side of the same wall, reachable from the same place.

**Shared feeds.** Common electrical sources, common makeup inventory, common ultimate heat sink. This is the one that bites hardest on a multi-module campus, where the heat sink may be shared across every module on the site.

**Shared paths.** Cable routes, penetrations, corridors, and — increasingly — data paths. Two channels that are genuinely independent as designed can run through the same conduit.

## The adequacy question, restated

Once cutsets are the unit, the adequacy question changes shape in a way that is easy to state and uncomfortable to answer.

The old question is whether a credited function has enough redundancy. The new question is whether any credited function survives the loss of every member of a selectable correlated cutset. And the practical consequence is the one that catches designers out: **adding a redundant train that runs through the same shared bay does not reduce the cutset**. It adds cost, it improves the random-failure number, and it changes nothing at all about the deliberate case.

Reviewers should expect to see this argued the wrong way round. The instinct when a correlated-cutset finding appears is to propose more redundancy, because that is what has always worked. The demonstration that actually answers it is a dependency argument: here are the credited functions, here is everything each depends on, here are the minimal sets an actor could select, and here is what remains when each is removed.

## Where this lands for a campus

Nothing about the method is specific to small modular reactors. What is specific is the degree of sharing. A twelve-module campus with one control building, one service water system, one heat sink and one electrical distribution has correlated cutsets that a two-unit station simply does not have, and they reach across modules rather than within one.

This is why [LI-08](../../register/LI-08-gdc-5-sharing-of-structures.md) is load-bearing for so much else on the register. The General Design Criterion on sharing among units is the regulatory hook, and the reason the criterion is hard to apply here is precisely the reason the cutset analysis is necessary: the criterion asks whether sharing significantly impairs the ability to perform safety functions, and answering it at this degree of sharing requires exactly the dependency map described above.

Two adjacent entries are the same analysis in other clothes. [LI-15](../../register/LI-15-simultaneous-multi-module-trip.md) asks about the reliability of all modules tripping at once, which cannot be answered by multiplying single-unit reliabilities because that multiplication assumes the independence shared signals and shared actuation supports remove. And [LI-07](../../register/LI-07-assc-duration-on-aggregate-demand.md) asks how long the passive window lasts on aggregate demand, which is the heat-sink cutset expressed as a duration instead of as a failure.

## A decision-maker is a barrier too

The most useful extension of this idea came out of review comment on the warning-pathway work, and it generalizes further than it was first meant to.

If the plan for a deliberate event requires a cleared, pre-authorized person to decide something — to initiate a transition, to authorize a protective action — then that person is a credited barrier, and the cutset analysis applies to them. A single decision-maker in a single location is a single point of failure that one strike, one seizure, or one communications loss removes. The answer is the same answer as for any other correlated cutset: several of them, separately located, each independently able to act.

This is worth holding on to because it is the point at which the method stops being about hardware. Anything the response depends on — a person, an authority, a communications link, an assumption that someone will arrive — is a barrier, and the four kinds of sharing above apply to all of them. The corpus's treatment of this is in [LI-11](../../register/LI-11-the-warning-pathway-and-who-decides.md).

## What to carry forward

An adversary is a deliberate common-cause failure that selects which barrier to take first. The unit of analysis is the correlated cutset — barriers sharing supports, bays, feeds or paths — and adequacy means a credited function survives the loss of a selectable one. Redundancy inside a shared dependency is not redundancy. And barriers include people, authorities and assumptions, not only equipment.

Next: [The Dual Design Basis](03-the-dual-design-basis.md), where a second design basis arrives and the seam between the two has to be governed rather than assumed.
