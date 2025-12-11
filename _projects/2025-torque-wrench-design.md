---
layout: project
title: Torque Wrench Design
description: Design of a torque wrench to meet certain safety requirements
technologies: [statics, materials science, ANSYS]
image: /assets/images/torque.jpg
---

<h3>Project Overview</h3>
<p>
  This project involved the design and finite element analysis (FEA) of a torque wrench to ensure it met strict safety factor requirements. Using ANSYS, I simulated various load conditions to identify stress concentrations and optimize the material selection.
</p>

<div class="project-gallery">

  <div class="gallery-item">
    <img src="/assets/images/CADMeasurements.png" alt="CAD drawing of torque wrench">
    <p class="caption">1. Initial CAD Drafting & Dimensions</p>
  </div>

  <div class="gallery-item">
    <img src="/assets/images/3a.png" alt="ANSYS Displacement Setup">
    <p class="caption">2. Boundary Conditions & Displacement Setup</p>
  </div>

  <div class="gallery-item">
    <img src="/assets/images/3b.png" alt="ANSYS Force Application">
    <p class="caption">3. Force Application (50 lbf Load)</p>
  </div>

  <div class="gallery-item">
    <img src="/assets/images/4a.png" alt="Preliminary Stress Mesh">
    <p class="caption">4. Preliminary Stress Analysis (Mesh View)</p>
  </div>

  <div class="gallery-item">
    <img src="/assets/images/4b.png" alt="Stress Concentration Zoom">
    <p class="caption">5. Stress Concentration at Fillet (Zoom)</p>
  </div>

  <div class="gallery-item">
    <img src="/assets/images/5a.png" alt="Refined Stress Analysis Head">
    <p class="caption">6. Refined Stress Analysis (Head Detail)</p>
  </div>

  <div class="gallery-item">
    <img src="/assets/images/5b.png" alt="Full Bar Stress Distribution">
    <p class="caption">7. Full Bar Stress Distribution</p>
  </div>

  <div class="gallery-item">
    <img src="/assets/images/5c.png" alt="Max Stress Location">
    <p class="caption">8. Maximum Stress Location Analysis</p>
  </div>

  <div class="gallery-item">
    <img src="/assets/images/6Materials.png" alt="Material Optimization Gradient">
    <p class="caption">9. Material Optimization & Safety Factors</p>
  </div>

  <div class="gallery-item">
    <img src="/assets/images/8Materials.png" alt="Strain Gauge Diagram">
    <p class="caption">10. Strain Gauge Selection & Placement</p>
  </div>

</div>

<style>
  .project-gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 25px;
    margin-top: 30px;
    margin-bottom: 40px;
  }
  
  .gallery-item {
    background: #f9f9f9;
    padding: 10px;
    border-radius: 6px;
    border: 1px solid #eaeaea;
    transition: transform 0.2s;
  }

  .gallery-item:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 8px rgba(0,0,0,0.05);
  }

  .gallery-item img {
    width: 100%;
    height: auto;
    border-radius: 4px;
    display: block;
  }

  .caption {
    font-size: 0.85em;
    color: #666;
    text-align: center;
    margin-top: 10px;
    margin-bottom: 0;
    font-family: sans-serif;
  }
</style>
