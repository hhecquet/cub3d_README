# cub3d

> [!IMPORTANT]
> None of my code is publicly available here, but if you're a recruiter, I'd be happy to share it with you upon request.

<p align="center"> 
  <img width="318" height="272" alt="Screenshot from 2025-07-24 10-52-37" src="https://github.com/user-attachments/assets/c4063a37-0364-4dfd-bec0-2e0f68c44350" />
</p>

The Cub3D project is a 42 graphics and game engine assignment where I created a basic 3D first-person perspective game using raycasting, inspired by early games like Wolfenstein 3D. The core goal was to render a 3D environment from a 2D map, with textures, player movement, and basic interactions — all built from scratch using C and the MiniLibX graphics library.

This project introduced me to the principles of raycasting, game loops, and real-time rendering, while also reinforcing low-level graphics programming skills.

What I had to do:
Parse and validate a .cub configuration file containing:
A 2D map layout
Texture paths for each wall direction (N, S, E, W)
RGB color values for the ceiling and floor
Render a 3D environment using raycasting, projecting wall slices based on distance
Implement a player with real-time movement (forward, backward, left, right)
Handle rotation for looking left and right using key inputs
Load and render textures onto walls depending on ray direction and collision point
Manage a continuous game loop with keyboard input and dynamic frame rendering
To achieve this, I had to:
Calculate ray-wall intersections using DDA (Digital Differential Analysis)
Map 2D coordinates to screen-space for accurate rendering
Normalize and manage angles to prevent distortion
Control frame updates efficiently for smooth gameplay
Design and enforce a solid parsing and error-handling system for the .cub file

Bonus Part: Full Collision Detection
For the bonus, I implemented full collision detection to improve gameplay realism:
Prevented the player from walking through walls or clipping through corners
Added checks against the surrounding map grid to ensure accurate collision boundaries
Fine-tuned movement precision to allow smooth motion while still respecting solid boundaries
Considered diagonal collisions and edge detection to avoid glitches or sliding into invalid spaces
This feature made the player movement feel much more natural and immersive, and required precise control over position updates and map checks per frame.

What I Learned:
Core principles behind raycasting and 3D projection from 2D data
How to build a basic rendering engine using pixel-by-pixel control
Parsing and validating structured input files with edge-case handling
Real-time input management and event-driven rendering loops
Implementing precise collision detection and managing spatial constraints
Working with low-level graphic libraries like MiniLibX

Cub3D was a true milestone in my C journey — combining mathematics, graphics, and real-time logic. Implementing full collision detection made the game feel polished and taught me how much fine-tuning goes into even the simplest game mechanics.

<p align="center"> 
  <img width="503" height="282" alt="maze" src="https://github.com/user-attachments/assets/e0d76d9f-fa95-441e-945f-208941e687eb" />
  <img width="503" height="282" alt="simple" src="https://github.com/user-attachments/assets/7d9c0726-df5b-4d3f-bbe7-49bc995b7696" />
</p>

Project done with [heperez](https://github.com/hdprz)
