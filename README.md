🎮 Tic-Tac-Toe Console Game in Java

Tic-Tac-Toe is a classic two-player game that can now be played right from your console!  
This simple yet fun Java program lets two players take turns placing their marks (**X** or **O**) on a 3x3 grid. The goal is to get **three of your marks in a row** — horizontally, vertically, or diagonally.

---

## 🧩 Game Overview

The game board is represented as a **3x3 grid** with slots numbered **1 to 9**, allowing players to easily pick their desired position by entering the corresponding number.

### 🎲 Board Layout
![Screenshot of code](https://github.com/Charantejatheju/Tik-tac-toe-game/blob/main/board%20input.png)

---


## 🕹️ How to Play

1. Two players choose either **X** or **O**.
2. The player with **X** always goes first.
3. Each player takes turns entering the **slot number** where they want to place their mark.
4. The board updates automatically after every move.
5. The first player to align **three marks** in a **row**, **column**, or **diagonal** wins.
6. If all slots are filled without a winner, the game ends in a **draw**.

---

## 💻 Sample Gameplay

![Screenshot of code](https://github.com/Charantejatheju/Tik-tac-toe-game/blob/main/sample%20game.png)


The game continues until a player wins or all cells are filled.

---

## 🧠 Key Concepts

### 🧱 Arrays

Arrays are used to represent the game board.  
A **1D array of size 9** stores the values **1–9**, representing each cell of the board.

```java
// Creating a board with 9 positions
String[] board = new String[9];

// Filling the board with numbers 1 to 9
for (int a = 0; a < 9; a++) {
    board[a] = String.valueOf(a + 1);
}
```
### 🔄 Conditional Statements
```
Conditionals control the game’s logic — from validating user input to checking for a winner.

✅ Example: Input Validation
if (board[numInput - 1].equals(String.valueOf(numInput))) {
    board[numInput - 1] = turn;
} else {
    System.out.println("Slot already taken; re-enter slot number:");
}

```
This ensures players cannot place their mark on an already occupied slot.

### 🧩 Switch Case: Checking for a Winner
---

The switch statement checks all possible winning combinations (rows, columns, and diagonals).
```
switch (a) {
    case 0:
        line = board[0] + board[1] + board[2];
        break;
    case 1:
        line = board[3] + board[4] + board[5];
        break;
    // Additional cases for columns and diagonals...
}

```
If any combination equals XXX or OOO, a winner is declared.

### 🏁 Game Logic Summary
Step	Description
1	Display the game board (numbers 1–9).
2	Player X starts and enters a slot number.
3	Replace the number with the player’s symbol (X or O).
4	Check for winning conditions after each move.
5	If no one wins and all slots are filled → Draw.

### 🧰 Technologies Used
---
```
Language: Java

Concepts: Arrays, Loops, Conditional Statements, Switch Case, Console Input

Environment: Any Java IDE or command-line compiler (javac, java)
```

### ⚙️ How to Run the Program
---

Clone this repository:
```
git clone https://github.com/yourusername/tic-tac-toe-java.git
```

Navigate to the folder:
```
cd tic-tac-toe-java
```

Compile the Java file:
```
javac TicTacToe.java
```

Run the program:
```
java TicTacToe
```

### 🧑‍💻 Author

Charan Teja Muddukuppam
B.Tech, ECE — Chadalawada Ramanamma Engineering College, Tirupati
✨ Passionate about building intelligent, interactive software solutions.
