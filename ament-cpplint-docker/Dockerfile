ARG UBUNTU_VERSION
FROM ubuntu:${UBUNTU_VERSION}

ARG ROS2_VERSION

RUN apt update \
        && apt install --no-install-recommends -y \
        ros-${ROS2_VERSION}-ament-cpplint \