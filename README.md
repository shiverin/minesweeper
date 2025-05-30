# Minesweeper AI Agent

A AI agent that plays the classic Minesweeper game using logical inference and knowledge representation. Developed in Python, this project demonstrates advanced problem-solving skills, set manipulation, and intelligent decision-making through knowledge-based reasoning.

## Overview

This Minesweeper AI mimics human deduction to solve Minesweeper boards. It builds and continuously updates a knowledge base of logical sentences representing safe cells and mines. The AI then infers safe moves and mines by analyzing relationships between these sentences.

By leveraging set theory and propositional logic, the agent can solve many Minesweeper puzzles efficiently, marking cells as safe or mines with high accuracy. When no certain moves remain, it makes probabilistic guesses to continue the game.

## Key Features

- **Logical Knowledge Representation:**  
  The AI constructs and updates sentences about the board, encoding which cells might be mines and how many are contained within a subset.

- **Inference through Subset Relationships:**  
  New knowledge is inferred by comparing sentences using subset relations, allowing the AI to deduce additional safe cells or mines.

- **Dynamic Knowledge Base:**  
  Sentences with empty cell sets are cleaned up to maintain efficiency. The knowledge base is updated as new information is gained.

- **Safe and Mine Marking:**  
  Cells confidently identified as mines or safe are marked, helping avoid errors and improve subsequent inferences.

- **Random Move Strategy:**  
  When no known safe moves remain, the AI intelligently picks random moves that are least likely to be mines.

## Technical Highlights

- Python 3 implementation with custom `Sentence` class encapsulating board knowledge.
- Use of sets and subset checks for logical deduction.
- Efficient updating and pruning of the knowledge base to optimize performance.
- Clear separation of knowledge updating, inference, and move-making logic.
- Extensive use of object-oriented design for modularity and clarity.

## How It Works

1. **Add Knowledge:** When the AI uncovers a safe cell and the number of neighboring mines, it creates a sentence representing the unknown neighboring cells and the mine count.

2. **Mark Known Mines and Safes:** Using the knowledge base, the AI identifies cells that must be mines or safe and updates its internal records.

3. **Infer New Knowledge:** By checking if one sentence’s cells are a subset of another’s, the AI infers new sentences to add to the knowledge base.

4. **Make Moves:** The AI chooses known safe moves first. If none are available, it makes an educated random move.

## Why This Project?

This project showcases:

- Logical reasoning and AI problem-solving skills.
- Expertise in data structures like sets and lists.
- Ability to implement algorithms for knowledge representation and inference.
- Clear and maintainable code design.

It also demonstrates a deep understanding of Minesweeper’s underlying logic, allowing an AI to “think” about the board.
