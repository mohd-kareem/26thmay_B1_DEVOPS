# TASK 1
### what is alpine 
Alpine image is a linux distribution based on musl and BusyBox, designed for security, simplicity, and resource efficiency.It uses OpenRC for its init system and compiles all user-space binaries as position-independent executables with stack-smashing protection.

Because of its small size, it is commonly used in containers providing quick boot-up times it is of only 5MB

# TASK 2
### create a container with name 'example' using ubuntu:20.04 image that should run in background

$ docker pull ubuntu:20.04

$ docker run -d --name example ubuntu:20.04 sleep 500

# TASK 3
### get bash shell in above container

$ docker exce -it example bash

# TASK 4
### create a user test and give password 'q' in runnuing container example

adduser test

root@ea1040473881:/# adduser test

Adding user `test' ...

Adding new group `test' (1000) ...

Adding new user `test' (1000) with group `test' ...

Creating home directory `/home/test' ...

Copying files from `/etc/skel' ...

New password: 

Retype new password: 

passwd: password updated successfully

