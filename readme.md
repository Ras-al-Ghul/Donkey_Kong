#Donkey Kong



###To play the game

- `sudo apt-get install python-Xlib`
- `python game.py`

This game works only on Linux as it uses `pyxhook` for input which is a Linux only version of the Windows `pyhook`.
The file `pyxhook.py` is the `Copyright (C) of Tim Alexander` <dragonfyre13@gmail.com> `2008`.
It is licensed under GNU's GPL.
To use `pyxhook`, Python's `Xlib` module needs to be installed if it is not already.

###Notes

- OOP concepts have been used extensively.
- One can increase/decrease the `sleep` time in `game.py` if the terminal screen flickers.
- The `floors` are randomly generated (even for the same level) using a kind of backtracking algorithm ensuring the freshness of the game.
- The `stairs` are randomly generated and care is taken that there is atleast one path from the player spawn position to the princess.
- The differences between the levels are:
	-  There are more `Donkeys` in the higher levels (1 in level 1, 2 in level 2, 3 in level 3).
	-  There are more `Fireballs` in the higher levels.
	-  There are less `Stairs` in the higher levels meaning less paths to the princess and more difficulty.
	-  There are less `Coins` in the higher levels meaning a lower score.
- The user has complete control over the number of donkeys, the number of fireballs and the number of stairs. All the three can be reset changing a maximum of two variables each. This is possible because there is no hardcoding.
- Multiple `Donkeys` make the game more challenging.
- The `Stairs` break if two `Fireballs` move over them at the same time or if the `Player` collides with a `Fireball` on a `Stair`.This ensures a more challenging game and the player has to be real quick to finish it.
- If the `Stairs` break, the game is as good as over and the player has to quit.
- One can change the number of `rows` and `columns`. To do this, change the `ROWS` and `COLUMNS` values in the `game.py` file.
- The `Donkeys` die if the `Player` collides with a `Donkey`. This is done so that the game is not too hard.
- Care has been taken to ensure keyboard responsiveness and lag mitigation.
- Comments have been provided in the sourcecode where ever necessary.
- Jumping using the spacebar may take a while to get used to. If the user has pressed `d` and then `space`, then the player jumps to the `right`. Similarly for `left`. If it has been more than a `second` since a user pressed `a` or `d`, then on pressing `space`, the player jumps vertically.
- Colors have been added.
- The `Player` gets bonus scores when he performs some specific actions like killing a `Donkey` or rescuing the `Princess`.


