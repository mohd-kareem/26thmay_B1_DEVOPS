# TASK 1
 ## update apt package
 $ sudo apt-get update
 $sudo apt-get install \apt-transport-https \ca-certificates \curl \gnupg \lsb-release
 
 ## add GPG key
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
