---
layout: project
title: Heat Transfer & Thermal Analysis
description: Applying thermal resistance networks and lumped capacitance methods to evaluate heat sinks and transient systems.
technologies: [Fin Array Analysis, Thermal Resistance Networks, Lumped Capacitance Method]
image: /assets/images/HeatTransfer.jpg
---

From this assignment I learned about fin array analysis, resistance networks, as well as the lumped capacitance method for transient heat transfer. I have always wondered about why heat sinks are designed the way that they are, and this homework enabled me to see just how much of an impact they have on heat dissipation and management. Moreover, using the electrical analogy to accurately model heat transfer through and between different surfaces made a murky concept much easier to visualize and conceptualize.


<h3 style="margin-top: 30px;">Fin Array & Resistance Network Analysis</h3>
<p>The first part of the analysis focused on a cylindrical pin fin and a subsequent 5x5 fin array, calculating efficiency, thermal resistance, and overall heat dissipation. I then applied a thermal resistance network to model a heat sink mounted on a thin film heater to calculate the temperature reduction.</p>

<div style="background-color: #f9f9f9; padding: 20px; margin: 20px 0; border-radius: 8px;">
    <h4 style="margin-top: 0;">Problem 1: Fin Array and Heat Sink Optimization</h4>
    <p>This problem involved analyzing a cylindrical pin fin and a 5x5 fin array to determine temperature distribution, fin efficiency, and overall thermal resistance. The final part of the problem applied these concepts to evaluate how much a heat sink reduces the operating temperature of a thin film heater using a thermal resistance network.</p>
    
    <div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin-top: 20px;">
        <img src="/assets/images/p1p1.png" alt="Problem 1 Statement Parts A-E" style="width: 45%; border: 1px solid #ddd; box-shadow: 2px 2px 5px rgba(0,0,0,0.1);">
        <img src="/assets/images/p1p2.png" alt="Problem 1 Statement Part F" style="width: 45%; border: 1px solid #ddd; box-shadow: 2px 2px 5px rgba(0,0,0,0.1);">
    </div>
</div>

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 20px 0;">
    <img src="{{ '/assets/images/ht1.png' | relative_url }}" alt="Problem 1 knowns and schematic" style="width: 45%; margin-bottom: 20px;">
    <img src="{{ '/assets/images/ht2.png' | relative_url }}" alt="Temperature distribution calculations" style="width: 45%; margin-bottom: 20px;">
    <img src="{{ '/assets/images/ht3.png' | relative_url }}" alt="Fin efficiency and effectiveness" style="width: 45%; margin-bottom: 20px;">
    <img src="{{ '/assets/images/ht4.png' | relative_url }}" alt="Corrected length and overall array efficiency" style="width: 45%; margin-bottom: 20px;">
    <img src="{{ '/assets/images/ht5.png' | relative_url }}" alt="Heat dissipation calculations" style="width: 45%; margin-bottom: 20px;">
    <img src="{{ '/assets/images/ht6.png' | relative_url }}" alt="Thermal resistance network for heat sink" style="width: 45%; margin-bottom: 20px;">
</div>

<h3 style="margin-top: 30px;">Transient Heat Transfer</h3>
<p>The second part of the assignment evaluated a submerged wire experiencing Joule heating. Using the lumped capacitance method, I derived the temperature as a function of time to determine how quickly the system reached its steady-state temperature.</p>

<div style="background-color: #f9f9f9; padding: 20px; margin: 20px 0; border-radius: 8px;">
    <h4 style="margin-top: 0;">Problem 2: Transient Joule Heating</h4>
    <p>This problem focused on a transient heat transfer scenario where a submerged wire experienced sudden internal Joule heating. By applying the lumped capacitance method, I derived an expression for the wire's temperature over time to calculate exactly how long it would take to reach within 5°C of its steady-state temperature.</p>
    
    <div style="text-align: center; margin-top: 20px;">
        <img src="/assets/images/p2.png" alt="Problem 2 Statement" style="width: 90%; max-width: 800px; border: 1px solid #ddd; box-shadow: 2px 2px 5px rgba(0,0,0,0.1);">
    </div>
</div>

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 20px 0;">
    <img src="{{ '/assets/images/ht7.png' | relative_url }}" alt="Problem 2 schematic and assumptions" style="width: 45%; margin-bottom: 20px;">
    <img src="{{ '/assets/images/ht8.png' | relative_url }}" alt="Energy balance and steady state calculations" style="width: 45%; margin-bottom: 20px;">
    <img src="{{ '/assets/images/ht9.png' | relative_url }}" alt="Lumped capacitance time calculations" style="width: 45%; margin-bottom: 20px;">
</div>

