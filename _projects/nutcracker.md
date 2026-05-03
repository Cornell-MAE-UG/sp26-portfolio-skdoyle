---
layout: project
title: Nutcracker Project
technologies: N/A
image: <img width="443" height="284" alt="Screenshot 2026-03-07 at 11 54 26 AM" src="https://github.com/user-attachments/assets/12cb675c-33e6-4b1d-8b13-bc67ff39bcb7" />
---
 
# Nutcracker Lever Design Project

## Overview
This project designs a simple hand-operated lever nutcracker capable of cracking a macadamia nut using average human grip strength. The design uses statics and mechanical advantage to determine the required handle length and the distance between the hinge and the nut.


## 1. Problem Statement and Objective ("Find")

design a lever-based nutcracker that allows a person to crack a macadamia nut by hand.

The goal is to determine:

• the distance from the hinge to the nut  
• the required handle length  
• whether average human grip strength is sufficient to crack the nut  


## 2. Constraints and Input Parameters ("Given")

### Macadamia Nut Force
Average load required to crack a macadamia nut:

222.18 kg

Convert to force:

F = mg  
F = 222.18 × 9.81  
F = 2179.59 N

Rounded design value:

FN ≈ 2300 N


### Nut Geometry

Macadamia nut diameter:

28 mm

Radius:

14 mm

The nut is assumed to sit symmetrically between the two jaws of the nutcracker.


### Human Grip Strength

Average human grip strength:

36 kg

Converted to force:

FG = 36 × 9.81  
FG = 353.16 N

Rounded value used for design:

FG ≈ 350 N

Because the nutcracker is symmetric:

FGU = FGL = 175 N

The cracking force is also split between the jaws:

FNU = FNL = 1150 N


## 3. Approach to the Problem

The nutcracker is modeled as a simple lever rotating about the hinge.


### Moment Balance

Taking moments about hinge point A:

ΣMA = 0

The moment produced by the user force must equal the moment required to crack the nut.

|AG| FG = |AN| FN

Rearranging:

FN / FG = |AG| / |AN|


### Mechanical Advantage

Substitute the design forces:

FN = 2300 N  
FG = 350 N

2300 / 350 = 6.571

Therefore the nutcracker must provide a mechanical advantage of approximately:

MA = 6.57


### Selecting Nut Position

Assume the nut center is located:

|AN| = 50 mm

Distance from hinge to grip:

|AG| = 6.571 × 50  
|AG| = 328.55 mm

Rounded for design:

|AG| ≈ 350 mm


### Handle Length Calculation

From the geometry of the sketch, the vertical offset between hinge and grip is approximately:

|BG| = 48 mm

Using the Pythagorean theorem:

|AB| = √(350² + 48²)

|AB| = √(122500 + 2304)

|AB| ≈ 353 mm

Using the dimensions in the design sketch:

|AB| ≈ 363.46 mm


## 4. Usability of the Design

This design is practical because the long handles create a mechanical advantage that multiplies the user's applied force, allowing an average person to crack a macadamia nut.

### Advantages

• simple lever mechanism  
• symmetric design distributes force evenly  
• large mechanical advantage  
• easy to manufacture  

### Limitations

• handles around 360 mm long may be slightly large for compact storage  
• misalignment of the nut could cause uneven loading  
• real macadamia nuts vary slightly in cracking force  

### Possible Improvements

• rubber grips for better comfort  
• shaped grooves to hold the nut securely  
• curved handles for better ergonomics  


## Final Design Summary

Required cracking force: ~2300 N  
Human grip force: ~350 N  
Mechanical advantage: 6.57  
Distance from hinge to nut: 50 mm  
Handle length: ~363 mm  


## Conclusion

By modeling the nutcracker as a lever system, it is possible to design a tool that allows a user with average grip strength to crack a macadamia nut. Placing the nut close to the hinge and using long handles creates the mechanical advantage necessary to generate the required cracking force. The final design uses a hinge-to-nut distance of approximately 50 mm and handle lengths of roughly 363 mm to achieve this result.
