# Abyss Wolf — A JavaScript Action Game

<p align="center">
  <img src="https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/HTML5-Canvas-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5 Canvas" />
  <img src="https://img.shields.io/badge/CSS3-Modern-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License" />
</p>

> *"Embrace the darkness, become the legend."*

**Abyss Wolf** is a 2D side-scrolling action platformer built entirely with vanilla JavaScript, modern CSS, and HTML5 Canvas. Battle creatures of doom, navigate corrupted landscapes, unlock special powers, and test your survival instincts before time runs out!

---

## Features

- **Fluid Movement & State Machine**:
  - Implements state-driven animations for sitting, running, jumping, falling, rolling, diving, and taking damage.
- **Dynamic Combat & Varied Enemies**:
  - **Flying Enemies**: Swift aerial adversaries that dive from above.
  - **Climbing Enemies**: Giant spiders descending from tree canopies.
  - **Ground Enemies**: Carnivorous plants and hazards on the floor.
- **Parallax Background**:
  - Multi-layered scrolling background that creates a sense of depth and speed.
- **Particle & Collision Effects**:
  - Dynamic fire particles during special moves and explosive collision animations on impact.
- **HUD & Status Tracking**:
  - Live score counter, 60-second survival timer, remaining lives indicator, and game over summary.
- **Debug Mode**:
  - Toggle visible bounding boxes for collision detection and debugging.
- **Atmospheric UI & Pages**:
  - Lore & landing page (`game.html`), game canvas (`index.html`), leaderboard (`leaderboard.html`), and auth pages (`login.html`, `register.html`).

---

## Controls

| Key | Action |
| :--- | :--- |
| **Arrow Up** ($\uparrow$) | Jump |
| **Arrow Down** ($\downarrow$) | Sit / Dive |
| **Arrow Left** ($\leftarrow$) | Move Left |
| **Arrow Right** ($\rightarrow$) | Move Right |
| **Control** (`Ctrl`) | Roll / Special Fire Attack |
| **D** | Toggle Debug Mode (Hitboxes) |

---

## Project Structure

```text
js game/
├── assests/                    # Game sprites, audio, and visual assets
│   ├── layer-1.png .. layer-5.png  # Parallax background layers
│   ├── player.png              # Player spritesheet
│   ├── enemy_*.png             # Enemy spritesheets
│   ├── boom.png                # Collision explosion animation
│   └── logo.png                # Game banner & branding
├── bg.js                       # Parallax background handler
├── collisionAnimation.js       # Impact explosions & animations
├── enemy.js                    # Enemy classes (Flying, Climbing, Ground)
├── game.html                   # Game overview, lore & landing page
├── index.html                  # Main game canvas entrypoint
├── input.js                    # Keyboard event handler
├── leaderboard.html            # High scores & rankings page
├── login.html                  # User login view
├── main.js                     # Core game loop & initialization
├── particles.js                # Particle systems (fire, dust, splash)
├── player.js                   # Player character controller
├── playerStates.js             # State pattern animation transitions
├── register.html               # User registration view
├── style.css                   # Global styles & canvas positioning
├── UI.js                       # Head-Up Display (Score, Timer, Lives)
├── .gitignore                  # Git ignore rules
└── README.md                   # Project documentation
```

---

## How to Play

Because the game uses **ES6 JavaScript Modules** (`import` / `export`), it must be served through a local HTTP/HTTPS server rather than directly opening the file via `file://`.

### Quick Start Options

#### Option 1: VS Code Live Server
1. Open the project folder in **VS Code**.
2. Right-click [`index.html`](file:///d:/nigga/PROJECTS/Projects/js%20game/index.html) (or `game.html`).
3. Click **"Open with Live Server"**.

#### Option 2: Python HTTP Server
```bash
# In the project directory:
python -m http.server 8000
```
Then visit `http://localhost:8000/index.html` or `http://localhost:8000/game.html`.

#### Option 3: Node / npx
```bash
npx serve .
```

---

## Tech Stack

- **HTML5 Canvas**: Frame-by-frame rendering and sprite animations.
- **Vanilla JavaScript (ES6+)**: Modular code with Object-Oriented Programming (OOP) and State design pattern.
- **CSS3**: Custom dark fantasy styling, responsive layouts, and animations.

---

## Contributing

Contributions and ideas are welcome!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/NewFeature`)
3. Commit your Changes (`git commit -m 'Add NewFeature'`)
4. Push to the Branch (`git push origin feature/NewFeature`)
5. Open a Pull Request

---

## License

This project is open-source and available under the [MIT License](LICENSE).
