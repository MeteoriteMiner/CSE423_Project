# Rolling Ball Runner

A 3D endless runner built from scratch with PyOpenGL and GLUT — dodge obstacles, collect coins, and use power-ups while the camera follows your ball down an infinite track.

This was originally built as a group project for **CSE423 (Computer Graphics), BRAC University**. This repository is a fork of the [original team repo](https://github.com/Mayen-Shahriar-Kabir/CSE423_Project), cleaned up and maintained here as part of my personal portfolio.

**Team:** [Anirban Saha](https://github.com/MeteoriteMiner) (initial setup and core game loop), [Mayen Shahriar Kabir](https://github.com/Mayen-Shahriar-Kabir), and [suhanaprova](https://github.com/suhanaprova).

## Gameplay

- Endless 3-lane runner rendered with raw OpenGL primitives (no game engine) — camera, lighting, and collision are all hand-built
- Procedurally placed obstacles and coins along the track
- Power-ups: shield, speed boost, shrink, and a spin attack that clears nearby obstacles
- Increasing difficulty — move speed ramps up the longer you survive
- Free camera controls and an optional first-person mode

## Controls

| Key | Action |
|---|---|
| `A` / `D` | Move left / right |
| `Space` | Jump |
| `F` | Spin attack (clears obstacles, limited uses) |
| `S` | Shrink (temporary size reduction) |
| `R` | Restart after game over |
| `C` | Toggle cheat mode |
| Arrow keys | Adjust camera height / rotation |
| Right-click | Toggle first-person view |

## Running it locally

```bash
pip install -r requirements.txt
python main.py
```

Requires Python 3 and a system that supports OpenGL/GLUT (most Windows, Mac, and Linux desktops do by default; on Linux you may need `freeglut3` installed via your package manager).

## What I worked on

I built the initial project setup and most of the core systems: the 2D-to-3D rendering setup, forward ball movement and jumping, random spawning of obstacles and collectibles along the track, scoring and penalties, the bonus/power-up triggers, the restart-on-R flow, the menu, and the camera system including both first-person and third-person modes. Teammates built on this foundation with additional polish and features.
