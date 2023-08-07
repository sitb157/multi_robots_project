FROM ros:humble-perception-jammy

ARG ROS_DISTRO=humble
RUN apt-get update 
RUN apt-get install -y \
    vim
RUN groupadd -g 999 sitb157 
RUN useradd -r -u 999 -g sitb157 sitb157 
USER sitb157

RUN echo "source /opt/ros/$ROS_DISTRO/setup.bash" >> ~/.bashrc
