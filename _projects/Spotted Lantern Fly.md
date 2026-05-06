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
- Click [here](#client-report) for client report assignment (or here to [view as PDF]({{ "/assets/images/SLF_Project/Client_report.pdf" | relative_url }}))


---

#### Project Description

In this project, we developed a mechanical solution to help vineyard operators in North America mitigate the impact of Spotted Lanternflies (SLF) during harvesting. These invasive pests not only damage grapevines throughout the growing season but also contaminate harvested crops, leading to costly rejection under strict quality standards.

The key challenge is removing SLF immediately prior to harvest without disturbing the vines or dislodging ripe grapes, which are highly susceptible to damage. Our approach focuses on a front-mounted, brush-based attachment for mechanical harvesters that selectively clears insects from the vine moments before collection. The system is designed to integrate with existing harvesting equipment while maintaining yield, reducing contamination risk, and minimizing additional labor or processing requirements. 


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

<a name="client-report"></a>
## Client Report

###### Context and Problem Statement
Due to limitations in the labour force, New York vineyard operators use mechanical harvesters rather than hand-picking grapes. This allows Spotted Lanternflies (SLF) to frequently enter harvester bins and contaminate the yield. A Cornell–Penn State study found that 60% of lanternflies on vines end up in harvester bins, and current standards require rejection if even 1–2 adult insects are found per 1 kg sample. This leads farmers to invest a season's worth of resources in a crop, only for it to be rejected due to late-stage contamination. Addressing this issue reduces uncertainty in harvest outcomes, allowing farmers to plan and allocate resources with greater confidence. It will also invariably lead to higher profits as fewer crops will be rejected due to contamination.

<figure style="float: right; width: 300px; margin: 0 0 1em 1em;">
  <img src="{{ site.baseurl }}/assets/images/SLF_Project/Vines.png"
       alt="Vines"
       style="width: 100%; height: auto;">
</figure>

Significantly disturbing the vine to remove SLF's proves a problem when harvesting, as ripe grapes detach very easily, potentially resulting in losses if directly exposed to excessive forces. Thus we have tailored our design to vertical shoot positioning trellis systems, which have long vines, with grapes growing above a set level, allowing us to target the vine without 

---

###### Final Prototpe and Application
Our prototype consists of two motorized brushes that mount onto the front of a harvester. As the harvester travels through the field, it removes SLF from the vine moments before the grapes are harvested, ensuring no lanternflies contaminate the crop. Each attachment is modular in design, with key features being the shaft and the strip brushes. Shafts have been 3D printed with slots to hold strip brushes in place, allowing the quick and easy replacement of brushes without compromising on snugness of fit. Shafts are also split into two parts - allowing farmers to adjust for different vine dimensions by simply changing the length of the brushes fitted in the shaft. The shafts are suspended by a top and bottom bracket, which attach to the front of the harvester.

<figure style="float: right; width: 300px; margin: 0 0 1em 1em;">
  <img src="{{ site.baseurl }}/assets/images/SLF_Project/Prototype.png"
       alt="Prototype"
       style="width: 100%; height: auto;">
</figure>

In practice, farmers will determine the required brush length based on vine dimensions and how low-hanging the grapes are. The brushes should only contact the vine and therefore not disturb the grapes growing above. The farmer will then insert them into the shaft and mount the modules onto the harvester. As the harvester travels through the vines, the motorized brushes sweep in an outward direction, ensuring all SLF are directed away from the harvesting bins. While the prototype motors are powered by a mains supply, a deployed system would draw power directly from the harvester’s onboard electrical system.

---

###### Conclusion and Recommendation
From testing our prototype, it displays clear potential for solving the subproblem we have identified. One primary success criteria we judged our design on was its ability to remove objects from vine-like structures. In our functionality test, it removes up to 80% of sticky notes and 70% of paper clips - two objects with similar length scales and resistance to removal as SLF. Another success criteria we judged our design on was how easy the shaft and brushes were to assemble. In the assembly test, it took 41 seconds to replace the brushes and around 4.5 minutes to mount on the brackets. Since mounting on the brackets will only have to be done once per harvest, we have judged this is a reasonable amount of time and therefore meets the success criteria. Alongside meeting our success criteria, our design is very financially viable. It requires only a one-time setup, attaching it to the front of the harvester, and from there, the only upkeep would be brush replacement, which, due to the modularity of our design, is very quick and simple. Likewise, vineyard owners would only have to purchase one of these per harvester and replace brushes as needed.

Despite our primary success criteria being met, we believe our prototype requires further development before field testing. One major aspect our current design is missing is a mounting system for the harvester. For future iterations of our design we would make a metal frame to attach the arms to the harvester and also make the shaft and arms out of a lightweight weather-resistant material. This would make our design more structurally robust and able to withstand the higher loads experienced on high powered machinery. Once these adjustments have been made we would be able to perform field tests to validate our lab results under real conditions. 

Overall, we recommend our design should continue to be developed, with improvements primarily focusing on the mounting system and also structural integrity. After these have been implemented, field tests should be conducted.

---

###### Testing and Results
To test the validity of our success we completed: a functional test, an assembly test and a rupture test.

Functional test: 
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/images/SLF_Project/bar_chart.png"
       alt="bar_chart"
       style="width: 100%; max-width: 600px; height: auto;">
</figure>
For the functional test we passed a tube through rotating brushes with different types of attachments, modeling the lantern flies. The attachments were differentiated by how strongly they stick to the vine to evaluate different grip strengths. We also examined which orientation of brush rotation would be most effective in removing the most attachments. For the 3 different attachments, we found that outwards rotation was the most effective, therefore, this is what we used for our final design and what we recommend for harvesters. 

Assembly test:
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/images/SLF_Project/table.png"
       alt="table"
       style="width: 100%; max-width: 600px; height: auto;">
</figure>
For our assembly test, we wanted to make sure that the modular aspect of the design was highlighted. We completed the test by doing three timed trials of replacing brushes and mounting the brushes onto the bracket. We found that replacing brushes took an average of 41 seconds, showing how time effective this design is as this is the only part of the design that will need to be replaced in the long term. This passed our success criteria as we were able to replace the brushes under a minute. Additionally, we found that the average time for the brushes to be mounted onto the bracket was around 4.5 minutes.

Rupture test:
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/images/SLF_Project/line_graph.png"
       alt="line_graph"
       style="width: 100%; max-width: 600px; height: auto;">
</figure>
Our last test was to assess the effect of the brushes on low hanging grapes. We found that the larger the exposure of the grapes to the brushes, the more grapes were harmed. We completed this to test results on vines without vertical shoot positioning. We decided that this design would work better on vineyards that do use it, which is around 78% of New York vineyards. We also came to the conclusion that grapes lost due to rupture, is negligible compared to yield lost due to contamination.  

---

###### Prototype and Testing Details
The final prototype consists of two identical brush modules, each containing its own shaft, six replaceable nylon brushes, and a 12V motor, designed for smooth rotation and easy assembly.

<figure style="float: right; width: 300px; margin: 0 0 1em 1em;">
  <img src="{{ site.baseurl }}/assets/images/SLF_Project/Exploded.png"
       alt="Exploded"
       style="width: 100%; height: auto;">
</figure>

The system is assembled in a top-down sequence for easier installation. First, the motor is mounted to the top bracket and secured with nuts. The motor wiring is routed through the center of the top bracket and exits out the back for connection. For the second module, the wires are swapped so the motor spins in the opposite direction.

Next, the six nylon brushes are inserted into the slots of the central shaft. The bearing is press-fit into the bottom bracket to support rotation. The shaft is then inserted through the bearing and connected to the motor shaft above, allowing the system to rotate.

Finally, the top and bottom brackets are aligned, and the full assembly is secured to the backboard with screws. This process is repeated for the second module. This ensures proper alignment of the rotating components while allowing for easy brush replacement.

Functional testing: Initial brushes were too short and did not make consistent contact. Increasing the brush length (~3") improved performance.
Assembly testing: Brush insertion was difficult at first. Redesigning the shaft with larger slots made assembly faster and more reliable.
Torque testing: The initial motor was not strong enough due to friction. Loads were added to estimate required torque, which helped the selection of the 12V motor.

---

###### Bill of Materials
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/images/SLF_Project/bill.png"
       alt="bill"
       style="width: 100%; max-width: 600px; height: auto;">
</figure>
---

###### References 

- [PSU: Grapevines may only need help to survive heavy spotted lanternfly infestations](https://www.psu.edu/news/research/story/grapevines-may-only-need-help-survive-heavy-spotted-lanternfly-infestations)

- [SevenFifty Daily: The science behind vertical shoot positioning in vineyards (Wright, 2026)](https://daily.sevenfifty.com/the-science-behind-vertical-shoot-positioning-in-vineyards/)

---