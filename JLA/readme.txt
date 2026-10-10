--- This file may be incomplete. Try the in-game help (F1) for help.
--- check http://audiogames.net if you have further questions.


== overview ==

  This game is a 2D sidescroller. Use the arrow keys to navigate menus or select your character, or to move your character while in-game. 
  While in menus, the enter, or spacebar keys will activate the currently selected item. In the case of character selection, this will have you enter the game with the selected character. Pressing escape will attempt to close or cancel a menu. 
  The game consists of several levels, each constructed randomly based on a certain theme. Levels are cleared by either defeating that level\'s boss, or by reaching the exit. 
  Clearing some levels will unlock new heroes that you can use in-game. You can also play levels that you\'ve already cleared with the unlocked heroes. Your progress is automatically saved when a level is cleared or you exit the game. 
  Your goals will vary from level to level, but as a general rule, you want to defeat enemies (the ones that make threatening remarks and/or attack people) and protect civilians (the ones screaming for help and/or going about their business). 
  Each character has a variety of skills. You can select which skill to use with the number row--pressing 1 usually sets you to using fists, for example. Press space to use the selected skill. 
  Some skills have limited ammo, or draw on your power reserves. You can check these with the A and P keys. 
  There will be times in which you need to interact with your environment in a more direct way, such as collecting items, moving or talking to civilians, or hiding in dark alleys. Most of these can be accomplished by pressing enter. 


=== Control list ===

Jump, or fly up: up arrow
 crouch, or fly down: down arrow
 left: left arrow
right: right arrow
attack, or use item: spacebar
interact or pick up item: enter
select power or item: 1-9
hold shift while moving to move faster
look: hold alt and press a direction
look in bounds: alt+space
Hear ammo: A
hear health: H
hear coordinates: C
Hear power: P
Hear current skill or item: S
Voice options: F5
Control list: F1
Pause / main menu: Escape"
adjust BGM volume: page up / page down


=== Concepts ===

Generally speaking, this is a sidescroller, with the main idea being to defeat the enemies.
The game is fully 2d, with both horizontal (x) and vertical (y) motion possible.
Some characters can fly. Those who can't can jump and crouch.
Often, jumping is not enough to reach the tops of buildings, statues, or whatever you're trying to climb. Some characters may have to deal with this, while others have tools like grapplinghooks to reach high places.
Sometimes, enemies will be wandering about in high places, but they tend to favor the ground. More often, your reason for climbing will be to pick up items, perhaps to refill supplies, perhaps to restore some health, or perhaps to find a key or some other necessity for advancing. Well, and there are quite a few cities with quite a bit of traffic. You might try jumping cars, or hiding in an alley until they pass, or you could make for the rooftops and ninja about that way.
Be warned, though, that most of the time, you're walking on narrow ledges, and falling at a high enough speed can cause you to fall past them anyway. As you might expect, this makes jumping from rooftop to rooftop a bit tricky.

There is a pseudo 3d(z) element, in that objects can be in the background, foreground, or the middle of the area. By default, all characters focus on the middle area, and most solid objects that one can stand on can be reached regardless of their z position.
At this point, you might wonder what the point of the z element is. It has quite a few uses, in fact. The most obvious is that walls and other barriers only affect people on the same z.
So, for instance, you can run through the streets of Gotham and pass all of the buildings, but if you duck into an alley in the background, any buildings in the background can block your path.
Similarly, if you run into an obstruction like a destroyed vehicle or a security door, you can step around it if there is an object in the background or foreground that you can enter, such as an alley or a room.
(You can enter and exit objects such as alleys, rooms, etc by pressing enter while near them, but keep in mind that if there is a solid object at the same z, you won't be able to enter from its position.)
The z element also affects projectiles, of which there are many, and some other types of attacks. It does not, however, affect punches. So, for instance, Batman stands atop a building, while the Joker walks by, devilishly twirling his favorite uzi in one hand and clutching his acid-spraying flower in the other. You could jump down and attack directly (and get shot and/or melted), or, if the Joker is approaching an alley that runs by the building, Batman could simply dive into the alley (be sure to press enter so that you don't just land in front of it), and sucker-punch the Joker, safe from both bullets and acid.

Most attacks can be aimed, and most enemies aren't particularly clever about their own aiming (this depends on the difficulty, and even then, it's mostly bosses who bother to aim). You can only really aim in the four primary directions--up, down, left, or right--not so much diagonals.
To aim, simply hold the direction while performing the attack (space). For projectiles, one only need hold the directions until the projectile is launched, whereas for non-projectiles, the buttons must remain held until the attack completes.

=== Technical issues ===

First, let's explain a couple of in-game options, then move on to the more annoying side-effect of having such massive levels full of stuff.

Hopefully the "voice options" item on the main menu is self-explanetory, but if it isn't, it allows you to select a sapi voice (or to use the active screen reader), and adjust settings such as speaking rate (and sapi pitch, if you really want to). These settings will be saved and loaded automatically.

The "difficulty" option affects a number of things that, as one might expect, influence how difficult it is to complete the game, such as when enemies attack, how often they aim intelligently, etc.
One particular effect you might be interested in is that the difficulty determines how likely a moving object, such as a car, is to hit enemies as well as the player. On the easy setting, one could stick to the rooftops and let traffic wipe out the enemies, while on superhuman, enemies will never be hit by anything but your attacks and their own misfiring projectiles.
The reason the "cars-hit-enemies" effect is important is because of game performance. The more cars, and the more enemies, the more the game will need to do in order to check for collisions. So a lower difficulty on levels with lots of moving objects could result in the game running more slowly than at the highest difficulty.

Keeping a consistent game speed has been an important goal throughout development, but with a game in which so much happens, it is exceedingly difficult to prevent lag entirely.
To offset this, there are two special features that might help, but be warned that using them improperly can have undesired results.

The safest of these is the "step spread" value, which divides up how many items are to be investigated each frame.
This one is the safest in that it should not adversely affect speed, with or without lag.
To use this feature, press F3, and enter a number (must be positive, and greater than 0!). The bigger the number, the less work the game does each frame.
However, if the number you enter is too large, the game may become jumpy. Generally speaking, values between 1 and 15 (inclusive) are the best. If the game seems to be lagging, one might try entering a number such as 7 or 10.

A far less stable option is emergency speed.
To use this feature, press F2, and enter a number.
This value is the number of milliseconds to add to the native time of each frame.
Entering anything more than 300 here will probably cause the game to move too quickly to control; even in the worst-case situation (where lag is up to deciseconds), a high value can cause the game to become jumpy rather than offset lag propperly.
Emergency speed should be used as a last resort, and starting with smaller values (if 25-150 is not enough, going up to 200 or 250 probably won't help).
If the game lags badly enough that both of these features do not help, please let us know! If it happens consistently, please let us know the specifics (for instance, if it's worst on certain levels, at certain difficulties, etc).

=== Further support ===

You can contact us at http://www.audiogames.net (more specifically, the forums, which can be found at http://forum.audiogames.net ).
Or, you can visit us at www.PlanetSeva.com
Or the forums, at http://jeqo.proboards.com

While most of our games will remain free (*cough* especially those based on not-original works), having money to work with certainly helps improve the quality of our products, so if you are willing to donate, by all means, do so, at http://planetseva.com/audiogames.htm
