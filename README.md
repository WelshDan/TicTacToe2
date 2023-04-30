# Tic Tac Toe  

This website provides a simple game for two human players to play the classic game Tic Tac Toe. Tic Tac Toe is a turn-based game where players take it in turns to lay their game piece in a 3x3 grid with the aim of forming three-in-a-row. The match is won when a player can get three of their own game piece in a row, whether it be horizontally, vertically or diagonally. A match can be drawn if neither player achieves a three-in-a-row before all the areas of the grid have been filled. Then the game can be just restarted and enjoyed all over again!

This game shows the basic functions in HTML, CSS and JavaScript so can be interesting to look at from that perspective - if the game is not interesting enough!

![Screenshot](assets/images/multidevice.jpg)

## Features


### Page layout

Website has its own unique favicon ![Screenshot](assets/images/favicon.ico) 


The website is all focused onto one page so there are no links to any other pages.

There is a Heading Box at the top which displays the name of the game and that there are two players who can play.

![Screenshot](assets/images/pagelayout1.jpg)

In the middle of the page is the playing grid. Is is a 3x3 grid of squares that can be clicked on during the duration of the game. Player 1 will enter X's and Player 2 will enter O's. <br>
These individual squares are clickable during the game and will insert an X or an O depending on which you have chosen.

![Screenshot](assets/images/pagelayout2.jpg)

There is a status bar underneath the playing grid. This will display one of the following "Player X's turn" or Player O's turn" during the game and once a game is finished it will display either "X wins", "O wins" or "It's a draw!" depending on the result.

![Screenshot](assets/images/pagelayout3.jpg)

At the bottom is the Play Again button which will reload the page when clicked.

![Screenshot](assets/images/pagelayout4.jpg)

And finally the footer which includes the author of the website.

![Screenshot](assets/images/pagelayout5.jpg)

## Bugs

### Resolved issues

There were a few bugs which have now been remedied:
 - Squares could be clicked on multiple times even if they were previously chosen and it also saw a change of player. What should have happened is that the square once chosen is then blocked from further clicks. This issue was solved by ensuring that during the onTileClick function an "if tile was empty" check was inserted secondly in the onTileClick function.<br>
 - The player could continue clicking on empty squares even after the game was finished. This was corrected by first entering a "running = false" line in the roundWon part of the checkWinner function. Then after inserting a "game still running?" check initially in the onTileClick function, it stopped the clicks once the game is over.
 <br>

### Unresolved issues

- "New Game" Button
Expected = Clicking "New Game" button clears game board<br>
Tested = Clicking on "New Game" button<br>
Result = Game board not cleared<br>
Fix= A reload page command was inserted.<br>

- Game grid layout
Expected = Layout aligns when changing to smaller screen<br>
Tested = Layout sizes changed in Google Dev Tools<br>
Result = Layout of game grid is not aligned correctly on the iPad on the MultiDevice picture<br>
Fix = No fixes made<br>


## Validator testing

HTML - W3C validator

![Screenshot](assets/images/w3validator.jpg)

CSS - official (jigsaw) validator

![Screenshot](assets/images/w3CSS.jpg)

I have run this page through dev tools Lighthouse function:

![Screenshot](assets/images/lighthouse.jpg)

## Deployment

The website has been deployed through gitHub and can be found in the following link:
https://welshdan.github.io/TicTacToe/

## Credits

Tips and help:

W3.org - centering of start box / color coding<br>
JavaScript Master - startGame functions and layout help (https://www.youtube.com/watch?v=Slj9rPBJTcY&t=1214s)<br>
Emer Heffernan, personal tutoring and help<br>
Code.mu Winner check function (https://code.mu/en/javascript/book/practice/tick-tack-toe/victory-checking/)<br>
My mentor Akshat Garg, for his guidance and assistance.<br>
