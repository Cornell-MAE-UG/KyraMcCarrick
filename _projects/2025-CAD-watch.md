---
layout: project
title: Garmin Watch CAD Model
description: CAD Model of a Garmin 265 Forerunner Watch
technologies: [Fusion360, Reverse Engineering, Drafting]
image: /assets/images/garmin.jpg
---

As a part of my Intro to Mechanical Design course, I reverse-engineered and created a fully parametric CAD model of my Garmin Forerunner 265 watch. [Insert a few more sentences here detailing your process, the biggest challenges you faced while modeling it, or specific Fusion360 tools you utilized to achieve the complex curves of the watch body.]

<div style="clear: both; padding-top: 20px;"></div>

### Software & Skills Applied
<p style="margin: 20px 0 40px 0; font-size: 1.1em; line-height: 1.8;">
    <strong>Autodesk Fusion360</strong> &nbsp;|&nbsp; <strong>Reverse Engineering</strong> &nbsp;|&nbsp; <strong>Calipers & Dimensioning</strong> &nbsp;|&nbsp; <strong>Parametric Modeling</strong> &nbsp;|&nbsp; <strong>Digital Rendering</strong>
</p>

### Phase 1: Reference & Dimensioning
The first step was to carefully analyze the physical watch. Using digital calipers, I took precise measurements of the watch face, strap, latch, and retaining clips. I translated these measurements into hand-drawn technical sketches to serve as a blueprint before opening any software.

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 30%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/GarminBefore.jpg' | relative_url }}" alt="Real Garmin Watch Top View" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>The physical watch.</em></p>
    </div>
    <div style="width: 30%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/Watch.jpg' | relative_url }}" alt="Real Garmin Watch Angled View" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Side profile reference.</em></p>
    </div>
    <div style="width: 30%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/GarminCADSketches.jpg' | relative_url }}" alt="Hand drawn dimension sketches" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Initial hand-drawn dimensioning.</em></p>
    </div>
</div>

### Phase 2: Modeling & Assembly in Fusion360
Using the sketches as a guide, I built the individual components in Fusion360. This required creating multiple independent bodies—including the long strap, short strap, main watch face, latch, and strap holder—and carefully assigning joints and mates to assemble them into a cohesive final product.

<div style="text-align: center; margin: 30px 0;">
    <img src="{{ '/assets/images/GarminWorkspace.jpg' | relative_url }}" alt="Fusion360 Workspace and Assembly Tree" style="width: 90%; max-width: 800px; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
    <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>The Fusion360 workspace showing the component tree and fully mated assembly.</em></p>
</div>

### Phase 3: Final Digital Renders
Once the geometry was fully defined, I applied appropriate materials and appearances to the model to mimic the matte silicone strap and glass face of the real device, producing the final digital renders.

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/GarminRender.jpg' | relative_url }}" alt="Front angled render of CAD model" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Front view final render.</em></p>
    </div>
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/GarminRender2.jpg' | relative_url }}" alt="Back angled render of CAD model" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Back view detailing the sensor housing.</em></p>
    </div>
</div>