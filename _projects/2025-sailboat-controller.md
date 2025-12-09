---
layout: project
title: 2D Sailboat Control System
description: LQR control system for a sailboat
technologies: [MATLAB, System Dynamics, LQR]
image: /assets/images/sailboattrajectory.jpg
---


As part of a class project for MAE 3260, System Dynamics, my group and I worked on both 1D and 2D simplified models of a sailboat. We implemented an LQR control system to respond to wind disturbance as an impulse as well as a step input.

I was interested in the fluid dynamics of the system. I used Professor Brian Kirby’s textbook, How Fluid Machines Work, 2025 edition, to try to make a more accurate model of the drag and lift force acting on the 1D model of the sailboat (assuming the sail acts as a bluff body and not an airfoil). I found drag coefficients for a 60 degree cone (the hull in water), and used the drag coefficients for a cup anemometer in its 180 degree and 0 degree orientations to model the lift force and the drag force on the sail. Our control inputs here are the angle of the sail, the wind force, and our output is the boat position x. I then realized that the drag and lift terms are dependent on the relative wind speed, which is U-xdot, not just U, so I added that in.

Here is some of my work creating the model: 
<div style="text-align: center;">
    <img src="/assets/images/Sailboatwork.png" alt="Calculations" width="600">
</div>

Using the State Space model my group mate, created I used AI and to make a MATLAB Livescript that helped us tune our controller and visualize the corresponding response of the system.

Here are some screenshots of the model:
<div style="text-align: center;">
    <img src="/assets/images/ControllerUI.png" alt="UI" width="600">
</div>
<div style="text-align: center;">
    <img src="/assets/images/sailboattrajectory.jpg" alt="" width="600">
</div>
<div style="text-align: center;">
    <img src="/assets/images/sailboaterror.jpg" alt="" width="600">
</div>

