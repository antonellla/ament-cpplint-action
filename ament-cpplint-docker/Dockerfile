ARG ros2-version
FROM ros:${ros2-version}-ros-base

#ARG ROS2_VERSION

#RUN apt update \
#    && apt install --no-install-recommends -y \
#    ros-${ROS2_VERSION}-ament-cpplint \
#    && ln -s /opt/ros/${ROS2_VERSION}/bin/ament_cpplint /usr/bin/ament_cpplint


#WORKDIR /


#ENTRYPOINT ["/opt/ros/${ROS2_VERSION}/bin/ament_cpplint"]

#ENTRYPOINT ["/usr/bin/ament_cpplint"]


# Container image that runs your code
#FROM alpine:3.10
#FROM ros:humble-ros-base

# Copies your code file from your action repository to the filesystem path `/` of the container
COPY --chmod=777 entrypoint.sh /entrypoint.sh

#RUN chmod +x /entrypoint.sh

# Code file to execute when the docker container starts up (`entrypoint.sh`)
ENTRYPOINT ["/entrypoint.sh"]
