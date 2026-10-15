9:03 AM 3/3/2013
CAEJones

This is mostly a test of an audio platforming concept.
The fighting doesn't work.
You can add zombies in the editor, but they don't do anything.
Sorry about that.

To access the editor, press ctrl+u

The sounds of the various platforms come from the closest edge of the object to the camera.
So if, for example, you're standing on a squeaky board, you'll hear that creeking from center if you are standing atop it, regardless of how close you are to the edges.
But if you are to the left or right of the board, you'll hear the sound from the right or left.

The pitch of a sound drops slightly when it is below the camera, which is hopefully sufficient to distinguish whether an object is above or below.

Normally, the camera is linked to your position, but you can hold alt and use the directional controls to move the camera a short distance.
This lets you examine the shape of objects better than you could by walking around, and without risking falling off an edge!

Wind sounds will play from the edges of whatever you're standing on. This doesn't indicate whether there is something safe to step onto beyond that edge or not, so you might want to try looking around if you aren't familiar with the area.


The editor gives you some tips, but here are a few more keystrokes:

w : change width of map
h : change height of map
s : save map
l : load map
home: move to left edge of map
end: move to right edge of map
page up : move to top of map
page down: move to bottom of map
enter: select object at cursor
shift+enter: edit selected object
space: add object at selected area
delete: remove object
m : set mark. Objects are created between the mark and the cursor, so this is kinda important.
shift+m: move to mark
v : hear position and selection.

