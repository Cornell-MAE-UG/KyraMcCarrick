---
layout: project
title: Drop-Down Closet Shelf
description: An extendable, drop-down storage solution designed to maximize vertical closet space in small apartments.
technologies: [Laser Cutting, 3D Printing, Acrylic Fabrication, Mechanism Design, Structural Testing]
image: /assets/images/finaldownside.jpg
---

As part of my MAE 2250 (Intro to Mechanical Design) course, my team ("4Store") was tasked with addressing a problem and then designing and creating a solution. We interviewed many college students, and found that a common issue was a lack of storage space. We focused on unusable vertical space, specifically in closets, where the back and top areas are often completely inaccessible.

### Brainstorming & Ideation
We initially brainstormed 15 different concepts. After evaluating them based on feasibility and impact, we pursued a drop-down shelf. The core concept was a shelf plate that could slide forward on rails and drop down 90 degrees, allowing easy access to items stored in the back of the closet.

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0; align-items: center;">
    <div style="width: 25%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/early.png' | relative_url }}" alt="Early sketch idea 1" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Lecture desk extender.</em></p>
    </div>
    <div style="width: 40%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/ideas.jpg' | relative_url }}" alt="Brainstorming List and Feasibility Chart" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Our initial brainstorming list and feasibility rankings.</em></p>
    </div>
    <div style="width: 25%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/early2.png' | relative_url }}" alt="Early sketch idea 2" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Alternative dropdown approach.</em></p>
    </div>
</div>

Once the concept was selected, we drafted detailed mechanical sketches to map out the sliding rails, baseplate, and the specific geometries needed for the drop.

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/finaldesignsketch.jpg' | relative_url }}" alt="Detailed Drop Down Shelf Sketch 1" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Mechanism detailing and dimensioning.</em></p>
    </div>
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/finalsketch2.jpg' | relative_url }}" alt="Detailed Drop Down Shelf Sketch 2" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Visualizing the drop-down motion and joints.</em></p>
    </div>
</div>

### Scrappy Prototyping
Before cutting any final materials or designing complex CAD assemblies, we built "scrappy" prototypes using cardboard, wood, and basic hardware. This allowed us to physically test the sliding mechanics and visualize how the different parts worked together.

<div style="display: flex; justify-content: center; gap: 15px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 30%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/proto1.jpg' | relative_url }}" alt="Early cardboard prototype base" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
    </div>
    <div style="width: 30%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/proto2.jpg' | relative_url }}" alt="Early cardboard prototype sliding mechanism" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
    </div>
    <div style="width: 30%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/proto3.jpg' | relative_url }}" alt="Early cardboard prototype extended" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
    </div>
    <p style="font-size: 0.9em; color: #666; width: 100%; text-align: center; margin-top: 10px;"><em>Initial prototypes testing the sliding and dropping mechanism.</em></p>
</div>

### Testing & Refinement
To ensure our design was structurally viable, we established core metrics: the entire assembly needed to support 10-15 lbs, with the dropdown shelf safely supporting a minimum of 5 lbs on its own. 

We conducted rigorous reliability testing by placing a 5-pound weight on the deployed shelf and dropping the mechanism 10 consecutive times to observe where the force transferred. This testing revealed that our initial hot-glue joints and string-based sliding mechanisms were our limiting factors, and often broke apart. Based on this data, we revised our design, abandoning hot glue and strings in favor of screws, wood supports beneath the acrylic, and rigid hinges to better facilitate the sliding movement.

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/weight_test.png' | relative_url }}" alt="Shelf undergoing 5lb weight test" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Testing the drop-down shelf.</em></p>
    </div>
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/broken_joint.png' | relative_url }}" alt="Failed hot glue joint" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>The platform began to bow with too much weight.</em></p>
    </div>
</div>

### Manufacturing Challenges & Iteration
Our first full-sized prototype was intended to be laser-cut from marine-grade plywood. However, we discovered at the Rapid Prototyping Lab (RPL) that this specific wood was too dense for the laser cutters. We had to cut the pieces using a bandsaw, which cost us significant time and precision. 

<div style="display: flex; justify-content: center; gap: 15px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 30%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/mid.png' | relative_url }}" alt="Intermediate wood prototype" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
    </div>
    <div style="width: 30%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/mid2.png' | relative_url }}" alt="Intermediate mechanism test" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
    </div>
    <div style="width: 30%; min-width: 200px; text-align: center;">
        <img src="{{ '/assets/images/mid3.png' | relative_url }}" alt="Intermediate prototype extended" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
    </div>
    <p style="font-size: 0.9em; color: #666; width: 100%; text-align: center; margin-top: 10px;"><em>First full-scale prototype.</em></p>
</div>

For our next iteration, we switched to 1/8" and 1/4" black acrylic to ensure smooth, precise laser cutting. To further improve the mechanism beyond standard hinges, we utilized T-shaped alignment pins slotted into custom 3D-printed fasteners. This allowed the plates to stack smoothly and securely without taking up vertical space.

### Bill of Materials
Below is the comprehensive Bill of Materials detailing the sourced hardware and raw materials required across all prototypes.

