# Python Atomic Chess Engine

A console-based implementation of **Atomic Chess**, a chess variant where every capture triggers an explosion that destroys nearby pieces.
This project was written in Python and implements standard chess movement rules along with the special explosion mechanics used in Atomic Chess.

---

## Features

- Standard chess starting board
- Algebraic move input (`a2 a4`)
- Turn-based gameplay
- Piece movement validation for:
  - Pawn
  - Rook
  - Knight
  - Bishop
  - Queen
  - King
- Atomic chess explosion mechanics
- Automatic win detection when a king is destroyed
- Console board display for testing and gameplay

---

## Atomic Chess Rules Implemented

The game follows normal chess movement rules with the following differences.

### Explosion Rule

Whenever a capture occurs:

- The **captured piece is removed**
- The **capturing piece is also destroyed**
- All **non-pawn pieces in the surrounding 3×3 area explode**
- **Pawns adjacent to the capture survive**
