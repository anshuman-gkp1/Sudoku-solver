# 🔢 Sudoku Solver

A **Python-based Sudoku solver** that uses a **backtracking algorithm** to solve any valid 9×9 Sudoku puzzle. Solves puzzles in milliseconds by recursively trying digits and backtracking on conflicts.

## 🧠 How It Works

The solver uses the classic **backtracking** approach:

1. **Find** the next empty cell (represented as `-1`)
2. **Try** digits 1–9 in that cell
3. **Validate** the digit against row, column, and 3×3 box constraints
4. **Recurse** — if valid, place the digit and move to the next empty cell
5. **Backtrack** — if no digit works, reset the cell and try the previous one
6. **Solved** when no empty cells remain

## ✨ Features

- ✅ Solves any valid 9×9 Sudoku puzzle
- ⚡ Fast backtracking algorithm
- 🖨️ Formatted console output with visual row grouping
- 🔍 Validates rows, columns, and 3×3 sub-grids

## 🛠️ Tech Stack

| Technology | Details |
|------------|---------|
| Language | Python 3 |
| Algorithm | Recursive Backtracking |
| Dependencies | None (standard library only) |

## 🚀 How to Run

### Prerequisites
- Python 3.x installed

```bash
git clone https://github.com/anshuman-gkp1/Sudoku-solver.git
cd Sudoku-solver
python sudoku.py
```

## 📋 Example

**Input puzzle** (`-1` = empty cell):
```python
[5, 3, -1,  -1, 7, -1,  -1, -1, -1]
[6, -1, -1,   1, 9,  5,  -1, -1, -1]
...
```

**Output** (solved):
```
[5, 3, 4, 6, 7, 8, 9, 1, 2]
[6, 7, 2, 1, 9, 5, 3, 4, 8]
[1, 9, 8, 3, 4, 2, 5, 6, 7]

[8, 5, 9, 7, 6, 1, 4, 2, 3]
[4, 2, 6, 8, 5, 3, 7, 9, 1]
[7, 1, 3, 9, 2, 4, 8, 5, 6]

[9, 6, 1, 5, 3, 7, 2, 8, 4]
[2, 8, 7, 4, 1, 9, 6, 3, 5]
[3, 4, 5, 2, 8, 6, 1, 7, 9]
```

## 📁 Project Structure

```
Sudoku-solver/
└── sudoku.py    # Complete solver with backtracking algorithm
```

## 🔮 Future Improvements

- Add a GUI using Tkinter or Pygame
- Accept puzzle input from the user at runtime
- Add puzzle generator for random boards
- Visualize the backtracking process step-by-step
