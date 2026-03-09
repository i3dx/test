# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a simple HTML5 Ping Pong game project. A complete browser-based game with single HTML file containing HTML, CSS, and JavaScript.

## Project Structure

```
.
├── CLAUDE.md       # This file - guidance for Claude Code
├── index.html      # Main game file (HTML + CSS + JavaScript)
```

## How to Run

Simply open `index.html` in any modern web browser:

```bash
# On macOS
open index.html

# On Linux
xdg-open index.html

# On Windows
start index.html
```

Or use a simple HTTP server for development:

```bash
# Python 3
python -m http.server 8000

# Node.js (if http-server is installed)
npx http-server -p 8000
```

Then visit `http://localhost:8000`

## Game Controls

- **Arrow Up / W**: Move paddle up
- **Arrow Down / S**: Move paddle down
- **Space**: Start / Restart game

## Architecture

The game is contained in a single HTML file with three sections:

1. **HTML**: Canvas element and UI layout
2. **CSS**: Dark gradient theme with neon glow effects
3. **JavaScript**: Game logic including:
   - Player paddle control via keyboard
   - Simple AI for computer paddle
   - Ball physics with collision detection
   - Score tracking (first to 10 wins)
   - Game loop at 60 FPS

## Key Code Sections

- `player`: Controls for the user paddle
- `computer`: AI-controlled opponent paddle
- `ball`: Ball physics and collision logic
- `gameStep()`: Main game loop
- `updateBall()`: Ball movement and collision detection
