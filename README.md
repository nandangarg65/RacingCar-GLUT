
# 🚗 Rage on the Road: An OpenGL Car Racing Game

**Rage on the Road** is a 2D car racing game developed in **C++ using OpenGL**. It features a dynamic and interactive road race environment with real-time animations, score tracking, and difficulty scaling. Designed as a beginner-friendly graphics project, this game demonstrates core concepts in computer graphics and game development using OpenGL and GLUT.

---

## 📌 Table of Contents

- [🎯 Objective](#-objective)
- [✨ Key Features](#-key-features)
- [💻 System Requirements](#-system-requirements)
- [🔧 How to Run](#-how-to-run)
- [🧩 Implementation](#-implementation)
- [📸 Screenshots](#-screenshots)
- [📚 Learnings](#-learnings)
- [📄 License](#-license)

---

## 🎯 Objective

- Build a basic 2D car racing game using OpenGL in C++.
- Understand graphics rendering and input handling using the GLUT toolkit.
- Simulate real-time animation and dynamic gameplay.
- Provide a foundation for future enhancements in game development and computer graphics.

---

## ✨ Key Features

- 🔼 Smooth player car movement with arrow keys.
- 🕹️ Keyboard controls:
  - `← / →`: Move car left or right
  - `↑ / ↓`: Adjust game speed (FPS)
  - `SPACE`: Start/restart game
  - `ESC`: Quit game
- 🛣️ Moving road dividers simulate car movement.
- 🚗 Incoming enemy cars from the top.
- 🧠 Collision logic and game-over triggers.
- 🧮 Score counter and level-based speed adjustment.
- ⏱️ Timer-controlled frame updates using `glutTimerFunc`.

---

## 💻 System Requirements

### Software:
- C++ Compiler (GCC, g++)
- OpenGL Utility Toolkit (GLUT)
- OpenGL and GLU Libraries

### Platforms:
- Windows / Linux (Tested)
- Any OS that supports OpenGL and GLUT

---

## 🧩 Implementation
The game logic is implemented using a combination of OpenGL/GLUT functions and custom user-defined functions to handle rendering, input, and game logic.

### 🔧 Core OpenGL & GLUT Functions Used
-glClear() – Clears the screen buffer before rendering new frames.
-glColor3f() – Sets the color for drawing elements.
-glBegin() / glEnd() – Used for drawing shapes (cars, dividers, road).
-glVertex2f() – Specifies the coordinates for vertices of shapes.
-glFlush() – Ensures all OpenGL commands are executed.
-glutSwapBuffers() – Used for double buffering to display the rendered frame.
-glutKeyboardFunc() – Handles standard key inputs.
-glutSpecialFunc() – Handles special keys like arrow keys.
-glutTimerFunc() – Sets a timer to call the game loop for continuous updating.
-glOrtho() – Sets up a 2D orthographic viewing region for rendering.
-glutMainLoop() – Starts the GLUT event-processing loop.
-glutInit() – Initializes the GLUT library.
-glutInitDisplayMode() – Sets the initial display mode (e.g., RGB and double buffer).
-glutInitWindowSize() – Specifies the initial width and height of the window.
-glutInitWindowPosition() – Sets the window’s initial position on the screen.
-glutCreateWindow() – Creates a window with the specified title.
glutDisplayFunc() – Registers the display callback for rendering frames.
-glutPostRedisplay() – Marks the current window as needing to be redrawn.
-glClearColor() – Sets the background color of the display window.
-exit() – Terminates the program.

### 🧠 User-Defined Functions
-display() – Clears the screen and displays either the welcome screen or the main game screen.
-spe_key() – Handles arrow key inputs for controlling the player’s car and speed.
-processKeys() – Handles standard key inputs like Space and Esc.
-timer() – Controls frame updates and animation timing using a timer callback.
-fristDesign() – Displays the welcome screen with title and instructions.
-startGame() – Main game loop that handles all rendering and updates.
-drawRoad() – Draws the background road and borders.
-drawDivider() – Animates dashed lines in the center of the road.
-drawCar() – Renders the player’s car.
-drawOtherCars() – Renders enemy cars and handles their motion.
-collided() – Detects collisions between the player’s car and enemy cars.
-updateScoreAndLevel() – Increments the score and increases game difficulty over time.
-gameOver() – Displays the game over screen and final score.
-drawText() – Renders text at specific screen positions.

---
