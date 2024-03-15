## Theorems of Digital Democracy
Prepared by Brendan A. Miller on 3/14/24 in Los Angeles, CA.
Website: https://brendanmiller.com


### BACKGROUND:

These theorems are based on Brendan's prior research and work for 2Gather. Specifically the document entitled "Can I Trust this Software?" which was published on the [2Gather website](https://2gather.one/can_i_trust_this_software.pdf) as well as on [Github](https://github.com/2gatherproject/2gather-project-documentation/commit/ed7bc06559fee63e5d37d9d1747f00c75b8ea333) on June 12, 2021, and then [revised](https://github.com/2gatherproject/2gather-project-documentation/commit/eddf4bb6b76871612ffc905f182835db804089ab) on November 19, 2023.


### DEFINITIONS:

* **Democracy** is defined as government by the people, or alternately as governance by a group of people over their own affairs.
* **Group of people** is defined as any collection of people, of any size, from 1 person up to possibly including every person who has existed in the past, exists now, or will exist in the future.
* **Protecting democracy** is defined as ensuring that, for a given group of people, that the decision making by the group and execution of their decisions are goverend and managed by that group only, without unwanted influence from outside the group.
* **Digital infrastructure** is defined as as any digital hardware, software, networking, data stores or other digital processing equipment or data used in performing functions for one or more groups of people.
* **Centralized infrastructure** is defined as digital infrastructure that is shared by two or more groups of people.
* **Decentralized infrastructure** is defined as any digital infrastructure that is used exclusively by one group of people in the process of governing their own affairs.

NOTE: An important note on the word "shared." We should assume that infrastructure should be fully disjoint between groups in order to not be considered "shared." It is possible that certain technological solutions such as confidential computing, end-to-end encryption, virtual private networks, etc. may be able to provide acceptable compromises for some groups so that infrastructure that is physically shared may be considered "logically" disjoint. This may vary depending on their cost sensitivity, their perceived need for privacy and security in their work, performance considerations, etc. Development of technologies like these over time may also change which groups consider which physically shared infrastructure to be logically disjoint.


### THEOREMS:

1. Protecting democracy requires decentralized digital infrastructure.

2. Protecting democracy requires the ability to discern data provenance, specifically which human was responsible for submitting a given piece of data into a digital system.

3. Protecting democracy requires the ability of a person to have full control over their data (e.g. granulary granting/delegating access rights to specific people for specific purposes, revocation of delegation, encryption, signatures)

4. Protecting democracy requires that software that performs functions or processes data for a group be inspectable and auditable by the members of the group (e.g. open source, reproducible builds).

5. Protecting democracy requires that software used by a group be able to be modified by that group to meet their evolving needs.


### PROOFS BY CONTRAPOSITION:

#### 1.
Assume there is some centralized infrastructure involved in some democratic group decision making or implementation process.

It is possible for a malicious actor outside of the "democratic boundary/jurisdiction" to gain access to the data flowing through this infrastructure, allowing them to
* interrupt the flow of vital data,
* inject false/malicious data,
* surveil the data and have access to information that can be abused either inside or outside of the system,
* or to actively manipulate the system in order to cause harm.

In other words, this malicious actor can disrupt the democratic decision making and effective operation of the group in question, rendering it undemocratic.

QED

#### 2.
Assume there is a possibility that we do not know where even one piece of data comes from that is involved in a group process.

This means that a malicious actor outside of the system could insert/alter/manipulate that piece of data in such a way as to confuse or bias an essential analysis for the group. Consider a situation where an outcome is binary in nature with a close balance of data on each side. The malicious actor could inject a piece of data that sways the result from the correct outcome to alternative incorrect outcome.

This could also happen if a person within the group tried to alter the outcome in a similar way.

Therefore the democratic operation of the group has been undermined if we cannot determine where data comes from, regardless of whether that data comes from the outside or inside the group.

NOTE: Software code is a form of data and subject to the same analysis. Attestation and verification of running software is also required for this reason.

QED

#### 3.
Assume that a person (the actor) does not have full control over their data, even within a chosen group.

The trivial case of faking a digital signature is obvious and well understood: any group member could pretend to be the actor and incorrectly attribute it to that person. Votes could be altered, etc. This clearly undermines democracy.

Also, consider if a piece of private data from the actor that was shared in confidence (not publicly, but only within the group) could be retained by other group members against that person's wishes, and proved to come from the actor (e.g. for example via the true digital signature). This could prevent the actor from changing their mind (for example, within the allowed timeline for a decision process). This could undermine a democratic process that requires a group come an agreed decision via a deliberative process. Either it would seem as if the actor might have voted twice, or that their preliminary and final decisions were swapped.

(This needs more work and better examples. It also needs to define and consider all conditions of "full control".)

Thus democracy is undermined.

QED

#### 4.
Assume that the software used by a group cannot be fully inspected or audited.

Then the software could be modified one an outside malicious actor or by a group member who wishes to bias the software in their favor.

Therefore democracy is undermined.

QED.

#### 5.
Assume that the software used by a group cannot be modified by them for some reason (it is not being maintained, or the maintainer refused to service their request, etc.).

The group changes over time, and new conditions in their situation arise. For example new requirements or opportunities emerge.

The software was not built to consider these requirements or opportunities.

Therefore the software cannot support the group in effectively making decisions, for example because certain options cannot be considered or because certain operations are impossible.

Therefore democracy is undermined.

QED
