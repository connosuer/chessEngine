# Chess AI with Minimax Algorithm

This project implements a simple chess AI using the Minimax algorithm with Alpha-Beta pruning. The AI plays against a random move generator, demonstrating basic chess strategy and decision-making.

## Features

- Chess board representation using the `python-chess` library
- Minimax algorithm with Alpha-Beta pruning for move selection
- Simple board evaluation function
- Game simulation between the AI (playing as White) and random moves (playing as Black)

## Requirements

- Python 3.6+
- python-chess library

## Installation

1. Ensure you have Python 3.6 or newer installed on your system.
2. Install the required library using pip:

```
pip install python-chess
```

## Usage

To run the chess game simulation:

1. Save the provided code in a file, e.g., `chess_ai.py`.
2. Run the script using Python:

```
python chess_ai.py
```

The program will start a game where the AI (White) plays against random moves (Black). Each move and the resulting board state will be printed to the console.

## How It Works

1. **Board Evaluation**: The `evaluate_board` function assigns a score to the current board state based on material balance and a simple measure of piece mobility.

2. **Minimax Algorithm**: The `minimax` function implements the Minimax algorithm with Alpha-Beta pruning to search for the best move.

3. **Move Selection**: The `get_best_move` function uses Minimax to evaluate possible moves and select the best one for the AI.

4. **Game Simulation**: The `play_game` function sets up a game where the AI plays as White against random Black moves.

## Customization

- Adjust the depth of the Minimax search in the `play_game` function to change the AI's look-ahead capability.
- Modify the `piece_values` dictionary or `evaluate_board` function to refine the AI's position evaluation.

## Limitations

- The current implementation uses a simple evaluation function and may not consider advanced chess concepts.
- The AI's strength is limited by the search depth, which is set to 3 in the current implementation.


## License

This project is open-source and available under the MIT License.
