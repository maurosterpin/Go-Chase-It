# Go Chase it!
Simple ROS robot which chases a white ball.
This project is a part of the Udacity Robotics Software engineer nanodegree

If a white ball is within the robot's field of view it checks whether it's in the left, center or right part of the image and moves accordingly.
If a white ball isn't within it's field of view it stops moving.


https://user-images.githubusercontent.com/92162018/203051303-03deba21-317e-4cb6-b6df-01958d869f95.mp4


### Installation instructions
Installation requires Ubuntu with ROS installed

Clone this repository then open it in a terminal and run catkin_make.

Then open 3 new terminals and run following commands:

1- Launch the robot inside your world (starts up the simulation in gazebo)
```
$ cd catkin_ws/
$ source devel/setup.bash
$ roslaunch my_robot world.launch
```

2- Run drive_bot and process_image (exeutes ball_chaser.launch, which will track the ball and move the robot)
```
$ cd catkin_ws/
$ source devel/setup.bash
$ roslaunch ball_chaser ball_chaser.launch
```

3- Visualize (**optional**, launches the camera view)
```
$ cd catkin_ws/
$ source devel/setup.bash
$ rosrun rqt_image_view rqt_image_view
```






