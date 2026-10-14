# 3D Sumo Game (Python + OpenGL)

A two-player 3D sumo game built with **PyOpenGL** and GLUT for a computer graphics course at BRAC University. Two sumo wrestlers push each other inside a circular arena, and the first one pushed out of the ring loses. After 20 seconds the arena starts shrinking, and if nobody wins within 30 seconds the round is a draw.


![Gameplay](screenshot.png)


## Features

- 3D arena, stadium walls and sumo players drawn with OpenGL primitives (quadrics, spheres, cubes, triangle fans)
- Animated crowd of three rings of spectators, with waving arms and bouncing motion
- Player collision with push-back
- Shrinking arena after 20 seconds, with a background colour change as a warning
- 30-second match timer, win and draw detection, and instant restart
- Camera that follows the midpoint between the two players

## Controls

| Action | Player 1 (red) | Player 2 (blue) |
|--------|----------------|-----------------|
| Move up | W | Up arrow |
| Move down | S | Down arrow |
| Move left | A | Left arrow |
| Move right | D | Right arrow |

Press **R** after a round ends to restart.

## Requirements

- Python 3.8+
- PyOpenGL (includes the GLUT bindings)

## Installation and Run

```bash
pip install -r requirements.txt
python sumo_game.py
```

You can also open `sumo_game.py` in VS Code and run it from there.

**Windows:** the PyOpenGL package bundles the GLUT library, so `pip install PyOpenGL` is normally enough.

**Linux:** install freeglut first:
```bash
sudo apt install freeglut3-dev
```

**macOS:** GLUT is included with the system.

## Repository Structure

```
.
├── sumo_game.py        # Full game source code
├── requirements.txt
└── README.md
```
