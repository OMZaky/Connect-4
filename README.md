# Connect-4 AI

## Overview
This repository contains a Python-based implementation of the classic game Connect-4, featuring a custom-built Artificial Intelligence opponent. The AI is powered by the Minimax algorithm, allowing it to evaluate complex mid-game board states and calculate the optimal next move by anticipating future turns.

## Features
* **Intelligent AI Opponent:** Plays strategically against the user or evaluates specific board states to find the best possible move.
* **Minimax Algorithm:** Implements a robust decision rule used for minimizing the possible loss for a worst-case scenario.
* **Depth-Aware Scoring Heuristic:** The AI doesn't just look for a win; it optimizes for efficiency. 
  * **Quick Wins:** The scoring function uses a `10 - depth` calculation to prioritize winning the game in the fewest moves possible.
  * **Delayed Losses:** If a loss is inevitable, the AI uses a `depth - 10` calculation to prolong the game and force the opponent to work for the win.
* **Board State Evaluation:** Capable of loading specific mid-game configurations to predict scores and determine the exact optimal column for the next piece (e.g., predicting a score of 7 and identifying Column 3 as the best move).

## Technology Stack
* **Language:** Python

## Getting Started

### Prerequisites
* Python 3.x installed on your local machine.

### Installation
1. Clone the repository:
   ```bash
   git clone [https://github.com/OMZaky/Connect-4.git](https://github.com/OMZaky/Connect-4.git)
