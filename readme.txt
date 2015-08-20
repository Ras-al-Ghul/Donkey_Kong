Donkey Kong!!

Game notes:

To play the game run the "game.py" file.
Type "python game.py" in the console.

This game works only on Linux as it uses "pyxhook" for input which is a Linux only version of the Windows "pyhook".
The file "pyxhook.py" is the Copyright (C) of Tim Alexander <dragonfyre13@gmail.com> 2008.
It is licensed under GNU's GPL.
To use "pyxhook", Python's Xlib module needs to be installed if it is not already installed.
One can increase the sleep time, if the terminal screen flickers.

Some features about the game:

OOP concepts have been used extensively.
The main bonus features of the game are:
1) The FLOORS are RANDOMLY GENERATED (even for the same level) using a kind of backtracking algorithm ensuring the freshness of the game.
2) The STAIRS are RANDOMLY GENERATED and care is taken that there is atleast one path from the player spawn position to the princess.
3) The differences between the levels are:
	1) There are MORE DONKEYS in the higher levels (1 in level 1, 2 in level 2, 3 in level 3).
	2) There are MORE FIREBALLS in the higher levels.
	3) There are LESS STAIRS in the higher levels meaning less paths to the pricess and more difficulty.
	4) There are LESS COINS in the higher levels meaning a lower score results.
4) The user has complete control over the number of donkeys, the number of fireballs and the number of stairs.
   All the three can be reset changing a maximum of two variables each. This is possible because there is no hardcoding whatsoever.
5) Multiple donkeys make the game more challenging.
6) The STAIRS ARE MADE TO BREAK if two fireballs move over them at the same time or if a player collides with a fireball on a stair.
   This ensures a more challenging game and the player has to be real quick to finish it.
7) If the stairs break, the game is as good as over and the player has to quit.
8) One can CHANGE THE ROWS AND COLUMNS.To do this, change the "ROWS" and "COLUMNS" values in the "game.py" file.
9)The donkeys DIE if the player collides with a donkey. This is done so that the game is playable and not too hard.
10)Care has been taken to ensure keyboard responsiveness and lag mitigation.
11)Comments have been provided in the sourcecode where ever necessary.
12)Jumping using the spacebar may take a while to get used to. If the user has pressed "d" and then space, then the player jumps to the right.
   Similarly for left. If it has been more than a second since a user pressed "a" or "d", then on pressing space, the player jumps vertically.
13)Colors have been added to make the game attractive.