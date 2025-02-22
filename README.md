Game Development Documentation

Group Members (E4): 
Talha Faizan (L1F22BSCS0103)
Hassan Ashraf (L1F22BSCS0086)
Mubashar Tanveer (L1F22BSCS0094)
Game Title:
Space Blitz – Galactic Defender
Overview
This document provides an overview of how we developed our shoot 'em up game, covering the key GameObjects, controls, asset imports, and resource usage. The game is designed to be a fast-paced space shooter where players must defeat waves of enemy ships while avoiding incoming fire. The mechanics involve shooting, movement, and survival elements to create an engaging experience.
________________________________________
GameObjects Used
1. Player Ship
The player ship is the main controllable object in the game. It moves in horizontal and vertical directions, allowing smooth navigation across the screen. The player ship fires projectiles at enemies using predefined shooting points. It has a collider to detect collisions with enemy projectiles and ships. Additionally, the player ship may have a health or life system to handle damage.
2. Enemy Ship
Enemy ships spawn at the top of the screen and move downward toward the player. Some enemies may follow different movement patterns, such as left-right or direct tracking. Enemy ships fire projectiles at the player at timed intervals, making dodging and positioning important gameplay elements. When destroyed, enemies contribute to the player's score.
3. Shooting Points
Shooting points define the positions from which projectiles are spawned. The player and enemies both have designated shooting points to ensure accurate and balanced attack mechanics. These points are child objects of the main ship GameObjects and can be adjusted dynamically to create different weapon effects, such as laser beams.
4. Projectiles (Lasers)
Player lasers are prefabs for projectiles fired by the player. They travel upward and damage enemies upon collision. Enemy lasers are similar but travel downward, targeting the player. Both projectile types use physics components for movement and collision detection. Special effects, such explosion animations, enhance the visual appeal.
5. Score System
The score system tracks the player's progress by awarding points for each enemy destroyed. The UI updates dynamically to reflect the score in real time. A high-score tracking system may be implemented to store and compare top scores across multiple play sessions.

6. Player Respawn Feature
The respawn feature handles player death and reset mechanics. When hit, the player lose and respawns at a predefined position.
7. UI Elements (Canvas, Text, and Buttons)
The Canvas holds all UI elements, including the game menu and HUD. Buttons allow players to start the game, quit, or view instructions. The UI text displays the player's score,and game instructions.
8. Background Panel
The background panel is used for dynamic scrolling backgrounds. It creates a seamless space environment that gives the illusion of movement. Parallax effects may be applied to make the background more immersive.
9. Level Manager
The Level Manager is responsible for managing different levels or waves in the game. It controls enemy spawn patterns, wave progression, and difficulty scaling. This ensures a structured gameplay experience with increasing challenges.
10. Main Camera
The Main Camera is positioned at the top and follows a fixed or slight dynamic movement to enhance gameplay immersion. It may include visual effects like screen shake for impacts or smooth transitions between game states.


11. Background Music:
Added background music for more aesthetic feel. Player will feel immerse in this action game by listening to the enchanting music and sound effects;
________________________________________
Instructions for Controls
•	Move Left/Right: Arrow Keys or A/D to move left or right.
•	Move Up/Down: Use W/S to adjust the vertical position.
•	Shoot: Press the Spacebar to fire lasers.
•	Pause Game: Press the Escape OR P Key to pause the game.
•	Quit Game: Pressing Q will take you back to Main Menu.
•	Navigate Menus: Use the mouse to select menu options.
________________________________________
Importing Assets from Unity Asset Store
To import assets, open the Unity Asset Store from the Unity Editor. Search for the required assets, such as space-themed ships, UI elements, and background music. After selecting an asset, click Download and Import to bring it into the Unity project. Once imported, assign the assets to their respective GameObjects. Ensure that prefabs are properly configured with necessary components like colliders, rigidbodies, and animations before integrating them into the game.
________________________________________


Use of GameObjects and Resources
Prefabs are used for the player ship, enemy ships, and projectiles to ensure easy reusability and consistency. Physics components like Rigidbody2D and Collider2D are implemented for movement and collision detection. The GameManager script manages core gameplay logic, including score updates, wave spawning, and respawn mechanics. Additionally, Audio Sources are incorporated for background music and sound effects such as shooting, explosions, and UI interactions. Efficient memory usage and object pooling techniques help optimize performance by reusing instantiated objects instead of constantly creating and destroying them.
________________________________________
Conclusion
This documentation provides a structured approach to developing a shoot 'em up game. Each element is designed to ensure smooth gameplay, efficient resource management, and modular development. The implementation of prefabs, UI, and game mechanics contributes to a scalable and maintainable game structure.
________________________________________

