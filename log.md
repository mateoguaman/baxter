# Progress Log

### April 5th, 2018 - April 6th, 2018
---
#### Progress made: 
* Cloned baxter sdk and ran pick and place example
* Created own package called picknplace with same dependencies
* Modified script so that it holds the item in place after picking it up instead of placing it down (using rospy.spin()). 
* Wrote service call that allows to modify the link properties, which include the mass of the object
* Figured out terminal command to get joint states such as effort
#### Notes:
Instructions to run:
1. In new terminal, run ./baxter.sh sim
2. Run roslaunch baxter_gazebo baxter_world.launch
3. In new terminal, run ./baxter .sh sim
4. Run rosrun picknplace ik_pick_and_place_demo.py 
5. To get joint efforts, run in new terminal rostopic echo /robot/joint_states (not sure if ./baxter .sh sim is needed)

The modification of the weight is hard-coded in line 220

#### Future work:
* Add more dynamic way to change the mass of the block instead of hard-coding it
* Include way of detecting the pose of the block instead of hard-coding it when using this to change the mass of the block

#### Hours worked:
Start: April 5th, 10:09 PM

End: April 6th, 3:06 AM
