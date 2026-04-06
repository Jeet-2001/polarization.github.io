# Polarization Optics Visual Lab

An interactive, web-based physics simulation for exploring polarization optics. This visual lab allows users to build dynamic optical chains and analyze light polarization using Jones Calculus and Stokes Polarimetry.

[**View Live Site**](https://jeet-2001.github.io/polarization.github.io/)

---

## Overview

The **Polarization Optics Visual Lab** provides a sandbox environment to simulate the flow of light from a source through various optical components to a detector. It calculates and visualizes the state of polarization at each step in real-time, bridging the gap between abstract mathematical matrices and physical wave behaviors. 

## Features

* **Dynamic Chain Architecture:** Easily add, remove, and reorder optical components in the pipeline.
* **Dual Calculation Methods:** * Optical Bench (Jones Calculus)
  * Stokes Polarimetry Setup
* **Comprehensive Component Library:** Includes Linear Polarizers, Half-Wave Plates (HWP), Quarter-Wave Plates (QWP), Right/Left Circular Polarizers (RCP/LCP), Elliptical Polarizers, and Polarizing Beam Splitters.
* **Interactive 3D Optical Bench:** Physically drag and drop components along the z-axis. Features orbit, pan, and zoom functionality for full spatial awareness.
* **Real-Time Mathematical Analysis:** Instant display of the input wave vector ($E_{in}$), the overall system matrix ($J_{sys}$), and the resulting output wave vector ($E_{out}$).
* **Data Visualization:** Live 2D plotting of the Intensity Profile ($I$) and Wave Analysis across the optical bench position.

## How to Use

1. **Build the Pipeline:** Click **[+ Add Optic]** to insert new optical components into the flow.
2. **Adjust Parameters:** Modify the fast axis or transmission angle (e.g., setting a Linear Polarizer to 45° or a HWP to 0°) using the control sliders.
3. **Position Optics:** Drag components horizontally in the 3D view to adjust their physical spacing ($x$ position in cm) along the bench.
4. **Analyze Results:** Observe the transformation in the 2D Optical Setup Overview, check the updated matrices, and review the Intensity Profile graphs to see how the wave behaves before and after attachments.

## Mathematical Foundation

The simulation relies on matrix multiplication to determine the final state of light. For a system of optical components, the overall system matrix ($J_{sys}$) is calculated and multiplied by the input wave vector ($E_{in}$) to yield the output wave ($E_{out}$):

$$E_{out} = J_{sys} E_{in}$$
