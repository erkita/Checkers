## User vs Computer Checkers Game

--------------
### Demonstration
Below will demonstrate a game between a user (black checkers) and computer (red checkers). It demonstrates double and triple captures, computer moving red checker pieces during its turn, crowning of a king piece, and king piece being able to move in both directions.<br />
![ezgif com-gif-maker](https://user-images.githubusercontent.com/82434097/116802482-08a2cc00-aac8-11eb-8330-195dc659e2e4.gif)<br />

### Overview
This graphical game of Checkers was made utilizing a turtle module. The game is played with black (user) and red (computer) pieces on a 8x8 board. The goal of the game is to capture all of your opponent’s pieces. Following are the rules applied in the game:<br />
* Each player starts with 12 pieces.
* The user can make moves by clicking on the square containing the piece they would like to move, then clicking on the square the piece should be moved to.
* Pieces may only be moved diagonally by one square and in forward (player's start side to opposite side) direction.
* A piece is crowned "king" when it reaches the opponent's first row. It is identified by the crown mark on the piece.
* King pieces may move forward and backwards.
* Capturing moves can be made if an enemy piece is next to the player’s piece, and the next forward square in the same direction is empty.
* The captured piece is removed from the board and a score point is added to the capturing player.
* If a capture is possible, then it must be made.
* Multiple capture is possible in a single turn as long as the capturing piece continues forward. For a king piece, multiple capture may go both diagonally forward and backward. 
* The game ends when a player has captured all enemy pieces or when one of the players cannot legally move their remaining piece(s). "Game over" and the winner will be declared on the screen.<br />
<img width="443" alt="Screen Shot 2021-05-01 at 9 55 30 PM" src="https://user-images.githubusercontent.com/82434097/116802474-f2950b80-aac7-11eb-864a-b6f0ea360869.png"><br />


### Design
```main.py``` acts as a driver file that draws the board and executes the game while ther files represent game objects. Some files such as ```board.py``` and ```checkerutilities.py``` heavily uses turtle to generate 
a checkerboard and checker pieces.  The rules and basic mechanism of the Checkers game is represented by ```gamestate.py```. This class takes an instance of ```botplayer.py``` as a field which represents the computer player's selection of checker piece movements.<br />

### Coordinate convention
The following coordinate convention of checkerboard used in program. The origin is set to the upper-left corner of the board.<br />

<img width="1286" alt="checker_board" src="https://media.github.ccs.neu.edu/user/7830/files/d07bcb00-2e4f-11eb-835c-4200bcb59ebf">
