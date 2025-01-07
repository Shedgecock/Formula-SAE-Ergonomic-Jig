# Race Car Ergonomics Jig (Phase II)

![Proto6_1](https://github.com/user-attachments/assets/570ce05a-7a46-4898-af63-d41dbdd97730)

> **A modular, adjustable, and collapsible jig designed to optimize driver ergonomics for Formula SAE Electric Vehicles. Developed to enhance Aztec Electric Racing’s testing capabilities at San Diego State University.**

<div align="center">
  <img src="https://img.shields.io/badge/Status-In%20Progress-blue.svg" alt="Project Status">
  <img src="https://img.shields.io/badge/License-SDSU-green.svg" alt="License: SDSU">
  <img src="https://img.shields.io/badge/Tech-SolidWorks-lightgrey.svg" alt="Tech stack: SolidWorks">
  <img src="https://img.shields.io/badge/FEA-Ansys%20|%20SolidWorks-orange.svg" alt="FEA Tools: Ansys | SolidWorks">
</div>

---

## Table of Contents

1. [Project Goals](#project-goals)  
2. [Features](#features)  
3. [Design Highlights](#design-highlights)  
4. [Technical Documentation](#technical-documentation)  
   - [Trade Studies](#trade-studies)  
   - [Engineering Analysis](#engineering-analysis)  
   - [Prototyping and Testing](#prototyping-and-testing)  
5. [Lessons Learned](#lessons-learned)  
6. [How to Use](#how-to-use)  
   - [Installation](#installation)  
   - [Usage](#usage)  
8. [References](#references)  
9. [License](#license)  

---

## Project Goals

- **Ergonomic Range**: Accommodate 5th percentile female to 95th percentile male drivers.  
- **Compliance**: Ensure alignment with FSAE EV rulebook and safety standards.  
- **Collapsibility**: Support quick disassembly and storage in a 57-gallon bin.  
- **Modularity**: Enable interchangeable components (pedal box, steering column, seat) for future AER car iterations.  

> **Why It Matters**  
> \- This jig empowers electric racing teams to streamline driver testing, enhance on-track safety, and reduce lead time in optimizing cockpit ergonomics.

---

## Features

- **Tool-Free Adjustments**  
  Quick-release mechanisms allow seat and pedal positioning without specialized tools.

- **Multi-Degree Seat Assembly**  
  Pivoting seat mount plus telescoping punched tubing for seamless angle changes.

- **Integrated Harness & Headrest**  
  Built-in harness bar and adjustable headrest simulating real FSAE roll hoop geometry.

- **Storage Efficiency**  
  Collapsible to fit compact bins, maximizing limited shop space and portability.

---

## Design Highlights

1. **T-slot Aluminum Extrusions**  
   - High strength-to-weight ratio and straightforward assembly via standard 80/20 components.  

2. **Prototyping with 3D Printing**  
   - 1:6 scale PLA models to test basic geometry and module mobility.  

3. **Advanced Ergonomics**  
   - Incorporates FSAE egress rules, seat recline angles, and adjustable pedal positions for thorough driver coverage.  

4. **Validated via FEA**  
   - Multiple load scenarios (up to 450 lbs braking force) verified for frame and mounting plates.  

---

## Technical Documentation

### Trade Studies

- **Base Frame Layout**: Compared rectangular, single-beam, and two-level sliding bases for structural integrity vs. weight.  
- **Collapsibility Methods**: Sliding vs. hinge vs. disassembly, selecting the disassembly approach to maintain measurement repeatability.  

### Engineering Analysis

- **Seat Exo-Skeleton**: Free body diagrams, shear, and moment analyses combined with SolidWorks/Ansys FEA.  
- **Pedal Box Mount**: Verified under a 450 lb braking load. Achieved a factor of safety > 14 with minimal deflection.  
- **Frame Structure**: Replaced hinges with internal butt fasteners and dowel pins for improved load distribution.
- Refer to the [Engineering Analysis](https://github.com/Shedgecock/Formula-SAE-Ergonomic-Jig/blob/a6188684190f81b6f10be2cc678db0f85ad69125/Engineering%20Analysis.pdf) file for technical context and analysis.

### Prototyping and Testing

- **Scaled 3D Prints**: Simple geometry prototypes used to test steering, pedal, and seat movement.  
- **Iterative Refinements**: Widened back pillars, reduced complexity of pivot joints, and integrated sponsor feedback on adjustability.

---

## Lessons Learned

- **Team Coordination**: Importance of transparent communication channels (weekly meetings, group chats) to manage overlapping assignments.  
- **Iterative Design Process**: Leveraged sponsor feedback to refine pedal box angles, steering mounts, and seat brackets.  
- **Documentation & Version Control**: Maintaining consistent CAD models avoided confusion in final design presentations.  
- **Time Management**: Balanced academic workloads, part lead times, and sponsor expectations effectively.

---

## How to Use

### Installation
Use **SolidWorks 2022** or later (or a compatible viewer) to open the `.SLDASM` and `.SLDPRT` files located in the `CAD/` directory.

### Usage

1. **Customize CAD Components**  
   - Adjust seat angles, pedal box positions, or steering column length directly in SolidWorks.  
   - All major subassemblies can be found in the `CAD/` folder, and you can refer to the final assembly file to see the complete jig.

2. **Review FEA Studies**  
   - Open Ansys/Simulation files located in `./analysis` to validate load capacities and confirm factors of safety.  
   - Check boundary conditions, applied loads, and mesh settings to ensure they align with your specific design scenario.

3. **Prototype or Manufacture**  
   - Refer to `./docs/BOM.md` for a comprehensive Bill of Materials (BOM), including 80/20 part numbers and recommended fasteners.  
   - Use **SendCutSend** or a similar service for custom laser-cut parts, following your design’s required tolerances and materials.

---

## References

- **Formula SAE Rules 2024 (Version 1.0)*
- **Dr. Shaffar ME490W Lecture Slides*
- **80/20 Inc. T-slot Extrusion Catalog*
- **SendCutSend - Laser-cut custom brackets and plates*
- **Boskovich et al.: Ergonomic Jig Phase I Documentation (2023)*

---

## License

> **Disclaimer**  
> This project is licensed through **San Diego State University** (SDSU).  
> Usage, distribution, and modifications should adhere to the licensing terms set by SDSU and the Aztec Electric Racing Team (AER).  
>  
> If you plan to use or adapt this project outside the SDSU/AER context, please reach out to us at  
> [shedgecock5567@sdsu.edu](mailto:shedgecock5567@sdsu.edu) for additional guidance and permissions.
