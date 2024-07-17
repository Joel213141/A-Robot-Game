# A-Robot-Game
A game where the player's aim is to survive as long as possible, it can shoot the incoming robots, it can avoid them and the aim is to last as long as possible. Utilizing C# for gameplay mechanics, AI behavior, and overall game logic.

The game involves creating classes like Player, Robot, and managing them through a central class called RobotDodge. Here's a breakdown of your tasks and the steps you've outlined:

Player Class (Player.cs):
You've defined a Player class with properties for X, Y coordinates, Width, and Height.
Initialized the Player's bitmap from a provided image file ("Player.png").
Implemented a constructor to position the Player in the center of the game window and a Draw method to render the Player on screen.

Robot Class (Robot.cs):
Created a Robot class with properties for X, Y coordinates, and size.
Implemented methods to draw the Robot on screen and update its position based on its velocity towards the Player.

RobotDodge Class (RobotDodge.cs):
This serves as the main game manager class.
Manages the game loop, handling player input, updating robot positions, and checking collisions.
Implemented methods like HandleInput to manage player movement, Draw to render game elements, and Update to handle game logic like robot movement and collision detection.
Utilized a List<Robot> to manage multiple robots in the game, with functionality to respawn robots when they collide with the player or move off-screen.

Game Development Iterations:
Started with a basic player setup and gradually added features like player movement, robot spawning, and collision detection.
Each iteration built upon the previous one, ensuring functionality was tested and working before moving on.

Next Steps (Iteration 4):
Now looking to manage multiple Robot objects using a List<Robot>, allowing for more dynamic gameplay with multiple robots spawning and moving towards the player.
This involves updating the Update method in RobotDodge.cs to handle multiple robots, spawning new robots off-screen, and removing robots that collide with the player or move off-screen.
