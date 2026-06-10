*This project has been created as part of the 42 curriculum by ravazque and acerezo-.*

---

## Description

Gomoku is an AI project: build a program that **plays Gomoku and beats human players**, implemented in C++ with a playable graphical interface.

The game follows the subject's competitive ruleset rather than the classic one: a 19×19 goban where five (or more) aligned stones win, **Pente-style pair captures** (ten captured stones also win), an endgame rule that lets a capture break a five-in-a-row, and the prohibition of **double free-threes**.

The AI is built around the **Minimax algorithm with alpha-beta pruning**, supported by:

- A hand-crafted **evaluation heuristic** that scores alignments, captures and threats.
- **Move ordering**, candidate-move restriction and transposition tables, so the search reaches the required depth while keeping the average move time under half a second.
- A visible **timer** displaying the time taken by each move.

The program offers a human-vs-AI mode and a human-vs-human hotseat mode where the engine suggests a move to each player.
