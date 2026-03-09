---
layout: project
title: Torque Wrench Design
description: FEA Analysis of a titanium torque wrench using ANSYS.
image: assets/images/3b.png
---

**MAE 3270**
**Final Homework Analysis**
**Maggie Huggins and Kyra McCarrick**
**12/10/2025**

## 1. Model & Material Properties

Image of CAD model:
<div style="text-align: center; margin-top: 20px; margin-bottom: 20px;">
  <img src="{{ site.baseurl }}/assets/images/CADMeasurements.png" alt="CAD Drawing" style="width: 90%; border: 1px solid #ccc;">
</div>

We used Titanium Alloy, Ti-6Al-4V, annealed which has the following material properties:

| Property | Value |
| :--- | :--- |
| **Young’s Modulus** | 16x10⁶ psi |
| **Poisson’s Ratio** | 0.31 |
| **Tensile Strength** | 125x10³ psi |
| **Fracture Toughness** | 76.4x10³ psi*in¹/² |
| **Fatigue Strength** | 52x10³ (for 10⁶ cycles) |

---

## 2. Loads & Boundary Conditions

Diagram communicating how loads and boundary conditions were applied to the FEM model.
We clamped the model on all sides at the top of the bit portion (as highlighted in yellow) and applied a load of 50 lbf to the yz face of the wrench handle.

<div style="display: flex; justify-content: space-around; margin-top: 20px;">
  <div style="width: 48%;">
    <img src="{{ site.baseurl }}/assets/images/3a.png" alt="Displacement Constraint" style="width: 100%; border: 1px solid #eee;">
  </div>
  <div style="width: 48%;">
    <img src="{{ site.baseurl }}/assets/images/3b.png" alt="Force Application" style="width: 100%; border: 1px solid #eee;">
  </div>
</div>

---

## 3. FEM Stress & Strain Results

Normal strain contours (in the strain gauge direction) from FEM.
The strain is roughly constant throughout the entire model except for around the connection between the clamped and unclamped portion of the bit.

<div style="display: flex; justify-content: space-around; margin-bottom: 20px;">
  <div style="width: 48%;">
    <img src="{{ site.baseurl }}/assets/images/4a.png" alt="Preliminary Mesh" style="width: 100%;">
  </div>
  <div style="width: 48%;">
    <img src="{{ site.baseurl }}/assets/images/4b.png" alt="Mesh Zoom" style="width: 100%;">
  </div>
</div>

Contour plot of maximum principal stress from FEM.
The wrench handle is half in tension and half in compression, this aligns with what we know about applying force to fixed beams. Furthermore, the maximum stress appears in the body that serves as the connection.

<div style="display: flex; flex-wrap: wrap; justify-content: space-around;">
  <div style="width: 48%; margin-bottom: 15px;">
    <img src="{{ site.baseurl }}/assets/images/5b.png" alt="Global Stress" style="width: 100%;">
  </div>
  <div style="width: 48%; margin-bottom: 15px;">
    <img src="{{ site.baseurl }}/assets/images/5c.png" alt="Max Stress Side View" style="width: 100%;">
  </div>
  <div style="width: 48%;">
    <img src="{{ site.baseurl }}/assets/images/5a.png" alt="Head Stress Zoom" style="width: 100%;">
  </div>
  <div style="width: 48%;">
    <img src="{{ site.baseurl }}/assets/images/6Materials.png" alt="Deflection Analysis" style="width: 100%;">
  </div>
</div>

---

## 4. Summary & Sensor Selection

Summary of the results from FEM calculation showing maximum normal stress (anywhere), load point deflection, strains at the strain gauge locations:

| Metric | Result |
| :--- | :--- |
| **Maximum Normal Stress** | 14213 psi |
| **Strain at Strain Gauge location** | 9.8497x10⁻⁴ in/in (985 microstrain) |
| **Deflection of load point** | 0.21262 in |

The Torque wrench sensitivity in mV/V using strains from the FEM analysis is **0.985 mV/V**
The hand calculations lead to a torque wrench sensitivity of greater than 1, which satisfies the problem prompt.

**Strain gauge selection:**
We selected the SGD-5/350-LY43 Linear strain gauge. This gauge has a carrier area of 9.8 x 5.2 mm² or 0.386 x 0.205in², meaning it will fit comfortably within the wrench handle. This is a linear pattern strain gauge.

<div style="text-align: center; margin-top: 20px;">
  <img src="{{ site.baseurl }}/assets/images/8Materials.png" alt="Strain Gauge" style="width: 30%; min-width: 150px;">
</div>