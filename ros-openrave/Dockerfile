FROM ros:indigo-ros-base
MAINTAINER Pras Velagapudi <pkv@cs.cmu.edu>
ENV DEBIAN_FRONTEND noninteractive

# Add the personalrobotics APT repository
RUN apt-get update && apt-get install -y curl
RUN sh -c 'echo "deb http://packages.personalrobotics.ri.cmu.edu/public trusty main" \
        > /etc/apt/sources.list.d/personalrobotics.list' \
    && curl https://www.personalrobotics.ri.cmu.edu/files/personalrobotics.gpg | sudo apt-key add -

# Install OpenRAVE and clear cache.
RUN apt-get update \
    && apt-get install -y pr-openrave \
    && rm -rf /var/lib/apt/lists/*
