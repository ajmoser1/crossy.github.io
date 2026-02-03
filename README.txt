crossy.github.io
One hour crossy road
My strategy for this assignment was to begin with a clear outline and directive for the overall project, then prompted the model from the bottom up. I found that only making one change at a time was the most effective and kept the project from being incomparable between a single iteration.

Initial prompt:
I'm completing a prompt-engineering/assisted coding project where I'm trying to recreate crossy road in under an hour by prompting/vibe coding with AI. Let's get started. This will be in whatever language you deem best for the project. First step: Implement the basic structure of the game, including a basic character icon, movement using the arrow keys, and lanes that can be traversed and give points for crossing. Keep in mind I only have an hour to create this, so if you have an idea of what I can prompt you with to speed things up/improve the game, add them.

Following prompts:

Add moving cars on road lanes. They can be as simple as red/blue rectangles. Make each lane have a slightly different car speed. Make the cars kill the player upon collision and provide a way to restart the game.

Add floating logs on water lanes as well as infrequent bridges: player dies if they are in the water and not on a bridge or log

Add rocks that block some of the horizontal movement on the grass lanes

(Ran into bug with rock collision)
Unfortunately the player can still walk through the rocks. Please make sure they can't. Check the collision logic again

(fixed after that prompt)
It works. Next, update the screen so the player stays in the middle when moving instead of being able to move up a few lanes before the screen updates the lanes.

Now, make the lane change a little smoother, instead of abruptly jumping when the player moves from lane to lane.
(this prompt made a huge bug)

The change you just made created a huge bug. Now, when a new lane is supposed to generate, every existing lane just shifts down one and the 'new' lane is just black, and this continues until you can't even see your own icon anymore, he's shifted down too much.

It still doesnt work, and now the player appears to move up to two lanes at a time but is killed by something not in his lane. Take a deep look at the code and find the bugs with the camera movement/lane generation/player position.

(After this prompt, the bug still wasn't fixed and I ran out of free messages. I downloaded the last working version of the file and uploaded to github and made a github page for it.)

