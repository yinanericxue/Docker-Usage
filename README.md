# Docker Usage

#### Docker Use Case 1

#### forward vs backward compatibility
#### forward = without hardware upgrade, able to support future software upgrades (2020 macbook pro supporting mac os in 2025, aka future-proof)
#### backward = ubuntu 22.04 kernel able to support lib & bin & others from ubuntu 20.04

#### Docker Image - Ubuntu
#### https://hub.docker.com/_/ubuntu

#### docker pull ubuntu:20.04
#### docker image ls

#### docker run ubuntu:20.04 ls (run a command after starting the container and then exit)
#### docker run ubuntu:20.04 cat /etc/issue
#### docker run ubuntu:20.04 pwd
#### docker run ubuntu:20.04 (no command after starting the container, so exit)

#### docker run --name test1  -it ubuntu:20.04 /bin/bash
#### docker run --name test2  -it ubuntu:20.04 /bin/bash
#### https://docs.docker.com/engine/reference/commandline/run/

![image](https://github.com/yinanericxue/Docker-Usage/assets/102645083/92f6e35c-ddf1-4402-bdcb-9e73ffa168f9)
![image](https://github.com/yinanericxue/Docker-Usage/assets/102645083/c80e3084-9f47-4eab-9c3a-48f602171448)



![image](https://github.com/yinanericxue/Docker-Usage/assets/102645083/bc6249ec-8890-40d6-b9ca-812f55b95194)

![image](https://github.com/yinanericxue/Docker-Usage/assets/102645083/c113f327-94b5-46c8-8a3d-d749f728e4f9)

![image](https://github.com/yinanericxue/Docker-Usage/assets/102645083/f7b96884-b89a-4b6f-8719-c9c05ea23fd5)





####  Docker Use Case 2

#### NGINX
#### https://www.papertrail.com/solution/guides/nginx/
![image](https://github.com/yinanericxue/Docker-Usage/assets/102645083/9e1b728d-e07f-429d-bf51-f3e64366f277)


#### Create a Web Server by using NGINX
#### https://docs.docker.com/engine/reference/commandline/run/
#### https://www.baeldung.com/linux/nginx-docker-container

#### docker pull nginx
#### docker pull nginx:latest
#### docker pull nginx:1.24.0 # if selecting specific version

#### docker image ls

#### docker run -d -p 8000:80 nginx  # it's converting from 8000 (host port number) to 80 (container port number)

