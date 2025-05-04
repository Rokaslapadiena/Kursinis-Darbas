# 🕹 Pong Game - Python (Pygame)

A Python implementation of the classic arcade game **Pong**, developed using the `pygame` library. This version supports two players with keyboard controls, scoring, collision mechanics, and a win condition.

---

## 📦 Features

- Two-player paddle control (W/S and ↑/↓)
- Realistic ball bounce and angle control
- Score tracking with win condition
- Simple retro visuals
- Modular object-oriented design

---

## 🧠 Code Architecture

### 🗂 Main Components

- `GameObject`: Abstract base class with position and reset logic
- `Paddle`: User-controlled paddles with movement restrictions
- `Ball`: Moves with velocity, resets on scoring, detects paddle/wall collisions
- `draw()`: Handles rendering paddles, ball, score, and center divider
- `handle_collision()`: Physics and collision detection
- `handle_paddle_movement()`: Keyboard input and paddle motion
- `main()`: Game loop handling events, state updates, and rendering

---

## 🎮 Controls

| Player | Keys         |
|--------|--------------|
| Left   | `W` / `S`    |
| Right  | `↑` / `↓`    |

---

## 📐 Mechanics

- Ball movement determined by `x_vel` and `y_vel`
- Paddle collision affects bounce angle based on impact location
- Scoring system increments based on out-of-bounds events
- Game resets after a player reaches 5 points

---

## 🧰 Requirements

- Python 3.x
- `pygame` library

Install dependencies with:

```bash
pip install pygame
