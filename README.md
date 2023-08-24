The full release of the asigment!
---

Patch-notes
_______
Mechanics
- Double Jump
  - While in the air the player can press 'space' again in order to double jump
  - This also works when the players 'falls'
- Dash
  - A super fast horizontal movement in the direction of the current(ish) vector of movement   
  - On ground, it has a cooldown
  - It also works while in the air, but only once

The edited script for these mechanics was the **PlayerCharacterController.cs** i surgically edited this script to add both mechanics, that means i copy and pasted the jump thing to make another jump thing and kinda used the jump thing to make the dash thing.
For the dash mechanic i also added some sort of 'timer' in order to mimic a constant acceleartion and avoid the normal acceleration calculation to take place while the player 'isDashing'. Not the most elegant solution (a co-routine is probably the best way to implement this) but it works.
**PlayerInputHandler.cs** was also edited in order to include a new key (only for the keyboard)
_______
Levels

- DoubleJump
  - A simple level where the player has to use double jump in order to complete the level
  - An objective indicating that this level is a 'tutorial' was added
- DashTutorial
  - Another simple level, this time we present the 'dash' mechanic to the player
  - A couple of objectives had been added to indicate the player what they should do
 Both of this levels 'teach' the basic aspects of the mechanics, including a place where the player has to drop and then use jump and dash to reach the end of the level
- ExtraLevel
  - A big challenge!
  - More enemies (maybe too many enemies)
  - Two secret weapons
  - A secondary objective has been added, to reach it the player must use everything they lerned to reach the end and get their sweet, sweet reward
_______

Also added a flow to the levels (in a really lazy way but it works)
And edited the PNG with the controls to match the new imputs (i botched the image with Paint and i regret nothing)
__________

No build provided but launching 'IntroScene' should be enough to play trough the three levels.
