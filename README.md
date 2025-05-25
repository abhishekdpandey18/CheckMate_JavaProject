# GUI-Based Java Project

## 📋 Project Overview
This is a Java-based GUI project developed as part of an academic assessment. The project includes database integration using JDBC and a visually appealing, responsive user interface.

---

## 🛠️ Development Setup

### ✅ JDK Version
- **JDK Version**: `Java SE Development Kit 17`
- Make sure JDK 17 is installed and configured in your environment.
- [Download JDK](https://www.oracle.com/java/technologies/javase-downloads.html)

### ✅ IDE Used
- **IDE**: `IntelliJ IDEA Community Edition 2023`
- You may also use `Eclipse` or `VS Code` with Java extensions.

---
## 📁 Project Structure

JavaChess-main/
├── .idea/
├── bin/
│   └── com/
│       └── chess/
│           └── engine/
│               ├── board/
│               │   ├── Board.java
│               │   ├── BoardUtils.java
│               │   ├── Builder.java
│               │   ├── Move/
│               │   │   ├── AttackMove.java
│               │   │   ├── CastleMove.java
│               │   │   ├── KingSideCastleMove.java
│               │   │   ├── MajorMove.java
│               │   │   ├── MoveFactory.java
│               │   │   ├── NullMove.java
│               │   │   ├── PawnAttackMove.java
│               │   │   ├── PawnEnPassantAttackMove.java
│               │   │   ├── PawnJump.java
│               │   │   ├── PawnMove.java
│               │   │   ├── PawnPromotion.java
│               │   │   ├── QueenSideCastleMove.java
│               │   └── Tile/
│               │       ├── EmptyTile.java
│               │       ├── OccupiedTile.java
│           ├── pieces/
│           │   ├── Bishop.java
│           │   ├── King.java
│           │   ├── Knight.java
│           │   ├── Pawn.java
│           │   ├── Piece.java
│           │   ├── Queen.java
│           │   └── Rook.java
│           ├── player/
│           │   ├── ai/
│           │   │   ├── BoardEvaluator.java
│           │   │   ├── MiniMax.java
│           │   │   ├── MoveStrategy.java
│           │   │   └── StandardBoardEvaluator.java
│           │   ├── BlackPlayer.java
│           │   ├── MoveStatus.java
│           │   ├── MoveTransition.java
│           │   ├── Player.java
│           │   └── WhitePlayer.java
│           └── Alliance.java
├── src/
│   └── com/
│       └── chess/
│           └── engine/
│               └── [Same as bin structure...]
├── GUI/
│   ├── GameHistoryPanel.java
│   ├── GameSetUp.java
│   ├── Table.java
│   └── TakenPiecesPanel.java
├── JChess.java
├── Chess pieces/
│   ├── BB.gif, BK.gif, BN.gif, BP.gif, BQ.gif, BR.gif
│   ├── WB.gif, WK.gif, WN.gif, WP.gif, WQ.gif, WR.gif
│   ├── green_dot.png, red_dot.png, illegal.png
├── JavaChess-main.iml
├── README.md
└── out/ [build output]

