
# 🎲 Rummikub Game (C++ Implementation)


This project is a C++ implementation of the classic **Rummikub** game. It demonstrates how to use **Object-Oriented Programming (OOP)** and **dynamic data structures** to implement game logic and tile combinations.

---

# 📖 Overview

The program simulates a simplified version of Rummikub where players draw and play tiles to form valid combinations. It shows how real-world game logic can be modeled using programming concepts such as classes, dynamic arrays, and algorithms.

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

- Object-Oriented Programming (classes and encapsulation)  
- Dynamic arrays for flexible tile storage  
- Algorithms for validating groups and runs  
- Game state management for turns and combinations  

---

# 📸 Game Tiles Example

Here’s an example of Rummikub tiles:

![Rummikub Tiles](https://boardgoats.org/tag/rummikub/)

---

# 🚀 Conclusion

This project demonstrates how a complex game like Rummikub can be implemented using **OOP principles** and **dynamic data structures**. It highlights flexible tile storage, combination validation, and turn-based game logic in a clear and structured way.
