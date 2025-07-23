# Tap Tap Wacom

This project explores the convergence of tangible input and real-time 3D physics simulation. Designed as an interactive installation, it uses a **Wacom A5 touch tablet** as a physical surface to influence a virtual scene rendered using **HARFANG 3D**.

## Concept

The Wacom tablet is placed horizontally in front of the screen, creating an illusion of continuity between the physical and virtual space. When the user touches the tablet with a finger (no stylus required), an **invisible  collision sphere** is moved across the virtual plane, pushing solid objects out of it. Once all solids fall off, the simulation resets.

Future developments could include **head tracking with a Kinect sensor**, so the 3D perspective adjusts to the viewer’s position, reinforcing the illusion of depth.

## Technical Overview

- **Input**: Wacom A5 touch tablet, recognized as a standard mouse input.
- **Engine**: HARFANG 3D with Bullet physics.
- **Interaction**:
  - Touch triggers a repulsive force or displacement sphere in the virtual scene.
  - Physics objects are pushed and fall off a virtual platform.
  - Once the scene is empty, it resets with a new arrangement.
- **Perspective**:
  - The tablet is aligned with the screen to create a seamless interactive surface.
  - Optional Kinect integration for adaptive viewpoint tracking.

## Artistic Direction

While the current implementation focuses on technical feasibility and interaction design, future iterations will explore **narrative and symbolic layers** — possibly commenting on manipulation, entropy, or the illusion of control.

### Rendering & Immersive Ideas

- Minimalist lighting setup using a single spotlight and shadowmap, evoking a black-box studio atmosphere
- PBR materials to replicate the look and feel of the physical Wacom tablet
- Kinect-powered head tracking for dynamic perspective adjustment
- Haptic feedback by strapping an Xbox controller underneath the tablet (experimental)
