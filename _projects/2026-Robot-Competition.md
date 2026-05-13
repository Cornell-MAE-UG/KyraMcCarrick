---
layout: project
title: Expanding Cube-Collection Robot
description: An autonomous robot featuring a passive mechanical expansion system and sensor-based navigation to efficiently collect cubes within competition constraints.
technologies: [Arduino, Sensor Integration, Mechanism Design, Rapid Prototyping, Autonomous Navigation]
image: /assets/images/robot_final.jpg
---

As part of the MAE 3780 course, our team (Group 59: Sabrina Wang, Maggie Huggins, and Kyra McCarrick) was tasked with designing and building an autonomous robot to collect cubes[cite: 1, 2, 3]. The primary engineering challenge was strict size constraints: the robot had to fit within an 8 in x 8 in starting area but needed to maximize its collection footprint[cite: 4]. To solve this, we designed a system that could expand to a maximum width of 12 inches during operation[cite: 4].

### Brainstorming & Iteration
Our mechanical design evolved significantly throughout the project[cite: 30]. We initially prototyped an expanding arm mechanism to collect blocks in front of the robot, but it failed to fit within the 12-inch diameter limit[cite: 30]. We then pivoted to an expanding flap design[cite: 31]. 

Our first iteration of the flaps utilized polypropylene sheets[cite: 31]. However, these proved to be too heavy, increased the risk of the robot tipping, and did not spring back open as effectively as we needed[cite: 31]. They were also difficult to modify[cite: 32]. We ultimately switched to cardboard, which was lightweight, durable enough for the competition, and much easier to quickly prototype and iterate upon[cite: 8, 33]. 

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0; align-items: center;">
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/sketches_dimensions.jpg' | relative_url }}" alt="Robot dimensional sketches" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Front and top-down mechanical sketches mapping out the 8-inch starting constraint and 12-inch expansion[cite: 108, 110, 117, 121, 128].</em></p>
    </div>
</div>

### Mechanical Design & Passive Expansion
The final robot combined a passive mechanical expansion system with sensor-based navigation[cite: 5]. The chassis consisted of a cardboard outer shell mounted onto a two-wheel DC motor base[cite: 6]. The shell featured a back wall and two side flaps that acted as a funnel[cite: 7].

At the start of a match, the side flaps were folded inward at 90° angles to comply with the 8x8 inch starting size[cite: 9]. We used removable standoffs placed between the 130° limit brackets and the back wall to hold the flaps closed[cite: 11]. These standoffs were connected to the robot's wheels via string[cite: 12]. As soon as the robot began driving forward, the wheels pulled the strings, yanking out the standoffs and allowing the folded cardboard shell to naturally spring outward into a 12-inch wide V-shape[cite: 12]. Because the robot was programmed to never drive backwards, the collected cubes remained securely funneled within these side walls[cite: 13, 14].

During testing, we discovered that collected cubes were jamming between the wheels and the inner walls, stalling the robot[cite: 34]. To resolve this, we fabricated and installed a wheel cage to protect the drivetrain from collisions[cite: 35].

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/robot_starting.jpg' | relative_url }}" alt="Robot in starting configuration" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>The robot in its 8x8 starting position with standoffs locked[cite: 25].</em></p>
    </div>
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/robot_expanded.jpg' | relative_url }}" alt="Robot in expanded configuration" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>The expanded V-shaped configuration post-deployment[cite: 25].</em></p>
    </div>
</div>

### Electrical Systems & Strategy
Electrically, the robot was powered by an Arduino UNO[cite: 15, 58]. Initially, we attempted to navigate without QTI (line-following) sensors, but the robot struggled to detect borders and frequently drifted off the playing board[cite: 28]. To fix this, we integrated two front-mounted QTI sensors to detect the black field borders and prevent falls[cite: 17, 29]. We also mounted a color sensor centrally beneath the chassis to detect the transition between the blue and yellow sections of the competition field[cite: 16]. 

