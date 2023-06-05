| [![Teams](teamsb.png)]() |


**One task:** Pick the object, shake it, put it back. As many times as possible, as successfully as possible.

**Two strategies:** Vision based or Tactile based.

**Task A**

Mr White robot arm, with gripper.

(add tactile sensors on the gripper, QMUL, or a camera, UCL)

The target object sits on the table, within the arm workspace.

The arm moves to a random joints-space configuration (taken from a list of valid/safe configurations near to the table surface, gripper about 5 cm over the table).

__“Local exploration”__ starts. 
(This is the part of the code that students will have to update in the Hackathon; in the initial baseline we provide, the robot does nothing, or does something very simple.)

The gripper closes. 
The arm moves up to a fixed configuration, with the gripper at about 15 cm over the table.
Gentle shaking.
The arm moves back to a random/valid configuration near to the table.
Gripper opens.
The arm moves back to home configuration.


We will follow the below schedule:

* 9:30-10:00 Welcome and Introduction
Lorenzo will introduce the idea/objective of the SS, and explain the task.

Participants will be asked to make “teams”, as cross-affiliation as possible. Teams could be 4-6 people each.
A total of 8 teams (4 vision, 4 tactile) would be a good number.
For example, 4*8=32, 5*8=40, 6*8=48… this should match the expected number of participants.


* 13:00-15:30 Mini-Hackathon (part #1): code my robot (can you beat the baseline?)
Teams work on the code and test their solutions.
* 16:00-17:30 Mini-Hackathon (part #2): presentation of results and closing.
Knock-out games. How many objects can you pick&shake in 3 minutes. 1 point for each object contact,  2 points for each object pick, 3 points for each shake with no object fall.
One winner in each league (vision/tactile), and one overall winner of the FINAL game (vision VS tactile).


**Other possible tasks:**
* B: (tactile/visual) exploration
* C: haptic object recognition.

**Task B**
Mr White robot arm, with gripper. (add tactile sensors on the gripper, QMUL, or a camera, UCL)
The target object sits on the table, within the arm workspace.
The arm moves to a random joints-space configuration (taken from a list of valid/safe configurations near to the table surface, gripper about 5 cm over the table).
__“Exploration” starts.__
(This is the part of the code that students will have to update in the Hackathon; in the initial baseline we provide, the robot does what is written below)

At the beginning, all configurations have the same probability of being selected.
* step-1) One valid arm configuration is chosen from the list, based on probabilities.
* step-2) The arm moves to such a configuration, and depending on touch/no-touch (or, visual feedback), the probability of the configuration is updated (either decreased or increased).
Step-1 and step-2 are repeated for N number of times (e.g. N=1000); 
probabilities are reset; 
a new exploration starts.



**Task C** (last resort, if MrWhite does not work)
Robotiq adaptive gripper, with one 2x2 flat tactile sensor (empty soft pad on the other side).
Gripper is open (fixed on the desk).
One object (among 10) is placed within the fingers.
Gripper closes and applies a "squeezing strategy" to recognize object.
Gripper opens.
