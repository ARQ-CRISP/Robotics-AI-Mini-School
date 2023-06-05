
**One task:** Pick the object, shake it, put it back. As many times as possible, as successfully as possible.

**Two strategies:** Vision based or Tactile based.

### **Task**

We present you Mr White robot arm with gripper. We have two configurations: one with _tactile sensors_ on the gripper; the other one with _a camera_ attached to the gripper. 

The target object sits on the table, within the arm workspace.

The arm moves to a random joints-space configuration (taken from a list of valid/safe configurations near to the table surface, with gripper about 5 cm over the table).

_“Local exploration”_ starts. 

(This is the part of the code that teams will have to update in the Hackathon; in the initial baseline we provide, the robot only does simple things.)

The gripper closes. 

The arm moves up to a fixed configuration, with the gripper at about 15 cm over the table.

Gentle shaking.

The arm moves back to a random/valid configuration near to the table.

Gripper opens.

The arm moves back to home configuration.

[![Teams](teamsb.png)]() 


