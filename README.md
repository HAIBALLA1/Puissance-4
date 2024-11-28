# Connect Four

## Description

This project implements the classic **Connect Four** game in the C programming language. The game offers two modes:
- Play against an **AI (Artificial Intelligence)**.
- Play a **two-player duel**.

The objective is to align four tokens of the same color (horizontally, vertically, or diagonally) on a 6-row by 7-column grid.

## Features

### Game Modes
1. **Against AI:**
   - The AI uses the Minimax algorithm to evaluate the board and maximize its chances of winning.
2. **Two Players:**
   - Two players can alternate turns on the same terminal.

### Display
- A visual representation of the game board with colored tokens:
  - **Blue** ([34m•[0m) for the first player.
  - **Red** ([31m•[0m) for the second player or the AI.

### Validations
- Checks for alignments to detect wins or draws.
- Detects full columns.

### AI
- The **Minimax** algorithm explores the tree of possible moves to find the best one up to a given depth.
- The AI evaluates board positions to maximize its winning chances or minimize the opponent's.

## Prerequisites

### Compilation
- A C-compatible compiler (e.g., GCC).
- Standard C libraries (stdio.h, stdlib.h, limits.h, time.h).

## Installation

1. Clone this repository to your machine:
   ```bash
   git clone <repository_url>
   cd <project_folder>
   ```
2. Compile the main file using a C compiler:
   ```bash
   gcc -o connect4 main.c
   ```
3. Run the game:
   ```bash
   ./connect4
   ```

## Usage

1. Choose a game mode:
   - Press **1** to play against the AI.
   - Press **2** for a two-player duel.
2. On your turn, select a column to play (from 1 to 7).
3. Enjoy the game!

## Code Structure

### Key Functions
- `new_noeud`: Creates a new node for the Minimax tree.
- `tableau`: Initializes the game grid.
- `afficher_tab`: Displays the current state of the grid with colors.
- `minimax`: Implements the algorithm to determine the best moves for the AI.
- `lancer_jeux_entre_IA`: Manages the gameplay against the AI.
- `lancer_le_jeux_entre_deux_joueurs`: Manages the two-player duel.
- `test_horizontal`, `test_vertical`, `test_oblique`, `test_anti_oblique`: Check for winning alignments.

## Future Improvements

- **Add a graphical menu** for an enhanced user experience.
- **Configure AI depth** to adjust difficulty.
- **Save and load games** for continuity.

## Author
This project was developed by El Varougou Haiballa.

## License
This project is licensed under the MIT License. You are free to modify and redistribute it under the terms of this license.

