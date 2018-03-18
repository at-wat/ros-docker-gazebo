# ROS Kinetic + Gazebo + Rviz on Docker

This package is a demonstration of gazebo + rviz on docker.
Simulated turtlebot is controlled by a gamepad.
docker-compose.yml for Intel and ATI graphic board is also provided.

## Step 1: Install Docker
Install docker https://docs.docker.com/engine/installation/linux/ubuntu/

To run docker without super user:

      sudo groupadd docker
      sudo gpasswd -a ${USER} docker
      sudo service docker restart

## Step 2: Building the container

      docker-compose build

## Step 3: Start the container

      docker-compose up

ros-kinetic-kobuki container often fails because of nodelet load timing.
Try `docker-compose restart ros-kinetic-kobuki` to reload it.


# References

* http://wiki.ros.org/docker/Tutorials/Docker
* http://wiki.ros.org/docker/Tutorials/Hardware%20Acceleration
* http://wiki.ros.org/docker/Tutorials/GUI

