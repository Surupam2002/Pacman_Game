# Pac-Man Game (Java Swing) + QR Code Generator (Node.js)

This repository contains two small projects.

---

## 1. Pac-Man Game, `Pacman_Game/`

A classic **Pac-Man** arcade game built from scratch in **Java** using **Swing** and **AWT** for graphics.

### Features
- Grid-based **maze** rendered with Java 2D graphics
- **Pac-Man** controlled with the **arrow keys**, with directional animation frames (up, down, left, right)
- **Ghosts** that move around the maze
- **Score** tracking, with an intro screen and death/level logic
- Levels that continue and reset (`initLevel`, `continueLevel`)
- **Background music** using the `javax.sound.sampled` API
- Game loop driven by a Swing `Timer`

### Tech Stack
Java · Swing (`JFrame`, `JPanel`) · AWT (Graphics2D, KeyAdapter) · Java Sound API

### Code Structure
```
Pacman_Game/
├── src/pacman/game/
│   ├── Pacman.java   # Entry point: creates the game window (JFrame)
│   └── Board.java    # Game logic: maze, movement, ghosts, score, rendering, input
├── *.png             # Pac-Man and ghost sprites
└── pacmanMusic.wav   # Background music
```

### How to Run
1. Open the `Pacman_Game` folder in **Eclipse** (or any Java IDE) as an existing project.
2. Run `pacman.game.Pacman` as a Java application.
3. Press a key to start, and use the **arrow keys** to move.

> The image and sound files are loaded from the project folder, so run it with `Pacman_Game/` as the working directory.

---

## 2. QR Code Generator, `QR Code Project/`

A small **Node.js** command-line tool that asks for a URL and turns it into a QR code image.

### How It Works
- Prompts for a URL using **inquirer**
- Generates a QR code PNG with **qr-image** (`qr_img.png`)
- Saves the entered URL to `URL.txt` using Node's `fs` module

### How to Run
```bash
cd "QR Code Project"
npm install
node index.js
```

---

## Author

**Surupam Kumar Pandey** · [GitHub](https://github.com/Surupam2002) · [LinkedIn](https://www.linkedin.com/in/surupam-kumar-pandey-44b293218)
