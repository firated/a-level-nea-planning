# a-level-nea-planning
## Planning 
// Creating an AI chessbot
// Section 1: Definition, Investigation and Analysis
- Problem Definition:
  For my NEA I will be coding an AI bot based on the most popular board game in the world, as well as being played for centuries, called 'Chess'. The game involves a total of 16 pieces, including 8 pawns, 2 rooks, 2 bishops, 2 knights, 1 queen and a king. The main object for a player is to completely surround the king with each pieces, leaving no path for the king to move.

  (Screenshot of a chessboard)

  Chess involves multiple rules for each pieces, as well as how the game could end. In terms of pieces, each one of the them has different sets of movements such as the pawn being able to move by 2 blocks from its starting point and afterwards only one block each move. The rooks are able to move in straight lines front, back, left and right. Bishops are able to move diagnally. Knights are able to move in L shapes. The most powerful piece of all is the queen where it is able to move both diagnally and in straight likes side to side, front and back like the rook. As for the king it can move around a 3x3 square only if there is a path.
  The main objective of this project is to create a chess AI bot that is able to play against users at different levels.

- Chess System

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
                                                                          
