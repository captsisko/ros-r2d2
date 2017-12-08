This is a Robot Operating System (ROS) project.

It comprises 2 packages called r2d2_dscription and r2d2_gazebo.

R2d2_description contains a Universal Robot Description Format (URDF) document which uses
XML to create a virtual representation of the R2D2 robot.

R2D2_gazebo contains more files than it's neighbour. It contains a Digital Elevation Model file
(DEM) of landscape from Mongolia. This landscape is used to customize the instance of Gazebo created by r2d2.launch.

Together these packages launch Gazebo and place the DEM file of Mongolia in it.
The r2d2_description URDF robot is then spawned into the customised Gazebo world.

During development both these packages where both under a parent directory called my-robot.
However, as long as they are  placed in the src directory of a catkin workspace and catkin_make is executed, both packages should work just fine.