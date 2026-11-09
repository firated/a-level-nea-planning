# a-level-nea-planning
## Planning 
// Creating an AI chessbot

Section 1: Definition, Investigation and Analysis
- 1.1 Problem Definition:
  
  For my NEA I will be coding an AI bot based on the most popular board game in the world, as well as being played for centuries, called 'Chess'. The game involves a total of 16 pieces, including 8 pawns, 2 rooks, 2 bishops, 2 knights, 1 queen and a king. The main object for a player is to completely surround the king with pieces, where the king has no more legal moves and no way to attack the oppositions piece, leaving no path for the king to move.

  (Screenshot of a chessboard)

  The main objective of this project is to create an AI chess bot that human players are able to compete against. The AI bot will be capable of playing legal moves and evaluating the best moves/position to play. The program will have difficulty options, where users with varying experiences can play at their level.

- 1.2 Research and Investigation
    
  - How chess is played:
    - Movement system:
      Chess involves multiple rules for each pieces, as well as how the game could end. In terms of pieces, each one of the them has different sets of movements:
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

  - AI/Bot Algorithm
      - Determining the search algorithm
   
        There are various algorithm that can be used to code the AI model, such as a Deep Convolutional Neural Networks (Deep learning), which involves the usage of large datasets to train the algorithm to notice specific patterns and base its movements on millions of data from real-life users. Although this algoritm offers limitless possibilities in terms of Artificial Intelligence, I've decided to opt for the traditional AI algorithm called 'Minmax and Alpha-beta pruning'. This algorithm is the most appropriate for a project of this scale.

      - What is Minmax and Alpha-beta pruning?

        Minmax is a search algorithm, mainly for a 2-player game, that evaluates every possible option and computes the best possible result assuming the player is playing in an optimal way, which is perfect for chess. By using this algorithm, it allows for the creation of an intelligent bot that can make moves according to the response of an opponent, where it will then calculate the possible moves, and potentially think ahead into what the opponent can do next.
   
        
        Alpha-beta pruning is an algorithm optimisation technique, specifically for the Minmax algorithm. It optimises by removing unnecessary calculations, if it is able to analyse that another branch of the minmax algorithm leads to a worse outcome.
        
    
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


    An important factor that makes chess functional is the game itself. Above is a simple system I made to clarify how the game functions.
    The challenge within this section would mainly be to make a functional board with all the other rules associated with the official game. 

  

  - User Identification
    
      End users of this program could be open to anyone. Since chess is such a widely recognised and played game, though it would mainly target those who play chess to use this software to improve their gameplay.

  
    - Questionnaire
      
    As a way to gather information for the development of this software, I will be surveying .. people, who has plenty, some and little to no experience with chess to see their suggestions on things they’d like to see in this software.
    I have surveyed 10 people regarding features, quality of life improvements and suggestions to be implemented into this software.

1. How often do you play chess?
   - Never
   - Occasionally
   - Sometimes
   - Often
   - Always
    
2. What do you think your level of chess is ? (if you have played)
   - Beginner
   - Intermediate
   - Advanced
   - Expert
    
3. What’s your preferred way of playing chess? (Software/Physical)
   - Free Response
    
4. If you play software, where do you play?
   - Free Response
  
5. What kind of methods would you want for the difficulty?
   - Optional difficulty (Easy, Medium, Hard)
   - Tactics-based difficulty (Aggressive, Defensive)
   - Difficulty Slider
   - Adaptive difficulty
   - Combination of each
  
6. What would you expect from an easy AI difficulty?
   - Simple/Random moves
   - Reasonable moves, may miss tactical
   - Other: Free response
  
7. How fast do you expect an AI to make a move?
   - Less than a second
   - 1-3 seconds
   - 3-10 seconds
   - Varying time to move based on difficulty
  
8. Would you like a game analysis feature? (Enable stats of each game to be shown)
   - Yes
   - No
   - Maybe

9. What kind of UI would you suggest?
    - Minimalistic (Chess board and timer)
    - Feature heavy (Stats and other features)
    - Other: Free response
  
10. Would you like to save your chess games (potential option of replaying moments of your game)
    - Yes
    - No
    - Maybe
   
11. Would a beginner friendly option be useful (For teaching basis of game)
    - Yes
    - No
    - Maybe

12. What would be the most useful feature of Chess Bot software?
    - Free Response

13. Are there any other features you’d suggest?
    - Free Response
   
    
