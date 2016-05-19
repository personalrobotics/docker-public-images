#
# Makefile to build a docker image with the specified name.
#
NAME="personalrobotics/ros-openrave"

build: Dockerfile
	docker build -t $(NAME) .

clean:
	docker rmi $(NAME)
