FROM ros:melodic

RUN apt -y update && apt -y upgrade

# Create catkin_ws
RUN mkdir -p /home/catkin_ws/src && cd /home/catkin_ws/src && \
    /bin/bash -c "source /opt/ros/melodic/setup.bash; catkin_init_workspace" && \
    cd /home/catkin_ws && \
    /bin/bash -c "source /opt/ros/melodic/setup.bash; catkin_make" && \
    echo "source /home/ros_catkin_ws/devel/setup.bash" >> ~/.bashrc && \
    echo "export ROS_PACKAGE_PATH=\${ROS_PACKAGE_PATH}:/home/catkin_ws" >> ~/.bashrc && \
    echo "export ROS_WORKSPACE=/home/catkin_ws" >> ~/.bashrc

WORKDIR /home/catkin_ws
