Overview
This Python program implements a simple Tic-Tac-Toe game where two players take turns to mark spaces in a 3x3 grid until one of them wins or the game ends in a draw. The game is played via console input/output.

Components
createboard() Function
This function creates and prints the Tic-Tac-Toe board with empty spaces represented by underscores.
It prints the current state of the board to the console.
condition(s) Function
This function checks the winning conditions of the game.
It takes the current state of the board (s) as input and returns True if any player has won, otherwise False.
It checks for winning patterns horizontally, vertically, and diagonally.
startgame(s) Function
This function prompts the current player to input their move (position) on the board.
It checks if the selected position is available and updates the board accordingly.
If the position is already taken, it prompts the player to choose a new position.
Returns the position chosen by the player.
Main Game Loop
The main loop iterates for 9 rounds (maximum possible moves in Tic-Tac-Toe) or until a player wins.
It alternates between the two players in each round.
Each player inputs their move, and the board is updated accordingly.
After each move, the condition() function is called to check if any player has won.
If a player wins, the game announces the winner and exits the loop.
If no player wins after 9 rounds, the game announces a draw.
User Input and Player Identification
At the beginning of the game, it prompts players to enter their names.
It assigns 'X' to Player 1 and 'O' to Player 2.
Usage
Run the Python script.
Enter the names of Player 1 and Player 2 when prompted.
Player 1 starts the game, followed by Player 2.
Input the position where you want to place your mark (1 to 9).
The game continues until one player wins or it ends in a draw.
After the game ends, the program prints "GAME OVER".
Example Execution
mathematica
Copy code
| _ | _ | _ |
| _ | _ | _ |
| _ | _ | _ |

Player 1: Alice
Player 2: Bob
Alice, you will be using X
Bob, you will be using O

First Players turn Alice
Enter the position: 5
| _ | _ | _ |
| _ | X | _ |
| _ | _ | _ |

Second Players turn Bob
Enter the position: 1
| O | _ | _ |
| _ | X | _ |
| _ | _ | _ |

... Game continues ...

Second Players turn Bob
Enter the position: 9
| O | _ | X |
| _ | X | O |
| _ | _ | O |

Second Player Bob won the game
GAME OVER
Conclusion
This Python program provides a basic implementation of a Tic-Tac-Toe game that allows two players to play against each other. It demonstrates the use of functions, loops, conditional statements, and user input handling in Python.
