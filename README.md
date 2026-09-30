# ♟️ Chess Table 3D

<p align="center">
  <strong>A modern, immersive 3D chess experience built for the web.</strong>
</p>

<p align="center">
  Play chess locally with a fully interactive 3D board, smooth animations,
  dynamic camera controls, and a seamless 3D ↔ 2D visual experience.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-16-black?style=for-the-badge&logo=next.js" />
  <img src="https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react" />
  <img src="https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript" />
  <img src="https://img.shields.io/badge/Three.js-0.182-black?style=for-the-badge&logo=three.js" />
  <img src="https://img.shields.io/badge/chess.js-1.4-8B5CF6?style=for-the-badge" />
</p>

---

## ✨ Overview

**Chess Table 3D** is a browser-based chess game designed to combine the
classic rules of chess with a modern interactive 3D experience.

Instead of treating the chess board as a simple 2D grid, the project
represents the entire board and pieces inside a real-time Three.js scene.

The result is a chess board that feels more like a **virtual chess table**
than a traditional web chess interface.

The project focuses on:

- 🎮 Interactive local 2-player gameplay
- 🧊 Real-time 3D rendering
- 🎥 Free camera controls
- ♟️ Interactive 3D chess pieces
- 🔄 Animated 3D ↔ 2D view transformation
- ✨ Smooth piece and board animations
- 🧠 Complete chess rule validation
- ♿ Keyboard and accessibility support
- 📱 Responsive interface
- ⚡ Client-side gameplay with no backend required

---

## 🎮 Features

### ♟️ Complete Chess Gameplay

Powered by [`chess.js`](https://github.com/jhlywa/chess.js), the game handles
the core rules of chess including:

- Legal move validation
- Check
- Checkmate
- Stalemate
- Castling
- En passant
- Pawn promotion
- Draw detection
- Turn management

The UI is responsible for presentation and interaction while
`chess.js` handles the underlying chess rules.

---

### 🧊 Interactive 3D Chess Board

The default experience uses a real-time Three.js scene.

Players can interact with the board using:

- Orbit camera controls
- Perspective camera
- Smooth camera movement
- Interactive board squares
- 3D chess pieces
- Lighting and shadows

The board is rendered using:

- Three.js
- React Three Fiber
- React Three Drei

---

### 🔄 3D ↔ 2D Transformation

One of the main visual features of the project is the ability to transform
the same Three.js chess table between 3D and 2D-like views.

Instead of replacing the 3D board with a completely different HTML board,
the existing scene transitions visually.

### 3D Mode

```text
             Camera
                ↘
                 ↘

          ♜      ♞      ♝
       ┌─────────────────────┐
      /                     /│
     /       CHESS BOARD    / │
    └─────────────────────┘  │
     └───────────────────────┘
