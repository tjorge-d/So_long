# :video_game: SO_LONG
**So_long** is the first **42** visual project that uses the school’s graphic library (mlx). It is a game where the player must gather all the collectibles in order to escape and finish the level.<br>

![So_long](https://github.com/user-attachments/assets/7f131b9a-1c14-4d12-8396-7bdd7f6b587c)

<br>

## :key: Key components

### Game Initialization

After the compilation, to initialize the game, a file ending in "**.ber**" must be given as an **argument** to the program.<p>

```sh
make && make fclean      # Compiles the program and cleans the objects
./so_long maps/map.ber   # Runs the game
```

The given file will be **parsed** and the game’s **data structure** will be initialized if valid.<br>
A valid file must have a **rectangular** map drawn as text using **1**’s to define game walls, **0**'s for the walkable areas, a single **P** for the player spawning point, an **E** for an exit and **C**’s for the collectibles (all **must** be accessible by the beginning and end point of the game).<br>

```txt
111111111111
111111111111
1P11C01110C1
101110C00001
1C0000001111
111111101111
111111100001
1E000C0010C1
111111111111
```

After a **successful** map parse, the program will replace all the walls (**1**) with different numbers, taking into consideration all the neighbour walls, to use the proper **sprites**, seamlessly connecting them.<br>

### Game Loop
Everything is happening inside a **game loop**, limited by a **frame rate**, where the position of the player is updated, the **collisions** are checked, the collectibles **tracked** and the final image **displayed**.<br>

### Controls
The player movement and the closure of the game are handled with the use of **events** to tell the loop if a **key** has been pressed at any time during the program’s execution.<br><br>
Up    -> **W**<br>
Left  -> **A**<br>
Down  -> **S**<br>
Right -> **D**<br>
Exit -> **ESC**<br><br>

## :books: What did I learn?
Being one of my first projects at **42**, I had the opportunity to better enhance my **C** Low level graphics programming skills and also engage for the first time with **libraries**.<br>
Since **So_long** is a game, I delved also into concepts useful to **game development** (one of my biggest passions), like **game loops**, **events**, **delta time** and **sprite creation**.<br>
