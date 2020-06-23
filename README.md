# Seawolf-8-Software
This repository contains the ROS powered code that runs on Seawolf-8, an autonomous submarine built by North Carolina State Universities underwater robotics club.

## Important ROS Topics
The following is a list of major ROS topics in this project organized by the package they belong to
### wolf_serial
* wolf_twist
    * contains geometry_msgs/Twist messages that set the sub's linear (up, forward, left, etc.) and angular (pitch, roll, yaw) velocities
* wolf_imu_euler
    * contains Vector3 messages that describe the subs orientation using euler angles
    

## Running ROS Tests
To run the tests, use this command

`rostest PACKAGE TEST`

most commonly tests will be "sanity check" tests which check the validity of topic IO of nodes within a package, these can run like this:

`rostest wolf_serial sanity_checks.test`