
**One task:** Pick the object, shake it, put it back. As many times as possible, as successfully as possible.

**Two strategies:** Vision based or Tactile based.

### **Task**

We present you Mr White robot arm with gripper. We have two configurations: one with _tactile sensors_ on the gripper; the other one with _a camera_ attached to the gripper. 

The target object sits on the table, within the arm workspace.

The arm moves to a random joints-space configuration (taken from a list of valid/safe configurations near to the table surface, with gripper about 5 cm over the table).

_“Local exploration”_ starts. 

(This is the part of the code that the teams will have to update in the Hackathon; in the initial baseline we provide, the robot moves only.)

You are expected to update the provided code so that the gripper performs the tasks as below:

- The gripper finds the object.

- The gripper positions itself to perform the grasping. 

- The gripper closes and grasps the object. 

- The arm moves up to a fixed configuration, with the gripper at about 15 cm over the table.

- Gentle shaking.

- The arm moves back to a random/valid configuration near to the table.

- Gripper opens.

- The arm moves back to home configuration.


***Your code:***

Create a ROS node that reads the information provided by the input node. By reading this information, the node should also move the arms to a position that would enable grasping the object. The code we provide performs the grasping and shaking. 

- Pay attention to the functions:

```js
// Javascript code with syntax highlighting.
get_angles = rospy.ServiceProxy("get_joint_angles", GetAngles) 
set_angles = rospy.ServiceProxy("set_joint_angles", SetAngles)
```


- You need to read the service file in order to get information from the sensor

- Update the launch file to activate the node you have created. 

Your _rqt_graph_ should look like this: 


---


**TEAMS:**

[![Teams](teamsb.png)]() 