<div style="overflow-x: auto; margin: 30px 0; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.05);">
    <table style="width: 100%; border-collapse: collapse; text-align: left; font-size: 0.95em; background-color: #fff;">
        <thead>
            <tr style="background-color: #f4f4f4; border-bottom: 2px solid #ddd;">
                <th style="padding: 12px 15px; border: 1px solid #eee;">Part Description</th>
                <th style="padding: 12px 15px; border: 1px solid #eee;">Prototype</th>
                <th style="padding: 12px 15px; border: 1px solid #eee;">McMaster Code</th>
                <th style="padding: 12px 15px; border: 1px solid #eee;">Qty</th>
                <th style="padding: 12px 15px; border: 1px solid #eee;">Unit Cost ($)</th>
                <th style="padding: 12px 15px; border: 1px solid #eee;">Total ($)</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td style="padding: 12px 15px; border: 1px solid #eee;">24" by 24" marine grade plywood sheet 1/4" thick</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 3</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">1125T413</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">2</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">33.60</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">67.20</td>
            </tr>
            <tr style="background-color: #fcfcfc;">
                <td style="padding: 12px 15px; border: 1px solid #eee;">1/8" thick black acrylic 24" by 24" sheet</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 3</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">8505K744</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">1</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">37.07</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">37.07</td>
            </tr>
            <tr>
                <td style="padding: 12px 15px; border: 1px solid #eee;">1/8” thick black acrylic sheet 12” by 12” sheet</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 3</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">From Upson 242</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">2</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">0.00</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">0.00</td>
            </tr>
            <tr style="background-color: #fcfcfc;">
                <td style="padding: 12px 15px; border: 1px solid #eee;">Adjustable-Friction Hinge, Black Acetal Plastic, 1-11/16” x 23/32” Door Leaf</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 3 & 5</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">1791A44</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">6</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">8.28</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">49.68</td>
            </tr>
            <tr>
                <td style="padding: 12px 15px; border: 1px solid #eee;">3/16" birch rods, 25 per package, 36" long</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 3 & 5</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">9683K12</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">1</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">9.58</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">9.58</td>
            </tr>
            <tr style="background-color: #fcfcfc;">
                <td style="padding: 12px 15px; border: 1px solid #eee;">Conformable Magnet for Irregular Surfaces, 1/32” thick, .5” wide, 24” long</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 3 & 5</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">3651K855</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">4</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">18.12</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">72.48</td>
            </tr>
            <tr>
                <td style="padding: 12px 15px; border: 1px solid #eee;">12" by 24" black acrylic sheet 1/8" thick</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 5</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">8505K742</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">1</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">19.25</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">19.25</td>
            </tr>
            <tr style="background-color: #fcfcfc;">
                <td style="padding: 12px 15px; border: 1px solid #eee;">12" by 24" black acrylic sheet 1/4" thick</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 5</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">8505K755</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">1</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">26.41</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">26.41</td>
            </tr>
            <tr>
                <td style="padding: 12px 15px; border: 1px solid #eee;">24" by 24" black acrylic sheet 1/4" thick</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 5</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">8505K757</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">1</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">52.81</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">52.81</td>
            </tr>
            <tr style="background-color: #fcfcfc;">
                <td style="padding: 12px 15px; border: 1px solid #eee;">8-32 1/4" length fully threaded undercut screws, black oxide 18-8 stainless steel</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 5</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">96640A274</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">1</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">13.31</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">13.31</td>
            </tr>
            <tr>
                <td style="padding: 12px 15px; border: 1px solid #eee;">Precision Alignment Pin, T-Style, 1/8” 2-1/2” long</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 5</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">98021A412</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">4</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">5.50</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">22.00</td>
            </tr>
            <tr style="background-color: #fcfcfc;">
                <td style="padding: 12px 15px; border: 1px solid #eee;">3D-Printed pin holder</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 5</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">N/A</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">4</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">2.40</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">9.60</td>
            </tr>
            <tr>
                <td style="padding: 12px 15px; border: 1px solid #eee;">3D-Printed spacers</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">ODP 5</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">N/A</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">4</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">0.47</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">1.88</td>
            </tr>
            <tr style="font-weight: bold; background-color: #eaeaea;">
                <td colspan="5" style="padding: 12px 15px; border: 1px solid #eee; text-align: right;">TOTAL:</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">$381.27</td>
            </tr>
        </tbody>
    </table>
</div>

### Final Product Design
The final product successfully stores up to 5 pounds on the collapsible shelf and 10-15 pounds on the base plate. Using friction hinges and a magnetic locking backplate, it can be smoothly slid out and deployed in under 10 seconds. 

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/finalup.jpg' | relative_url }}" alt="Shelf in collapsed, stowed position" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>The shelf in its fully collapsed, stowed position.</em></p>
    </div>
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/finaldownside.jpg' | relative_url }}" alt="Shelf in extended, drop-down position" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>The mechanism deployed.</em></p>
    </div>
</div>

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/finalback.jpg' | relative_url }}" alt="Back view of mechanism" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Rear view detailing the magnetic locking plate and rails.</em></p>
    </div>
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/finaldown.jpg' | relative_url }}" alt="Top down view of extended shelf" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Top-down view of the deployed shelf surface.</em></p>
    </div>
</div>

### Demonstration
Check out the video below to see a demonstration of how the sliding and drop-down mechanisms work:

<div style="text-align: center; margin: 30px 0;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/d_e4e76CVhU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"></iframe>
</div>