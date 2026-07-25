---
layout: project
title: Parametric Bike Frame Design & Analysis
description: Using parametric CAD modeling and finite element analysis (FEA) project to design a bike frame from scratch
technologies: [Onshape, Parametric CAD, ANSYS, Finite Element Analysis, Structural Mechanics]
image: /assets/images/Frame_No_Weld.jpeg
---

I wanted to learn about FEA, more complex CAD design, and bikes, so I chose to iteratively design my own bike frame from scratch. I utilized YouTube for much of this project, and I will link videos I heavily relied on. Before beginning any tangible work on this project, I set baseline goals which are listed below.

##### Primary Project Goals
1. Develop proficiency in top-down parametric modeling with sketches, 3D part geometries, and assemblies.
2. Apply design for manufacturing (DFM) principles by accurately modeling tube shelling, joint mitering, and standard clearances required for welding and standard bicycle component assembly.
3. Learn and apply GD&T principles to create an engineering drawing of the frame and other assorted components.
4. Demystify the FEA "black box" by learning how CAD geometries are discretized into meshes and how the software mathematically solves for structural behavior.
5. Execute structural analysis using ANSYS by establishing realistic boundary conditions and applying real-world loading scenarios to analyze Von Mises stress, total deformation, and factors of safety, employing napkin sanity checks along the way.

<h3 style="text-align: center;">Master Geometry Sketches and Configuration Panel</h3>

Thanks to [Redburn Design's](https://www.youtube.com/@redburndesign) series on youtube: ["How to design a bike using Onshape CAD,"](https://www.youtube.com/playlist?list=PLAee2KkrOgzrAHBA8CoxkqoU4TDGOwVhZ) I was able to create the initial geometry sketches and extrudes. I made this bike configurable for different sizes, loosely following the [Cannondale Synapse 2](https://www.cannondale.com/en-us/bikes/road/endurance/synapse/synapse-2) design specs for sizing. I chose this bike to very loosely model the sizes after because it's a great entry level bike and doesn't have a geometry that's too aggressive.

You can see the config table and different size frame sketches below. I wanted to make this bike fully configurable, so I could learn to make sketches more robust and well-defined.

<div style="width: 100%; min-width: 300px; text-align: center;">
    <img src="{{ '/assets/images/Configuration_Panel.jpeg' | relative_url }}" alt="Full screen view of the basic frame geometry" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
    <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Partially shown config panel detailing the specs of different sizes.</em></p>
</div>

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0; align-items: center;">
    <div style="width: 32%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/Frame_Sketch_61.jpeg' | relative_url }}" alt="Master geometry sketch of the bike frame" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Size 61 Frame Sketch.</em></p>
    </div>
    <div style="width: 32%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/Frame_Sketch_54.jpeg' | relative_url }}" alt="Master geometry sketch of the bike frame" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Size 54 Frame Sketch.</em></p>
    </div>
    <div style="width: 32%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/Frame_Sketch_44.jpeg' | relative_url }}" alt="Master geometry sketch of the bike frame" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Size 44 Frame Sketch.</em></p>
    </div>
</div>

<h3 style="text-align: center;">3D Geometry</h3>

With the skeleton defined, I modeled the individual frame components. This required additional sketches for the rear triangle, tube shelling, mitering at the intersections, and creating planes + sketches for the lofts of the main triangle. The rear triangle is composed of the chainstays and seatstays, which I modeled to accommodate 700x32c tires and a 135mm rear axle width.

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 60%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/Full_Screen_OG_Frame.jpeg' | relative_url }}" alt="Full screen view of the basic frame geometry" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>The initial 3D geometry of the frame.</em></p>
    </div>
    <div style="width: 38%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/Frame_Exploded.jpeg' | relative_url }}" alt="Exploded view of the front triangle tubes" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Exploded view highlighting the individual tubes.</em></p>
    </div>
</div>

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/Chainstay_OG.jpeg' | relative_url }}" alt="Chainstay sub-assembly" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Chainstay geometry.</em></p>
    </div>
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/Seatstay_OG.jpeg' | relative_url }}" alt="Seatstay sub-assembly" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Seatstay geometry.</em></p>
    </div>
</div>

To model the welds and avoid huge stress concentrations in ANSYS at the tube connection points, I decided to model the frame as one part, with fillets. Below you can see the different frame geometry for different sizes.

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0; align-items: center;">
    <div style="width: 32%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/Frame_61.jpeg' | relative_url }}" alt="Master geometry sketch of the bike frame" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Size 61 Frame Geometry.</em></p>
    </div>
    <div style="width: 32%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/Frame_54.jpeg' | relative_url }}" alt="Master geometry sketch of the bike frame" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Size 54 Frame Geometry.</em></p>
    </div>
    <div style="width: 32%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/Frame_44.jpeg' | relative_url }}" alt="Master geometry sketch of the bike frame" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Size 44 Frame Geometry.</em></p>
    </div>
</div>

#### Derailleur Hanger, Bottom Bracket, and Head Tube
I did some research on standard components to make sure I got the bottom bracket threads and derailleur hanger threads to be realistic. I am still working on finalizing the derailleur hanger and its connection to the rear triangle.

<div style="display: flex; justify-content: center; gap: 15px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 30%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/Bottom_Bracket_Threads.jpeg' | relative_url }}" alt="Bottom bracket threading CAD view" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Modeled bottom bracket threading (1 3/8-24).</em></p>
    </div>
    <div style="width: 30%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/Derailleur_Sketch.jpeg' | relative_url }}" alt="Derailleur hanger layout sketch" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Derailleur hanger geometric sketch and constraints.</em></p>
    </div>
    <div style="width: 30%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/Derailleur_Hole.jpeg' | relative_url }}" alt="Derailleur hanger tapped hole feature" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Finalized derailleur hanger with tapped mounting hole.</em></p>
    </div>
</div>

<h3 style="text-align: center;">Finite Element Analysis Using ANSYS</h3>

Once the Onshape CAD model was finalized, I began learning how to perform FEA using ANSYS via the CornellX class ["A Hands-on Introduction to Engineering Simulations."](https://www.edx.org/learn/engineering/cornell-university-a-hands-on-introduction-to-engineering-simulations) This is what I'm currently working on for this project.

<div style="text-align: center; margin: 30px 0;">
    <img src="{{ '/assets/images/Frame_No_Weld.jpeg' | relative_url }}" alt="Final frame assembly prior to welding simulation" style="width: 80%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
    <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>The complete frame assembly, ready for simulation.</em></p>
</div>

<!--#### Mesh Generation & Boundary Conditions
In progress.

#### Results and Sanity Checks
In progress. -->

