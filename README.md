# learn-docker
Docker Learning

Docker:
C:\Gajendra\2017 Gajendra Preparation\Interview Questions\MicroServices\DevOps\Training\DevOps - Containers Docker.docx

Docker and Kubernetes are both important tools in the containerization ecosystem. 
Docker is used for creating and running containers, 
while Kubernetes is used for managing and automating the deployment, scaling, and operation of containers across clusters of hosts.


yum install docker 

- This will install podman docker.
- So we don’t want to go with PODMAN,

- Use CURL

curl -L get.docker.com | sudo bash
![image](https://github.com/gbogguru/learn-docker/assets/42975193/8fb42939-de5d-4692-87a2-6b4f4efa7d77)

After installation of docker, we need to start and enable with the admin rights.

Systemctl start docker

Systemctl enable docker

Docker ps
![image](https://github.com/gbogguru/learn-docker/assets/42975193/c73eecf0-547c-4eab-a503-fef8356faa61)


Docker Binary > Docker Daemon > ContainerD

Note: Need to add usermod
sudo usermod -a -G docker centos

id


- public images will be available at hub.docker.com 

sudo su -

docker pull nginx

docker pull nginx:stable

docker images

docker rmi nginx:stable

Untagged: nginx:stable
Untagged: nginx@sha256:57e42e00530faa65e8acf98c3cf7bf6794093a9841c8a676b6d2fd0a9ba7262f

run is a command to lunch a container

docker run -d nginx 

docker run -d nginx:stable

![image](https://github.com/gbogguru/learn-docker/assets/42975193/cd14e03f-1b29-4747-8bc5-69fda5b6e279)


docker ps

docker images
![image](https://github.com/gbogguru/learn-docker/assets/42975193/b59a07b1-7d72-4d6a-bdb1-0d2edf22233a)

We can use Dockerfile to make images like as JenkinsFile

GO inside a container with exec command
![image](https://github.com/gbogguru/learn-docker/assets/42975193/b6f99530-6a79-48cc-ae92-26d400e14086)


