# ♟ Excalibur – A Chess Engine

A chess engine which implements:
- The [Minimax algorithm](https://en.wikipedia.org/wiki/Minimax) for optimal movement analysis
- [Alpha-beta pruning](https://en.wikipedia.org/wiki/Alpha%E2%80%93beta_pruning) for move searching
- [Move ordering](https://www.chessprogramming.org/Move_Ordering) based off heuristics like captures and promotions
- Tomasz Michniewski's [Simplified Evaluation Function](https://www.chessprogramming.org/Simplified_Evaluation_Function) for board evaluation and piece-square tables
- A command-line user interface

It uses Python 3.8 with mypy type hints and unit + integration tests.

## Install

`pip install -r requirements.txt`

## Use it via the command-line

Start the engine with:

`python3 chess_board.py`

```bash
Start as [w]hite or [b]lack:
w

  8 ♖ ♘ ♗ ♕ ♔ ♗ ♘ ♖
  7 ♙ ♙ ♙ ♙ ♙ ♙ ♙ ♙
  6 · · · · · · · ·
  5 · · · · · · · ·
  4 · · · · · · · ·
  3 · · · · · · · ·
  2 ♟ ♟ ♟ ♟ ♟ ♟ ♟ ♟
  1 ♜ ♞ ♝ ♛ ♚ ♝ ♞ ♜
    a b c d e f g h

Your move (e.g. b1c3):
```

## Tests

There are unit tests for the engine, UI, and evaluation modules.

`python3 -m unittest discover tests/`

Type checking:

`mypy .`
