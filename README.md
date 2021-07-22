# bebop_simulator
A ROS package that simulates the Parrot Bebop. It also contains an implementation that simulates landing platforms that move with constant speed.

It is part of a ROS eco-system of packages that allow an autonomous UAV to land on a moving platform, using only a front-facing camera.
You can see a tutorial [here](http://wiki.ros.org/Tutorials/Landing%20an%20autonomous%20UAV%20on%20a%20moving%20platform%20using%20only%20a%20front%20facing%20camera).

# Dependecies:

* [hector_quardrotor_interface](https://github.com/tu-darmstadt-ros-pkg/hector_quadrotor.git)
* [hector_pose_estimation](https://github.com/tu-darmstadt-ros-pkg/hector_localization.git)
* [hector_gazebo_plugins](https://github.com/tu-darmstadt-ros-pkg/hector_gazebo.git)
* [realsense_gazebo_plugin](https://github.com/pal-robotics/realsense_gazebo_plugin.git)
* [twist_mux]
* [geographic_msgs]



## Installation procedure
Install twist_mux and geographic_msgs packages through apt.

``` 
sudo apt install ros-ROS_DISTRO-twist-mux
sudo apt install ros-ROS_DISTRO-geopgraphic-msgs

```
Clone bebop_gazebo package and its dependencies into your catkin_ws and then build it.:

``` 
cd your_catkin_ws/src
git clone https://github.com/tu-darmstadt-ros-pkg/hector_quadrotor.git
git clone https://github.com/tu-darmstadt-ros-pkg/hector_localization.git
git clone https://github.com/tu-darmstadt-ros-pkg/hector_gazebo.git
git clone https://github.com/pal-robotics/realsense_gazebo_plugin.git
cd .. && catkin build
source your_catkin_ws/devel/setup.bash

```