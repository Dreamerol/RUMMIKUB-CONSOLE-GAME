<div align="center">

# 🎲 RUMMIKUB CONSOLE GAME - C++

<img src="https://github.com/Dreamerol/Dreamerol/blob/cd7c3a8443730e5af56d1ae642a461862dd61bb0/ZRUMMICUB.jpg" alt="Rummikub" style="width:100%; height:auto; margin-bottom: 20px;">

---

</div>


<img src="https://img.shields.io/badge/Dev%20Environment-Visual%20Studio-blue?style=for-the-badge" alt="Visual Studio" height="40">
<img src="https://img.shields.io/badge/Language-C++-yellow?style=for-the-badge" alt="C++" height="40">
<img src="https://img.shields.io/badge/Paradigms-Procedural%20&amp;%20Modular-orange?style=for-the-badge" alt="Paradigms" height="40">

</div>

---

# 📖 Overview

This project brings the classic **Rummikub** game to life using C++, turning the tabletop experience into a console-based digital simulation.

Imagine sitting at a table with friends: each player draws tiles, tries to form sequences or sets, and carefully plans their moves. In this project, the computer takes the role of both dealer and referee, handling the game logic, tile distribution, and validation automatically.

I designed the program to be modular and **object-oriented**, using **classes** to represent players, tiles, and the game board. Dynamic data structures allow the program to manage each player’s hand and the pool of remaining tiles efficiently. Algorithms check for valid sets and sequences, ensuring that the rules of Rummikub are respected every turn.

Through this project, I learned how to model **real-world game mechanics** in code, simulate player interactions, and implement **dynamic logic** that adapts to the current state of the game. It’s more than just a game—it’s a hands-on exploration of **OOP**, **dynamic arrays**, and **algorithmic problem-solving**, showing how programming can capture the complexity and fun of classic board games.

---

# ⚙️ How to Run

First, compile the program using a C++ compiler, and then run the executable. The game will start in the terminal, allowing players to draw tiles, form combinations, and take turns until someone wins.

---

# 🧱 Object-Oriented Design

The project is structured using multiple classes, each responsible for a specific part of the game.

**Tile Class:** Represents a single tile with a number (1–13), a color (red, blue, yellow, black), and a joker flag. It encapsulates all data related to a tile and provides methods to access or display it.

**Deck Class:** Represents the full set of tiles. It generates all tiles, stores them in a dynamic array, shuffles them, and provides tiles to players as they draw.

**Player Class:** Represents each player, storing their tiles in a dynamic array (hand). It handles adding and removing tiles during gameplay and displays the current hand.

**Game Class:** Controls the game flow, initializes the deck and players, manages turns, validates tile combinations, and checks win conditions.

---

# 📦 Dynamic Arrays

Dynamic arrays are essential for handling collections of tiles because the number of tiles constantly changes as players draw and play. They allow flexible storage for:

- Player hands that grow and shrink  
- The deck that shrinks as tiles are drawn  
- Combinations that vary in size  

---

# 🧠 Tile Combinations

The core of Rummikub gameplay is forming valid combinations:

- **Groups:** Tiles with the same number but different colors. For example, a red 7, blue 7, and black 7.  
- **Runs:** Tiles with consecutive numbers of the same color. For example, a red 3, red 4, and red 5.  

The program validates combinations by storing selected tiles in a dynamic array, checking for the required pattern, and rejecting invalid moves.

---

# 🔄 Game Mechanics

### Turn Flow

Players take turns selecting tiles from their hand. Selected tiles are temporarily stored, validated, and then placed on the table if they form a valid combination. Invalid moves are rejected.

### Drawing Tiles

If a player cannot make a valid move, they draw a tile from the deck to continue playing.

### Joker Handling

Jokers can substitute any tile and are flexible within combinations. They can be replaced later with the correct tile.

---

# 🏆 Win Condition

The first player to empty their hand wins the game. Other players receive penalty points equal to the value of the remaining tiles in their hands.

---

# 💡 Key Concepts Demonstrated

- Object-Oriented Programming (**classes** and **encapsulation**)  
- Dynamic arrays for flexible tile storage  
- Algorithms for validating groups and runs  
- Game state management for turns and combinations  

---

# 🚀 Conclusion

This project demonstrates how a complex game like Rummikub can be implemented using **OOP principles** and **dynamic data structures**. It highlights flexible tile storage, combination validation, and turn-based game logic in a clear and structured way.
