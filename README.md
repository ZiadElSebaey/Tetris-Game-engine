# Tetris Game Engine

A fully-featured, multi-mode Tetris game built with JavaFX — developed as an individual university project with a focus on clean architecture, thorough testing, and creative design.

## Features

- **4 Game Modes** — Free Play, UpsideDown, 1984 (Retro Soviet), and Levels
- **Modern Tetris Mechanics** — Hold piece, hard drop, ghost piece preview, 3-piece queue
- **Audio System** — Background music with full sound effects, togglable in-game
- **Level System** — 5 unique levels with specific objectives and unlock progression
- **Leaderboard & High Scores** — Persistent across sessions
- **Alexey's Dialogue** — Animated mid-game dialogue system honouring Tetris creator Alexey Pajitnov
- **159 Passing JUnit 5 Tests** — Covering game logic, brick system, UI utilities, and audio
- **11 Utility Classes** — Refactored architecture eliminating code duplication
- **Full Javadoc** — Complete API documentation for all classes

## Game Modes

| Mode | Description |
|------|-------------|
| Free Play | Standard Tetris gameplay |
| UpsideDown | Board rotates 180°, pieces fall upward |
| 1984 | Retro Soviet aesthetic recreating Alexey Pajitnov's original 1984 version |
| Levels | 5 levels with unique objectives and unlock progression |

## Controls

| Key | Action |
|-----|--------|
| ↑ / W | Rotate piece |
| ← / A | Move left |
| → / D | Move right |
| ↓ / S | Soft drop |
| SPACE | Hard drop |
| H | Hold piece |
| P | Pause / Resume |
| M | Toggle music |

## Tech Stack

- **Language:** Java 23
- **UI Framework:** JavaFX 21.0.6 (controls, FXML, media)
- **Build Tool:** Maven
- **Testing:** JUnit 5 (159 tests)
- **Documentation:** Maven Javadoc Plugin

## Getting Started

### Prerequisites

- JDK 23 or higher
- IntelliJ IDEA (recommended) or any Maven-compatible IDE
- Maven (included via Maven Wrapper — no separate install needed)

### Run the project

```bash
git clone https://github.com/ZiadElSebaey/Tetris-Game-engine.git
cd Tetris-Game-engine
mvn clean javafx:run
```

Or open in IntelliJ IDEA — Maven will automatically download all dependencies. Run `Main.java` directly.

## Project Structure

```
src/
├── main/
│   ├── java/com/comp2042/
│   │   ├── Main.java
│   │   ├── bricks/       # Brick generation, rotation, hold, queue
│   │   ├── logic/        # Game logic, scoring, level management
│   │   └── ui/           # Controllers and utility classes
│   └── resources/
│       ├── *.fxml        # Scene layouts
│       ├── *.css         # Stylesheets
│       ├── *.png         # Images and assets
│       └── sfx/          # Sound effects and music
└── test/
    └── java/com/comp2042/
        ├── bricks/       # Brick system tests
        ├── logic/        # Game logic tests
        └── ui/           # UI utility tests
```

## Test Coverage

**159 tests — all passing**

| Category | Tests |
|----------|-------|
| Core Game Logic | 60 |
| Brick System | 25 |
| UI Utilities | 29 |
| Managers (Settings, Leaderboard, Audio) | 35 |
| Other | 10 |

### Run tests

```bash
mvn test
```

## Acknowledgements

- **Alexey Pajitnov** — Creator of Tetris, inspiration for the Russian theme and 1984 game mode
- JavaFX, OpenJFX, JUnit 5, and Maven communities
