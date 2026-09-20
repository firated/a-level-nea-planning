# a-level-nea-planning
## Planning 
// Creating an AI chessbot

Section 1: Definition, Investigation and Analysis
- Problem Definition:
  For my NEA I will be coding an AI bot based on the most popular board game in the world, as well as being played for centuries, called 'Chess'. The game involves a total of 16 pieces, including 8 pawns, 2 rooks, 2 bishops, 2 knights, 1 queen and a king. The main object for a player is to completely surround the king with each pieces, leaving no path for the king to move.

  (Screenshot of a chessboard)

  The main objective of this project is to create an AI chess bot that human players are able to compete against. The AI bot will be capable of playing legal moves and evaluating the best moves/position to play. The program will have difficulty options, where users with varying experiences can play at their level.

- Research and Investigation
    
  - How chess is played
    - Movement system:
      Chess involves multiple rules for each pieces, as well as how the game could end. In terms of pieces, each one of the them has different sets   of movements:
    
      - Pawn: able to move by 2 blocks from its starting point (En Passant) and afterwards only one block each move.
      - Rook: Move in straight lines front, back, left and right.
      - Bishops: Move diagnally.
      - Knights: Move in L shapes.
      - Queen: Most powerful piece and is able to move both diagnally and in straight likes side to side, front and back like the rook.
      - king: Can move around a 3x3 square only if there is a path.

    - Game Ending conditions:
      In chess there are two ways a game could end, as a win or a draw:
        - Check: When the king is within directory of an opposing piece's movement
        - Checkmate: Win for whichever player that is able to check the king and block all of the opposing king's path.
        - Stalemate: A draw for both players, where each player's king is not in check and there's no legal move left.
      
    - Legal Moves:
      These are moves in which players must follow:
        - White moves first: White starts first every game, and one piece is played each turn.
        - No self-checks: If a player's king is in check, you must either play a piece to block the check, or you cannot move the piece away from                              the positon if it endangers the king.
        - Movement: Each piece can either take the opponent's piece or move into a vacant space.
        - Jumping: No piece can jump over each other, except the knight and castling (special move).
  
    - Special Moves:
      In some circumstances, special moves can be played:
        - En Passant: The pawn can move 2 squares forward if it has not been moved yet.
        - Castling: If neither the rook or king has been moved, the king can move 2 spaces towards the rook. The rook would jump over the king.
        - Promotion: If the pawn of a player reaches the other end of an opposing player's board, it is able to be changed into any pieces.
    
- Basic chess System

                                                      Start
                                                        |
                                                        |
                                          setup chess board and pieces
                                                        |
                                                        |
                               ---------------Player turn (white first)
                               |     |                  |
                               |     |     No           |          Yes
                               |      ---------- is move legal? ---------- Move the piece
                               |                                                  |
                               |        No                           No           |
                               -------------------- Stalemate?  ------------ Checkmate?
                                                        |                         |
                                                        | Yes                     | Yes
                                                        |                         |
                                                       Draw            Game Over (Declare winner)
  

  - Potential user-base
      End users of this program could be open to anyone. Since chess is such a widely recognised and played game, it would mainly target those who     play chess. By clarifying my playerbase, it is important to gather the information from those who play to game, for suggestions of features to       further enchance the program.