Our competition strategy was coded to follow a specific flowchart:
1. **Trigger:** Drive forward to passively deploy the expansion mechanism[cite: 19].
2. **Center Alignment:** Continue straight until the color sensor detects a blue/yellow transition (indicating the center of the board)[cite: 20].
3. **Sweep:** Turn 90° to the right and drive forward to collect cubes[cite: 21].
4. **Border Reversal:** When the QTI sensors detect the black edge border, execute a 180° turn and drive to the opposite side[cite: 21, 22].
5. **Loop:** Repeat this back-and-forth sweeping motion across the center region to maximize cube collection[cite: 22, 23].

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin: 30px 0;">
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/circuit_diagram.jpg' | relative_url }}" alt="Circuit Diagram" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>Our custom circuit diagram mapping the Arduino to the QTI and Color sensors[cite: 56, 107].</em></p>
    </div>
    <div style="width: 45%; min-width: 300px; text-align: center;">
        <img src="{{ '/assets/images/flowchart.jpg' | relative_url }}" alt="Logic Flowchart" style="width: 100%; border-radius: 6px; border: 1px solid #eee; box-shadow: 2px 2px 6px rgba(0,0,0,0.05);">
        <p style="font-size: 0.9em; color: #666; margin-top: 10px;"><em>The autonomous logic loop governing the robot's sweeping strategy[cite: 150, 162].</em></p>
    </div>
</div>

### Total Bill of Materials
By utilizing cardboard and basic hardware, we kept our mechanical prototyping costs extremely low. Below is the final Bill of Materials for the structural components[cite: 54, 55].

<div style="overflow-x: auto; margin: 30px 0; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.05);">
    <table style="width: 100%; border-collapse: collapse; text-align: left; font-size: 0.95em; background-color: #fff;">
        <thead>
            <tr style="background-color: #f4f4f4; border-bottom: 2px solid #ddd;">
                <th style="padding: 12px 15px; border: 1px solid #eee;">Item</th>
                <th style="padding: 12px 15px; border: 1px solid #eee;">Quantity</th>
                <th style="padding: 12px 15px; border: 1px solid #eee;">Unit Price</th>
                <th style="padding: 12px 15px; border: 1px solid #eee;">Total Price</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td style="padding: 12px 15px; border: 1px solid #eee;">Zinc Plated Steel Surface Mount Hinges with Holes</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">2</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">$10.75/pair</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">$10.75</td>
            </tr>
            <tr style="background-color: #fcfcfc;">
                <td style="padding: 12px 15px; border: 1px solid #eee;">Polypropylene Sheets</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">(1) 12" x 24" sheet</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">$6.98/sheet</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">$6.98</td>
            </tr>
            <tr>
                <td style="padding: 12px 15px; border: 1px solid #eee;">Corner Bracket</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">2</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">$1.06</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">$2.12</td>
            </tr>
            <tr style="background-color: #fcfcfc;">
                <td style="padding: 12px 15px; border: 1px solid #eee;">Cardboard</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">(5) 36" x 36" sheet</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">$n/a</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">$n/a</td>
            </tr>
            <tr>
                <td style="padding: 12px 15px; border: 1px solid #eee;">String</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">12"</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">$n/a</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">$n/a</td>
            </tr>
            <tr style="font-weight: bold; background-color: #eaeaea;">
                <td colspan="3" style="padding: 12px 15px; border: 1px solid #eee; text-align: right;">TOTAL:</td>
                <td style="padding: 12px 15px; border: 1px solid #eee;">$19.85</td>
            </tr>
        </tbody>
    </table>
</div>

### Performance & Takeaways
During the competition, our robot performed incredibly well, consistently collecting between 8 and 13 cubes per round[cite: 37]. The navigation sensors proved highly reliable, successfully keeping the robot from falling off the board throughout the event[cite: 38, 45]. The expanding flaps successfully maintained a wide, efficient collection area[cite: 46]. 

We did face a few unexpected challenges. A late calibration adjustment caused the robot to over-turn past 90 degrees during competition day[cite: 39, 40, 41]. We also noticed that when opponent robots collided with our side flaps, cubes could spill out[cite: 42]. If we were to redesign the robot, we would utilize the remaining allowable starting length to add front standoffs to better protect the flaps from other robots, and we would source larger wheels to increase our travel speed[cite: 43, 50].