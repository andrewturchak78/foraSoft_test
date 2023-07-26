# Bugs and improvements for tic tac toe game:

## Preconditions:
1. Open the [game](https://qatest.staging.forasoft.com/) for the first player, **first player for X**;
2. Open the [game](https://qatest.staging.forasoft.com/qatest.staging.forasoft.com?id=408771690213560267MHWMxw6leaaEPqDzAAMk) in other window for the second player, **second player for 0**.

## Bugs:

### Critical: By clicking on the lower central cell, the player is given one more move for the opponent

**Description:** By clicking on the lower center cell, a player (for example, the first player playing for X) is immediately given the opportunity to resemble his opponent (for the second player, playing for 0). Moreover, if he makes a winning combination with a new symbol (with 0), he will be counted as a defeat, since he originally played for X.

**Steps:**
1. As the first player, click on the lower central cell;
2. Click on the box to the right of the bottom center;
3. As the second player, click on the box to the left of the bottom center;
4. As the first player, click on the center right field;
5. For the second player, click on the center left field
6. For the first player, click on the upper right field.

*Actual result:* The first player is considered defeated, as he has collected a combination of 0.

*Expected result:* the symbol '0' doesn't appear at the second step, so the second player(not the first) should go on playing for 0

**Test environment:**
* **Operating system:** Windows 11 Home
* **Browser:** Yandex.Browser, Version 23.5.2.625 (64-bit)

### Major: When one of the players wins by getting the combination of three(X or 0) diagonally from top left to bottom right, the game does not show anything to confirm his success and continues

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
3. It would be better if the chat displayed not only the time the message was sent, but also the author.
