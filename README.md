# Bugs and improvements for tic tac toe game:

## Preconditions:
1. Open the [game](https://qatest.staging.forasoft.com/) for the first player, **first player for X**;
2. Open the [game](https://qatest.staging.forasoft.com/qatest.staging.forasoft.com?id=408771690213560267MHWMxw6leaaEPqDzAAMk) in other window for the second player, **second player for 0**.

## Bugs:

### Critical: By clicking on the lower central cell, the player is given one more move for the opponent

**Steps:**
1. As the first player, click on any cell except the bottom center;
2. As the second player, click on the lower central cell;
3. As the second player, click on any cell.

*Actual result:* the symbol 'X' is on the cell, the second player went twice, the order of moves has gone astray, the first one now plays for 0, and the second one for X

*Expected result:* the symbol 'X' doesn't appear, so the first player(not the second) should go on playing

**Test environment:**
* **Operating system:** Windows 11 Home
* **Browser:** Yandex.Browser, Version 23.5.2.625 (64-bit)

### Critical: When one of the players wins by getting the combination of three(X or 0) diagonally from top left to bottom right, the game does not show anything to confirm his success and continues

**Steps:**
1. As any of two players, get the combination of three X or 0 diagonally from top left to bottom right.

*Actual result:* nothing happens, players are have to go on the game

*Expected result:* players get the message, that congrates the winner

**Test environment:**
* **Operating system:** Windows 11 Home
* **Browser:** Yandex.Browser, Version 23.5.2.625 (64-bit)

### Major: When the game ends, there is no ways to continue playing
**Decription:** to continue playing, players need to reopen the game window. This is so exhausting.

**Steps:**
1. As any of two players, get the winning combination or draw the game by filling in all the fields.

*Actual result:* as in case of winning, as in case of draw, there is no button to click to continue playing

*Expected result:* at the end of the game the restart button is appeared

**Test environment:**
* **Operating system:** Windows 11 Home
* **Browser:** Yandex.Browser, Version 23.5.2.625 (64-bit)

## Improvements:

1. It would be better to make the playing field bigger and move it to the right away from the chat field;
2. It would be better to make the chat field a bit smaller;

