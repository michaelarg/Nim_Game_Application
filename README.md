# Nim Game Application

## Table of Contents
- [About The Project](#about-the-project)
- [Built With](#built-with)
- [Usage](#usage)
- [Contact](#contact)


---

## About The Project

This is a JavaFX-based Nim game application that simulates the classic mathematical game of Nim. The implementation is for a single-pile version of the game and strictly adheres to the misère play convention: the player who takes the last stick loses.

The application utilizes the Model-View-Controller (MVC) design pattern and the Observable pattern (via `javafx.beans.Observable`) to keep the GUI synchronized with the game state. The computer opponent is capable of employing different game-play strategies, which can be switched dynamically via the menu bar.

## Key Features
- **Misère Play Rules:** The object of the game is to force the opponent to take the final stick.  
- **Variable Strategies:** The `ComputerPlayer` can use `CautiousStrategy`, `GreedyStrategy`, or `RandomStrategy`.  
- **JavaFX GUI:** A responsive graphical interface for easy setup, play, and status updates.  
- **Customizable Game:** Players can select the initial pile size and determine who goes first.  
- **Max Move Limit:** Players are limited to removing a maximum of 3 sticks per turn (`Game.MAX_STICKS_PER_TURN`).  

---

## Built With
- **Java** (JDK 17 or newer recommended)  
- **JavaFX** (for the graphical user interface)  
- **JUnit 5** (for unit and integration testing)  

---

## Features - Demo

Below is a step-by-step explanation of the Nim game application screenshots.

### 1. Initial Launch and Rules Dialog
The Nim game application starts by displaying a Help Dialog with the rules of the game.

#### Initial Rules Dialog
- Shows the Help dialog titled *"Nim Game App."*  
- Rules summary:  
  “Play against the computer. Alternate taking turns, removing 1 to 3 sticks per turn. The player who takes the last stick loses.”  
- Notes that the user can set the initial pile size and change the computer’s strategy at any time.  
- User can choose “Yes” or “No” for whether to show this dialog at startup.  

![Initial Rules Dialog](src/1_Nim_Rules.png)

### 2. Choosing Computer Strategy
The application allows strategy selection from the menu bar.

#### Strategy Menu
- Shows the *Strategy* menu.  
- Options:  
  - Cautious (selected with dot)  
  - Greedy  
  - Random  

![Strategy Menu](src/2_Strategy_Menu.png)

### 3. Accessing the Help Menu

#### Help Menu
- Shows the *Help* menu.  
- Options include:  
  - **Help** – reopens the rules dialog  
  - **About** – displays current time and developer info  

![Help Menu](src/3_Help_Menu.png)

### 4. Starting a New Game and Pile Size Selection

#### Pile Size and Player Selection
- Displays the New Game Pane.  
- Includes:  
  - *Initial Pile Size* dropdown (shows 9, 16 & 21 options).  
  - *Who Plays First* radio buttons: Human, Computer, Random.  

![Pile Size Selection](src/4_Pile_Size_Selection.png)

### 5. Taking Turns

#### Taking Turns
- Human Player Pane enabled.  
- Computer Player Pane disabled.  
- Game Info displays:  
  “~~ Game Info ~~ Pile size: 4”.  

![Taking Turns](src/5_Taking_Turns.png)

### 6. Game Over and Winner Announcement

#### Winner Announced
- Game Info displays:  
  “~~ Game Info ~~ Game over! Winner: Human”.  
- Both player panes disabled.  
- Computer Player pane shows its last taken sticks.  

![Winner Announced](src/6_Winner_Announced.png)

---

## Contact

**Michael Arg**  
📧 Email: **michgw7@gmail.com**  
🔗 Project Link: https://github.com/michaelarg/nim_game_application_project.git  

---

