# Fifty Bird

**Fifty Bird** is a clone of the classic Flappy Bird game, built using the **Lua programming language** and the **LÖVE2D game framework**. This project is part of the **Harvard CS50’s Introduction to Game Development** course. It focuses on recreating the mechanics of Flappy Bird while exploring core game development concepts such as object-oriented programming, collision detection, state machines, and frame-based animation.

---

## Gameplay

The player controls a bird that automatically falls due to gravity. The goal is to navigate the bird through pairs of pipes by flapping (pressing a key to make it rise). The game ends when the bird collides with a pipe or the ground.

---

## Features

* Smooth vertical physics for bird motion (gravity and jump impulse)
* Randomized pipe generation for dynamic obstacles
* State machine system managing different screens (title, countdown, play, score)
* Pixel-perfect collision detection
* Score tracking based on pipe traversal
* Parallax scrolling background and ground
* Simple and responsive input handling

---

## Built With

* **Language:** Lua
* **Framework:** [LÖVE2D](https://love2d.org/)
* **Course:** [CS50G: Introduction to Game Development](https://cs50.harvard.edu/games/)

---

## Getting Started

### Prerequisites

To run the game, you need:

* [Lua](https://www.lua.org/)
* [LÖVE2D](https://love2d.org/) (version 11.3 or compatible)

### Running the Game

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/fifty-bird.git
   cd fifty-bird
   ```

2. Run the game using LÖVE:

   ```bash
   love .
   ```

---

## File Structure

```
fifty-bird/
├── main.lua               -- Entry point of the game
├── StateMachine.lua       -- Custom state machine implementation
├── Bird.lua               -- Bird class with movement and collision logic
├── Pipe.lua               -- Pipe class for single pipe objects
├── PipePair.lua           -- PipePair class for top and bottom pipes
├── util.lua               -- Helper functions
├── states/                -- Game states (title, play, score, countdown)
│   ├── BaseState.lua
│   ├── TitleScreenState.lua
│   ├── CountdownState.lua
│   ├── PlayState.lua
│   └── ScoreState.lua
├── assets/                -- Sprites and sound assets
```

---

## What I Learned

* Fundamentals of 2D game physics and animation
* Lua's table-based OOP implementation
* Finite state machines for game state management
* Reusable game components and structure
* Handling frame-rate independence
* Building games using LÖVE2D

---

## License

This project is for educational purposes as part of the CS50G course. You are free to use and modify it for your learning or personal use. Commercial use of Flappy Bird assets may be restricted under copyright.

---

## Acknowledgements

* [CS50G - Harvard University](https://cs50.harvard.edu/games/)
* Original Flappy Bird by Dong Nguyen
* The LÖVE2D community and documentation

---