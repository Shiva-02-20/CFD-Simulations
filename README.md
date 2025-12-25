# CFD-Simulations



# CFD Analysis of NACA 64-206 Airfoil (STAR-CCM+)



## Overview

This repository presents a **2D CFD investigation of the aerodynamic performance of the NACA 64-206 airfoil** using **STAR-CCM+**.  

The study focuses on evaluating **lift, drag, pressure distribution, velocity fields, flow separation, and stall behaviour** across a range of angles of attack.



The analysis was conducted under steady-state conditions using a refined mesh strategy and convergence-driven validation.



---



## Objectives

- Evaluate lift and drag characteristics of the NACA 64-206 airfoil

- Study pressure and velocity distribution at different angles of attack

- Identify stall angle and associated flow separation

- Ensure numerical accuracy through mesh convergence and quality checks



---



## Geometry

- Airfoil: **NACA 64-206**

- Geometry coordinates obtained from the UIUC airfoil database

- Coordinates refined and imported into STAR-CCM+ as a 2D curve



---



## Computational Setup



### Solver

- Software: **STAR-CCM+**

- Dimensionality: **2D**

- Flow type: Incompressible, steady-state



### Boundary Conditions

 Boundary  Type 

|-------|------|

| Inlet | Freestream velocity |

| Outlet | Pressure outlet |

| Outer boundaries | Far-field |

| Airfoil surface | No-slip wall |



- Airflow velocity: **50 m/s**

- Angle of attack varied by adjusting flow direction



---



## Mesh Strategy

- 2D domain with a **semi-circular inlet region**

- Fine mesh refinement near the airfoil surface

- Wake refinement downstream of the trailing edge

- Target mesh size: **0.007**

- Growth rate: **1.3**

- Spread angle: **15°**



### Mesh Convergence

Mesh convergence was performed by progressively refining the mesh until variations in lift and drag coefficients became insignificant relative to increased computational cost.



---



## Mesh Quality Assessment

- **Wall y⁺ analysis** performed to ensure valid near-wall treatment

- Majority of mesh cells exhibited skewness angles **below 30°**, indicating high mesh quality

- Skewness angles maintained below the recommended threshold of **85°**



---



## Aerodynamic Analysis



### Lift and Drag

- Lift coefficient increases with angle of attack up to stall

- Drag coefficient increases rapidly beyond stall

- Performance assessed using **Cl, Cd, and Cl/Cd ratios**



### Stall Behaviour

- **Stall angle identified at approximately 7.9°**

- Beyond stall, residuals became erratic due to flow separation

- Loss of convergence used as an indicator of stall onset



---



## Pressure Distribution

- Pressure difference between upper and lower surfaces increases with angle of attack

- Maximum pressure observed near the **leading edge**

- At stall, pressure redistribution occurs towards the mid-chord, correlating with lift reduction



---



## Velocity Field

- Highest velocity observed over the upper surface at positive angles of attack

- NACA 64-206 exhibited higher local velocities compared to thicker airfoils in the same family

- Velocity reduced near the surface due to boundary layer effects



---



## Flow Separation

- Flow remained largely attached at low angles of attack

- Separation initiated near the trailing edge as angle of attack increased

- At stall, large separation regions formed, leading to lift degradation



---



## Results Summary

- Mesh convergence ensured numerical reliability

- Lift increased linearly with angle of attack until stall

- Stall occurred at a lower angle compared to thicker airfoils in the NACA 64 series

* y+ wall value was between 0 and 5

- NACA 64-206 showed relatively **laminar trailing-edge flow**, indicating higher aerodynamic efficiency



---



## Limitations

- 2D analysis neglects three-dimensional effects

- Steady-state assumption limits unsteady stall prediction

- No experimental validation included



---



## Tools Used

- STAR-CCM+

- Microsoft Excel (geometry preprocessing)



---



## Author

**Shivasubramanian Ramkumar**  

MSc Mechanical Engineering  

University of Portsmouth