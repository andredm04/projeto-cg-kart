# 3D Kart Garage

An interactive 3D computer graphics project developed in Python using PyOpenGL and GLFW.

The project features a stylized kart driving through a 3D garage environment, combining real-time rendering, scene graphs, animation, lighting, textures, camera control and collision detection.

## Overview

The application creates an interactive 3D garage scene where the user can control a kart and explore the environment.

The scene is built around a custom scene graph, allowing the different components of the kart and environment to be organized hierarchically. In addition to rendering the scene, the project includes interactive movement, collision handling and animated environmental elements.

Main features include:

- Interactive 3D kart
- Textured garage environment
- Kart movement and steering
- Collision detection with walls and scene objects
- Orbit and first-person camera modes
- Animated garage door
- Animated lighting and environmental elements
- Hierarchical scene organization using a custom scene graph
- Texture mapping
- Real-time OpenGL rendering

## Technologies

- Python
- PyOpenGL
- GLFW
- OpenGL

## Project Structure

```text
.
├── main.py
├── scene.py
├── graphics.py
├── geometry.py
├── materials.py
├── scenegraph.py
├── floor.jpg
├── wall.png
├── garage-door.png
└── ...
```

### `main.py`

The entry point of the application.

It is responsible for creating the scene and starting the rendering process.

### `scene.py`

The main scene definition and logic of the project.

It includes:

- Kart geometry and components
- Kart movement and steering
- Collision detection
- Garage door animation
- Sun and light pole animation
- Scene construction
- Object organization through the scene graph

### `graphics.py`

Handles the rendering and interaction layer of the application.

Its responsibilities include:

- OpenGL setup
- Rendering loop
- Camera control
- Input handling
- HUD rendering

### `geometry.py`

Contains primitive geometry drawing functions used to build the different objects in the scene.

### `materials.py`

Contains material and lighting definitions used during rendering.

### `scenegraph.py`

Implements the custom scene graph used to organize the hierarchical relationships between objects in the scene.

## Scene

The environment is built as a 3D garage containing a stylized kart and several interactive or animated elements.

The kart is composed of multiple individual components, including:

- Wheels
- Doors
- Lights
- Roof
- Trunk
- Body components

These elements are organized hierarchically using the scene graph, allowing complex objects to be constructed from simpler parts and transformed as a single structure.

The garage environment uses textures for surfaces such as the floor, walls and garage door.

## Controls

The kart can be controlled using the keyboard:

| Key | Action |
|-----|--------|
| `W` | Move forward |
| `S` | Move backward |
| `A` | Steer left |
| `D` | Steer right |

The application also includes camera controls and additional interaction handling through keyboard and mouse input.

## Camera System

The project supports multiple camera modes for navigating and viewing the 3D environment.

### Orbit Camera

Allows the user to rotate around the scene and inspect the kart and environment from different angles.

### First-Person Camera

Provides a first-person perspective from the kart for a more immersive driving experience.

## Rendering and Animation

The project uses OpenGL to render the 3D environment in real time.

Several animated elements are implemented within the scene, including:

- Kart movement and steering
- Garage door movement
- Sun animation
- Light pole animation
- Environmental lighting changes

The scene combines geometry, materials, textures, lighting and transformations to create the final rendered environment.

## Scene Graph

A custom scene graph is used to organize the scene into a hierarchy of nodes.

This structure makes it possible to model complex objects by combining simpler components while preserving relationships between their transformations.

For example, the kart can be represented as a hierarchy containing its body, wheels, doors, lights and other components. Transformations applied to parent nodes can therefore affect the corresponding child objects.

This approach simplifies both scene construction and object manipulation.

## Collision Detection

The kart includes basic collision detection with walls and objects in the environment.

This prevents the kart from moving freely through defined scene boundaries and provides more realistic interaction with the garage environment.

## Running the Project

Clone the repository:

```bash
git clone https://github.com/andredm04/projeto-cg-kart.git
cd projeto-cg-kart
```

Install the required dependencies:

```bash
pip install PyOpenGL glfw
```

Run the application:

```bash
python main.py
```

Note: Additional dependencies or specific Python versions may be required depending on the original development environment.

## Project Context

This project was developed as a university computer graphics project focused on the implementation of an interactive 3D environment.

The main concepts explored include:

- 3D scene construction
- Hierarchical modeling
- Scene graphs
- OpenGL rendering
- Lighting and materials
- Texture mapping
- Animation
- Camera systems
- User interaction
- Collision detection

## What I Worked On

This project provided practical experience with fundamental concepts of real-time 3D computer graphics.

The development involved building and organizing a complete 3D scene, implementing hierarchical object relationships, handling user input, controlling cameras, applying lighting and materials, adding textures, implementing animations and integrating collision detection.

The project also required combining multiple graphics components into a single interactive application using a custom rendering and scene management structure.
