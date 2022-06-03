# 2048_GAME
first import pygame

1. For left swipe, we will just compress and then merge the gridCell matrix and then if compress or merge is true (indicating the values of the matrix is affected by previous two functions), then we need to compress the grid again.
2. For moving up, we will take transpose then swipe left and again take transpose to return to the original order.
Moving down is same as moving up but we need to reverse the matrix.
3. Similarly, right is same as moving left+reverse.
4. After every operation, we need to check the game status, if all cells are occupied and we cannot even merge any two cells i.e. the state where no movement can change the matrix, then the game is over.

If any cell value has reached 2048, then the player is won and a message box is flashed on the screen announcing the winner.
