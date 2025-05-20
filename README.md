# SO_LONG
**So_long** is the first **42** visual project that uses the school’s graphic library (mlx). It is a game where the player must gather all the collectibles in order to escape and finish the level.<br>

![Screenshot from 2025-05-14 13-54-57](https://github.com/user-attachments/assets/c78c419b-2ac4-41f8-b5a4-139fa7b5067b)

## Key components
### Game Initialization
To initialize the game, a file ending in "**.ber**" must be given as an **argument** to the program.<p>
The given file will be **parsed** and the game’s **data structure** will be initialized if valid.<br>
A valid file must have a **rectangular** map drawn as text using **1**’s to define game walls, **0**'s for the walkable areas, a single **P** for the player spawning point, an **E** for an exit and **C**’s for the collectibles (all **must** be accessible by the beginning and end point of the game).<br>

### Game Loop
Everything is happening inside a **game loop**, limited by a **frame rate**, where the position of the player is updated, the **collisions** are checked, the collectibles **tracked** and the final image **displayed**.<br>
The player movement is handled with the use of **events** to tell the loop if a **key** has been pressed at any time during the program’s execution.<br>

## What did I learn?
Being one of the first projects from **42**, I had the opportunity to better enhance my **C** Low level graphics programming skills and also engage for the first time with **libraries**.<br>
Since **So_long** is a game, I also delved into concepts useful to **game development** (one of my biggest passions), like **game loops**, **events**, **delta time** and **sprites creation**.<br>
