# SO_LONG
So_long is a 42 game project that uses the school’s graphic library (mlx). A file should be sent as an argument to the program containing all the data to generate the map of the game. The player must gather all the collectibles in order to escape and finish the level.

![Screenshot from 2025-05-14 13-54-57](https://github.com/user-attachments/assets/c78c419b-2ac4-41f8-b5a4-139fa7b5067b)

## Key components
### Game Initialization
  To initialize the game, a file ending in ".ber" is given as an argument to the program.
  ```console
  So_long: ./so_long maps/map.ber
  ```

  The given file will be parsed and the game’s data structure will be initialized if valid. The file must have a rectangular map drawn as text using 1’s to define game walls, 0's for the walkable areas, a single P for the player spawning point, an E for an exit and C’s for the collectibles (all must be accessible by the beginning and end point of the game).

### Game Loop
  Everything is happening inside a game loop, limited by a frame rate, where the position of the player is updated, the collisions are checked, the collectibles tracked and the final image displayed. The player movement is handled with the use of events to tell the loop if a key has been pressed at any time during the program’s execution.

  C, Custom libraries use, Events handling, Sprites creation, Buffering, Low level graphics programming
  
  [Gameplay](https://github.com/user-attachments/assets/d1780199-0896-4b82-9729-54f3d9ecf9e1)
