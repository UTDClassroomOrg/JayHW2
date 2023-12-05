# Welcome to the JayShingariHW2 wiki!
# DCD Diagram
![DCDiagram (1)](https://github.com/UTDClassroomOrg/JayShingariHW2/assets/44877523/a9b90557-cc5a-4a2d-8afa-18ca1eda757e)
# DS Diagram Step 5 
![DSDiagram-Step5 (1)](https://github.com/UTDClassroomOrg/JayShingariHW2/assets/44877523/5dbd2e9a-c02a-4e92-9c2a-b5d41f8a8a13)
# Part D
Person Class
1. Initialization (Person() constructor):
- Initializes images array with `GreenfootImage objects.
- Sets the initial image for the Person.
2. Action (act() method):
- Applies gravity by adjusting the Person's vertical position.
- Checks if the space key is pressed and if the `Person` is not already jumping, then calls
jump().
- Calls animate() to cycle through images for animation.
3. Gravity (applyGravity() method):
- Adjusts the Person's vertical position based on velocity.
- Checks if the Person has landed (reached a certain Y position) and resets the jumping status
and velocity if so.
4. Jumping (jump() method):
- Sets the velocity to a negative value to simulate upward motion.
- Sets isJumping to true indicating that the Person is in the process of jumping.
5. Animation (animate() method):
- Cycles through the images array to create an animation effect.
Obstacle Class
1. Action (act() method):
- Moves the Obstacle at a specified speed.
- Resets the Obstacle position when it reaches the edge of the world.
- Checks for collision with Person and stops the game if a collision occurs.
In the Greenfoot game environment, the Person and Obstacle classes interact through a series
of background processes driven by the main game loop. The Person class, upon initialization,
sets up an array of images for animation and continuously checks for user input (like the space
bar for jumping) in its act() method. It simulates gravity by adjusting vertical velocity and
position, and employs an animation cycle to visually represent movement and jumping.
Conversely, the Obstacle class moves across the screen at a set speed, resetting its position
upon reaching the world's edge and continuously checking for collisions with the Person. If a
collision is detected, it halts the game. These interactions are orchestrated by Greenfoot's game
loop, which repetitively calls the act() method of both classes, ensuring smooth animation,
responsive controls, and the dynamic handling of game logic like collision detection and
movement, creating an engaging and interactive game experience.
# Part E

Within the interactive Greenfoot game, the Person class is driven by user inputs and
systematic updates. The spacebar press triggers the jump() method, initiating an animated jump
that modifies the character's vertical position. This jump, coupled with an animation sequence
represented by frame changes, provides real-time visual feedback to the player. The automated
game loop calls to the act() method manage these actions and maintain the physics of gravity,
central to the gameplay experience.
In contrast, the Obstacle class operates autonomously, propelled by the game loop to traverse
the screen. It continuously moves until reaching the screen's edge, where it resets its position.
The Obstacle class also listens for collisions with the Person, which, upon occurrence, prompts
an immediate game halt through Greenfoot.stop(). This represents a critical gameplay moment,
marking the player's failure to navigate the obstacle and resulting in a game-over state. The
expected outputs from both classes— Person's motion and Obstacle's movement and collision
response—create a dynamic and challenging environment that tests player agility and
strategizing, encapsulating the game's core mechanics and engagement loop.
