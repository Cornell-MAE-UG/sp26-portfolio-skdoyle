---
layout: project
title: Nutcracker Project Part 2
technologies: N/A
image: <img width="1070" height="368" alt="Screenshot 2026-05-02 at 5 22 08 PM" src="https://github.com/user-attachments/assets/1c3bf476-876a-4f12-923b-aac8dd7fe8fe" />

---

# Part 2

# Nutcracker Handle Beam Design

## Overview
This project analyzes the flexibility of nutcracker handles when they are no longer assumed rigid. The handles are modeled as beams that bend under applied forces from both the nut and the user. The goal is to determine where maximum deflection occurs and to design a beam cross-section that limits deflection while remaining mass-efficient.


## 1. Problem Statement and Objective ("Find")

Design the nutcracker handles as beams such that they remain structurally efficient and do not deflect excessively under load.

The goals are to determine:

• the location of maximum elastic deflection  
• a suitable beam cross-section and material  
• a final design that limits deflection to less than 2% of the beam length  


## 2. Constraints and Input Parameters ("Given")

### Forces (from previous analysis)

Total cracking force:

FN ≈ 2300 N  

Because the system is symmetric:

FNU = FNL = 1150 N  

User grip force:

FG ≈ 350 N  

Split between handles:

FGU = FGL = 175 N  


### Geometry

Total handle length:

L = 0.35 m  

Distance from hinge to force application:

a = 0.0702 m  


### Material Properties

Material selected:

Stainless steel  

Young’s modulus:

E = 193 GPa  


## 3. Approach to the Problem

The handle is modeled as a beam with a point load offset from the support.


### Maximum Deflection Location

Using standard beam deflection relationships:

x_max = sqrt((L² − a²) / 3)

Substitute values:

x_max = sqrt((0.35² − 0.0702²) / 3)

x_max ≈ 0.197 m  

So the maximum deflection occurs:

≈ 0.197 m from the hinge  


### Reaction Force Calculation

Taking moments about the hinge:

Fn × 0.0702 + Fg × 0.35 = 0  

Fn = −(175 × 0.35) / 0.0702  

Fn ≈ −803.8 N  


### Deflection Constraint

Maximum allowable deflection:

δ_max = 0.02 × L  

δ_max = 0.02 × 0.35  

δ_max = 0.007 m  

Using the beam deflection relationship and solving for stiffness:

Required flexural rigidity:

EI ≈ 63.93  

So the required second moment of area is:

I > 3.312 × 10⁻¹⁰ m⁴  


### Cross-Section Selection

For a rectangular beam:

I = (b × h³) / 12  

To maximize stiffness efficiently:

• increase height (h)  
• keep width (b) small  

Trial dimensions:

b = 0.005 m (5 mm)  
h = 0.0095 m (9.5 mm)  

Calculated:

I ≈ 3.572 × 10⁻¹⁰ m⁴  

This satisfies the requirement.


## 4. Final Beam Design

Material:

• Stainless steel  

Cross-section:

• Width = 5 mm  
• Height = 9.5 mm  

Geometry:

• Length = 350 mm  
• Load applied ≈ 70 mm from hinge  


## 5. Design Evaluation

This design meets the deflection constraint while maintaining a relatively small cross-sectional area.

### Advantages

• high stiffness due to tall rectangular profile  
• simple geometry for manufacturing  
• strong and durable material  
• deflection within allowable limits  

### Limitations

• stainless steel is not the most mass-efficient material  
• slightly larger height may affect handle comfort  
• assumes ideal loading and alignment  


### Possible Improvements

• use aluminum to reduce weight  
• optimize cross-section further (e.g., I-beam shape)  
• improve ergonomics with rounded edges  
• add grip materials to handles  


## Final Design Summary

Maximum deflection location: ~0.197 m from hinge  
Maximum allowable deflection: 0.007 m  
Required moment of inertia: > 3.312 × 10⁻¹⁰ m⁴  

Selected design:

• Material: Stainless steel  
• Cross-section: 5 mm × 9.5 mm  
• Length: 350 mm  


## Conclusion

By modeling the nutcracker handle as a beam rather than a rigid body, it is possible to design a structure that maintains structural integrity under load. The analysis shows that maximum deflection occurs near the mid-region of the handle, and that increasing the second moment of area is key to reducing deflection. A rectangular cross-section with greater height than width provides an efficient solution, meeting the deflection requirements while keeping the design practical.
