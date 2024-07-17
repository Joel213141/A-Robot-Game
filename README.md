# A-Robot-Game

## Overview

A game developed in C# where the player's objective is to survive as long as possible against incoming robots. The player can shoot robots, avoid collisions, and must aim to endure for the longest duration possible.

## Project Structure and Classes

### Player Class (Player.cs)

- **Properties:** X and Y coordinates, Width, Height.
- **Initialization:** Loads the player's bitmap from "Player.png" and positions it at the center of the game window.
- **Methods:** Includes a Draw method to render the player on screen.

### Robot Class (Robot.cs)

- **Properties:** X and Y coordinates, size.
- **Methods:** Includes methods for drawing the robot on screen and updating its position based on velocity towards the player.

### RobotDodge Class (RobotDodge.cs)

- **Purpose:** Acts as the main game manager class.
- **Responsibilities:**
  - Manages the game loop, player input, robot movements, and collision detection.
  - Utilizes a List<Robot> to handle multiple robot instances.
  - Implements methods like HandleInput for player movement, Draw for rendering game elements, and Update for game logic such as robot movement and collision checks.
  - Implements respawn logic for robots when they collide with the player or move off-screen.

## Development Iterations

1. **Initialization:** Setting up basic player functionality and rendering.
2. **Enhancements:** Adding player movement and basic robot behaviors.
3. **Refinements:** Implementing collision detection and respawn mechanics.
4. **Current Focus:** Managing multiple robots using List<Robot>, allowing dynamic gameplay with continuous robot spawning and movement.

## Next Steps

- Refine Update method in RobotDodge.cs to handle multiple robots effectively.
- Enhance gameplay dynamics with robust collision handling and seamless robot respawning.
