# 🎯 Traim - 3D Shooting Game

**Traim** is a 3D target-shooting game developed entirely in Python for CSE423: Computer Graphics.

The game features real-time 3D rendering, mouse-controlled aiming, multiple weapons, dynamic targets, customizable settings, and different gameplay modes. It combines interactive gameplay with fundamental computer graphics concepts, including camera transformations, perspective projection, and ray-sphere collision detection.

## 🎮 Features

- **3D Gameplay:** Perspective-based rendering with a movable camera and mouse-controlled aiming.
- **Multiple Weapons:** Choose between Pistol, Shotgun, and Sniper.
- **Multiple Game Modes:** Includes Easy, Medium, Hard, Practice, Reaction, and Fixed modes.
- **Dynamic Targets:** Targets can move, bounce off boundaries, shrink over time, and require multiple hits.
- **Collision Detection:** Uses ray-sphere intersection calculations to determine whether shots hit targets.
- **Visual Effects:** Bullet tracers, hit effects, and a sniper scope overlay.
- **Customizable Settings:** Adjust mouse sensitivity, target size, target color, and crosshair color.
- **Scoring System:** Tracks scores, shots fired, successful hits, misses, accuracy, and reaction times.
- **Interactive Menus:** Includes a main menu, settings screen, and game-over screen.
- **Optional Cheat Mode:** Includes an auto-aim mode for experimentation.

## 🕹️ Gameplay

Choose your preferred game mode, duration, and weapon from the main menu. Once the game starts, aim at the targets using your mouse and shoot to increase your score.

Different game modes introduce different target behaviors and objectives, offering a variety of ways to practice aiming and reaction speed.

## 🧰 Technologies Used

- **Language:** Python
- **Graphics:** OpenGL
- **Windowing and Input:** GLUT
- **3D Rendering:** Perspective projection and camera transformations
- **Collision Detection:** Ray-sphere intersection
- **Mathematical Concepts:** Vectors, direction calculations, and geometric intersection tests

## 🎯 Weapons

| Weapon | Description |
|---|---|
| Pistol | Fires a single shot in the aiming direction. |
| Shotgun | Fires multiple pellets with randomized spread. |
| Sniper | Uses a scoped view with a narrower field of view. |

## 🧩 Game Modes

| Mode | Description |
|---|---|
| Easy | Practice aiming at stationary targets. |
| Medium | Targets move and shrink over time. |
| Hard | Provides a more challenging target-shooting experience. |
| Practice | Focuses on hitting a specified number of targets. |
| Reaction | Tracks the time taken to hit targets. |
| Fixed | Challenges the player to hit a fixed number of targets. |

## 🎮 Controls

### Menu and Settings

| Key | Action |
|---|---|
| `W` / `S` | Navigate menu options |
| `A` / `D` | Change the selected option |
| `Enter` | Select an option or confirm a selection |

### Gameplay

| Input | Action |
|---|---|
| Mouse movement | Aim |
| Left mouse button | Shoot |
| Right mouse button | Toggle sniper scope |
| `W` / `A` / `S` / `D` | Move the player |
| `C` | Toggle cheat mode |
| `M` | Return to the main menu |
| `R` | Return to the menu from the game-over screen |

*The sniper scope is available when using the Sniper weapon.*

## ⚙️ Installation and Setup

### Prerequisites

- Python 3
- pip
- OpenGL-compatible graphics support
- GLUT or a compatible FreeGLUT installation

### 1. Clone the repository

```bash
git clone https://github.com/farabi092/Traim-3D-Shooting-Game.git
cd Traim-3D-Shooting-Game
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

On macOS or Linux:

```bash
source .venv/bin/activate
```

### 3. Install the Python dependencies

Install the Python packages required by the project.

For example, if the project imports PyOpenGL:

```bash
pip install PyOpenGL PyOpenGL_accelerate
```

Make sure GLUT or FreeGLUT is installed and available on your system.

*The exact dependencies may vary depending on your operating system and project configuration.*

### 4. Run the game

Run the main Python file:

```bash
python traim.py
```

If your main file has a different name, replace `traim.py` with the appropriate filename.

## 🧠 Computer Graphics Concepts

Traim incorporates several concepts from computer graphics and computational geometry.

- **Perspective Projection:** Uses `gluPerspective` to render the 3D scene.
- **Camera Transformations:** Uses `gluLookAt` with yaw and pitch to control the viewing direction.
- **2D and 3D Rendering:** Combines perspective-based gameplay with orthographic 2D menu and HUD overlays.
- **Ray-Sphere Intersection:** Calculates whether an aiming ray intersects a target sphere.
- **Vector Mathematics:** Uses direction vectors and geometric calculations for aiming and collision detection.
- **Animation and Visual Effects:** Updates moving targets, bullet tracers, and hit effects over time.
- **Event-Driven Interaction:** Uses keyboard, mouse, and GLUT callbacks to handle input and rendering.


## 🎓 Academic Context

Developed as a project for **CSE423: Computer Graphics** at BRAC University.
The project explores interactive 3D rendering, geometric collision detection, camera control, and real-time input handling through a Python-based game.
