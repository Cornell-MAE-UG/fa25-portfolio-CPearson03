---
layout: project
title: Active Suspension Project
description: Modeling and designing an active suspension system
technologies: [MATLAB]
image: /assets/images/Active_Suspension/Suspension System.png
---
<style>
  .img-row {
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
    justify-content: center;
  }
  .img-row img {
    max-height: 180px;
    width: auto;
  }
  figure {
    text-align: center;
    margin: 25px 0;
  }
  figcaption {
    font-size: 0.9rem;
    color: #555;
    margin-top: 5px;
  }
</style>

### Introduction
This project focuses on the analysis and design of an active suspension system. We take a state space approach to modeling the system and then use active control to optimize its performance. 

---

### Assumptions and Design Requirements
The following assumptions were made to simplify the analysis:
  <ul>
    <li>Quarter-car model represents one wheel and associated mass; only vertical motion considered.</li>
    <li>Yaw, pitch, roll, and aerodynamic effects are neglected.</li>
    <li>Masses are rigid; suspension components are linear and frictionless.</li>
    <li>Road input and actuator are ideal (perfect force application, no delays).</li>
    <li>Performance targets: driver acceleration &lt;1.5 m/s², body displacement &lt;1 cm, shock travel &lt;10 cm.</li>
  </ul>


### Model of the System
The governing equations of the system are:
<figure>
  <img src="/fa25-portfolio-CPearson03/assets/images/Active_Suspension/ODEs.png"
       alt="ODEs"
       style="width: 80%;">
</figure>


<p style="text-align: left;">We defined the state vector as:</p>
<figure style="text-align: center;">
  <img src="/fa25-portfolio-CPearson03/assets/images/Active_Suspension/X_vector.png"
       alt="X_vector"
       style="width: 20%;">
</figure>

<p style="text-align: left;">The output vector as:</p>
<figure style="text-align: center;">
  <img src="/fa25-portfolio-CPearson03/assets/images/Active_Suspension/Y_vector.png"
       alt="Y_vector"
       style="width: 20%;">
</figure>

<p style="text-align: left;">And the input vector as:</p>
<figure style="text-align: center;">
  <img src="/fa25-portfolio-CPearson03/assets/images/Active_Suspension/U_vector.png"
       alt="U_vector"
       style="width: 20%;">
</figure>


<p style="text-align: left;">This gave us the following state space representation:</p>
<figure style="text-align: center;">
  <img src="/fa25-portfolio-CPearson03/assets/images/Active_Suspension/state_space1.png"
       alt="state_space1"
       style="width: 80%;">
  <br>
  <img src="/fa25-portfolio-CPearson03/assets/images/Active_Suspension/state_space2.png"
       alt="state_space2"
       style="width: 80%;">
</figure>


<p style="text-align: left;">Following anaysis gave the closed form representation of the transfer function of the sytem
</p>
<figure style="text-align: center;">
  <img src="/fa25-portfolio-CPearson03/assets/images/Active_Suspension/Transfer function.png"
       alt="Transfer function"
       style="width: 40%;">
</figure>

<p style="text-align: left;">and its poles
</p>
<figure style="text-align: center;">
  <img src="/fa25-portfolio-CPearson03/assets/images/Active_Suspension/Poles.png"
       alt="Poles"
       style="width: 20%;">
</figure>

## Closed Loop Analysis
We analysed the closed loop dynamics using the block diagram of the system
<figure>
  <img src="/fa25-portfolio-CPearson03/assets/images/Active_Suspension/Block diagram.png"
       alt="Block diagram"
       style="width: 100%;">
</figure>

The control changed the state space system to the following 
<figure>
  <img src="/fa25-portfolio-CPearson03/assets/images/Active_Suspension/X_closedloop.png"
       alt="X_closedloop"
       style="width: 60%;">
</figure>


<h3>Parameters</h3>
In our model we used these parameters
<ul>
  <li>Acceleration (a(t)) &lt; 5 m/s² — Sprung Mass: 300 kg</li>
  <li>Displacement y(t) &lt; 1.5 cm — Unsprung Mass: 60 kg</li>
  <li>Shock Travel &lt; 10 cm — Tire Stiffness: 190,000 N/m</li>
  <li>Road Height: 0.05 m</li>
  <li>Suspension Stiffness: 17,000 N/m</li>
  <li>Suspension Damping: 2,500 N·s/m</li>
</ul>

## Results
We initially modeled the suspension system in its closed loop form, without any control. We then compared this to the system active control and yielded the following results

