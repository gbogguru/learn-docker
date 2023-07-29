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

docker ps
docker images

We can use Dockerfile to make images like as JenkinsFile


