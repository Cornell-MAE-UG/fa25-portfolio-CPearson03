---
layout: project
title: Open Design Project
description: Outline of our proposed solution for the New York vineyard owners' Spotted Lanternfly problem
technologies: [CAD]
image: "/assets/images/SLF_Project/ODP_Image.png"
---
**Team: Spotted... then Stopped**





---


#### Milestones

- Click [here](#client-pitch) for client pitch assignment (or here to [view as PDF]({{ "/assets/images/SLF_Project/Client_Pitch.pdf" | relative_url }}))
- Click [here](#functional-prototype) for functional prototype assignment (or here to [view as PDF]({{ "/assets/images/SLF_Project/Functional_Prototype.pdf" | relative_url }}))

---


<a name="client-pitch"></a>
## Client pitch


###### Problem Statement


New York vineyard operators aim to maximize yield during mechanical harvesting, but Spotted Lanternflies (SLF) frequently enter harvest bins and contaminate products. A Cornell–Penn State study found that 60% of lanternflies on vines end up in harvest bins, and current standards require rejection if even 1–2 adult insects are found per 1 kg sample. Significantly disturbing the vine to remove SLF's proves a problem when harvesting. Ripe grapes detach very easily, potentially resulting in high losses if they are directly exposed to excessive forces.


---


###### Impact


Reducing contamination during the harvesting process leads to less wasted product and maximizes yield.


---


###### Proposed Direction


Our main idea is to have a machine attached to the front of the harvester that would get rid of the flies right before the grapes are collected.


---


###### Concept: Spinning Brushes


An attachment to the front of the vehicle that has rotating brushes aimed at only the vine. The brushes would be located on a rotating rod (almost like a car wash brush) that scrapes the flies off the vine, placed at the right height so as to not disturb the grapes too much.


---


###### How it would be used


Mount system to harvester front


Attach height to match vine height


Brushes rotate at speed matched to forward motion


Flies are dislodged downward before grape collection


---


###### Why it’s better than the status quo


Removes insects before contamination


Avoids post-harvest filtering grapes and flies


Compatible with current harvesting equipment


---


###### End-of-semester proof-of-concept


Two cylindrical brushes attached to an adjustable mounting frame, spinning in tandem.


---


###### Key Risks / Unknowns


**Damage to vines** — Reduce yield if the vine is scraped: Test bristles on vine and assess damage.  


**Knocking off grapes prematurely** — Accidental removal of grapes: Test to ensure right height of bristles to avoid contact with grapes.


**Gaps between brushes may leave some flies on vines** — Might still leave some contamination: Test prototype on model of the vine with attachments of similar grip strength to SLF.


---


###### Questions for the client


**Can we get a blueprint/design for the harvesters used?** — Affects how the brush would mount the harvester, and design considerations that come with that.


**What is the average height/length of the vine?** — Affects the dimensions of the brush and the amount of materials needed.


**What is the durability of the vine?** — Affects the amount of force we can put on the vine and the material used for the bristles.




---


###### References


- [WineAmerica 2025 Methodology](https://wineamerica.org/wp-content/uploads/2025/05/2025-WineAmerica-Methodology-4-28-25-Final.pdf)

- [PSU: Grapevines may only need help to survive heavy spotted lanternfly infestations](https://www.psu.edu/news/research/story/grapevines-may-only-need-help-survive-heavy-spotted-lanternfly-infestations)



---

<a name="functional-prototype"></a>
## Functional Prototype


#### Purpose

The primary purpose of our prototype was to test the effectiveness and ease of assembly for the brush and shaft feature of our design. This feature is critical to the success of our design which is why we made it a priority to make a prototype before we progressed with big decisions such as purchasing motors and creating a bracket, which would be dependent on our findings.

This feature requires the most attention to detail in terms of fabrication, as the 3D printed shaft has to be toleranced in such a way that the brushes fit into the slots without excessive force, but are also secure enough that they do not come loose under working loads. From our testing, we also wanted to confirm the feature would be a suitable method of incorporating the strip brushes, and  that it would be effective in removing SLF when in motion. Finally, we wanted to create the prototype so we could get a gauge of what size motor would be required to run the brush for our chosen operating rate.




#### Tests and Outcomes:

---

##### Functional test — Brushes &nbsp; `Passed`

**What we tested:** Effectiveness of the brush at sweeping objects off a cylindrical surface.

**How:** Stuck 5 sticky-note rings (2 cm wide) onto a rod. Counted removals after ~10 revolutions. Repeated 3 times. Pass threshold: ≥ 4/5 removed.

**Results:**
- Trial 1: 3/5 removed
- Trial 2: 5/5 removed
- Trial 3: 5/5 removed

**Conclusion:** Brush stiffness is correct. Found that bristle length was too short — objects must be very close to the shaft to be reached. New longer brushes to be ordered for next prototype.

---

##### Assembly test (snugness of fit) — Brushes & shaft slots &nbsp; `Passed (v2)`

**What we tested:** Tolerancing between the brush base and shaft slot — looking for snug fit with no large gaps.

**How:** Inserted brushes into slots and measured gap using progressively folded paper strips until none would fit. If test fails, redesign shaft slots and print new shaft to repeat test.

**Results:**
- Print 1: **Failed** — zero gap, excessive force required, slot partially snapped
- *Changes for print 2: slot length increased by 1.27 in, edges smoothed*
- Print 2: **Passed** — smooth insertion, gap ≈ 1 sheet of paper

**Conclusion:** ~1 sheet of paper clearance gives the best balance of ease and secure retention. Current shaft design is ready to move forward; top and bottom details depend on final motor and arm design.

---

##### Torque test — Motor &nbsp; `Passed`

**What we tested:** Minimum torque needed to initiate shaft rotation at target speed.

**How:** Applied progressively heavier weights to a 1.75 cm crank arm until the shaft turned.

**Results:**
- 50g attached → no rotation
- 100g attached → rotation achieved
- Torque required: **T = 0.02 Nm**

**Conclusion:** A low-power motor will suffice. Torque will be higher once arm friction is included — re-evaluate after arms are fabricated.

---