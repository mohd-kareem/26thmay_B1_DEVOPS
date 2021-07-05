# TASK 1
 ### update apt package
 $ sudo apt-get update
 
~$ sudo apt-get install \apt-transport-https \ca-certificates \curl \gnupg \lsb-release
 
 ### add GPG key
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

### stable repo
~$ echo \
  "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
  
  ### Install Docker Ingine
 $ sudo apt-get update
 $ sudo apt-get install docker-ce docker-ce-cli containerd.io
  

# TASK 2
### pull ubuntu:20.04 docker image
$ docker pull ubuntu:20.04


# TASK 3
## Docker Operations
### sleep
$ docker run ubuntu:20.04 sleep 20
### stop
$ docker stop nervous_ptolemy
### start
$ docker start nervous_ptolemy
### pause
$ docker pause nervous_ptolemy



#TASK 4 
### get bash shell of that container
$  docker exec -it nervous_ptolemy /bin/bash
