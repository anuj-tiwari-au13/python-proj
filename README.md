###### ANUJ TIWARI
###### CV Raman (AUFS013038)


# Python Chess Game

It is a player versus computer implementation of chess using the pygame library 
for Python. 

It includes all the essential rules for chess. The computer player uses the minimax 
strategy with alpha-beta pruning for generating and deciding moves. 

It explores all possible moves, then explores
their possible moves and so on. This essentially creates a search tree to a depth of 3.
Minmax algorithm is being used.

The best move is decided by evaluating the 'score' of the board. 

A graphical representation of the board is rendered with a side menu with contextual tips,
that displays useful information such as whose turn it is, if the move you're
attempting is invalid, if someone is in check, among other things.

The mouse is used to select pieces and move them. 

The program only allows you to make valid moves according to the rules of chess, and also includes the
special moves: castling, and promotion. 

The program automatically detects check and checkmate, and for the latter, ends the game and declares the winner.

For more specific instructions on how to play, see 'Usage Instructions'.

---
## Setup Instructions:


###### Make sure you're using python 3. Install Chess Game by running following commands.

### Install pygame
```bash
sudo pip install pygame
```

### Once pygame is installed, run the game
```bash
 python3 chess.py  
```

### Install Flake 8 
```bash
 sudo pip install flake8  
```
### That's it!

### PLAY !! 

###### If for whatever reason, pygame fails to install try:



###### also, maybe updating pip will help:

###### `sudo pip install --upgrade-pip`

### Windows
###### In the installer, make sure to add python to your PATH
Install the latest version of python 3 (Tested on 3.6.4 and 3.6.5)

https://www.python.org/downloads/release/python-365/

Then, Open a command prompt window:
```
pip -m install --user pygame
python chess.py
```
---
## Playing the Game:

#### Moving A Piece On Your Turn:
Use the mouse to select one of your pieces and then select the square you want to move it to.
If you selected one of your pieces, the square that piece is on will be highlighted
by a purple square. 
If you choose an invalid place to move to, a message will be displayed informing
you of the rule infringement, and you will be able to try again. If you decide
to not move this piece, just select it again to cancel the move, and the purple
square will go away to indicate that you deselected that piece.

#### Checking:
If your opponent places you in check, a message will be displayed informing you
that you are in check. Your next move MUST get you out of the check. If you attempt
to make a move that doesn't get you out of check, a warning message will be
displayed, and the move will not be allowed. Once you get out of check, the game
proceeds as normal.

#### Checkmate/End Game:
If there is indeed a checkmate, the game will end and the
winner will be displayed. To play again, close the game, and run it again.

#### Castling:
If the rook and the king have not yet moved, the spaces are empty between them,
none of the in betweens or the new location of the king are in check,
you can castle. To perform the castling maneuver, select your king, and then
select the square where the king moves in the castling maneuver, and the move
will be performed automatically. Refer to https://en.wikipedia.org/wiki/Castling
for valid criteria for castling, if you are unfamiliar with this rule.

#### Promotion:
If one of your pawns reaches the opposite end of the board, it will automatically
be promoted to a queen, because why would you want anything else?

----

## File Layout / Description:

##### chess.py:
Run this if you want to play the game

##### modules/board,py:
Contains the board class

##### modules/computer.py
Contains move generation and the computer player's minimax algorithm

##### modules/pieces.py
Contains all the chess piece classes

##### assets/
Contains picture assets

---



#### Font: Google Roboto
