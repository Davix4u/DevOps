# Opportunities with Docker

Are you aware that as a skilled Docker engineer, you can command an impressive annual salary of up to $80,000? It's true. The allure lies in the profound impact that 
mastering this technology can have on your earning potential.

But what exactly is Docker?

Defined by Google as a lightweight, standalone, executable package of software encompassing all elements necessary for running an application—code runtime, system tools, 
libraries, and configurations—Docker is a game-changer in modern software development.

In simpler terms, Docker is a sophisticated tool for container management.

### Containers, in the Docker realm, are essentially encapsulated images or operating systems derived from Docker images. They provide an isolated environment for applications 
to run seamlessly across different computing environments.

### Docker extends beyond mere application virtualization; it embodies a revolutionary paradigm for virtualizing entire infrastructures, from applications to codebases, with 
dedicated features such as networking, volume management, inspection capabilities, and more.

At the heart of Docker's ecosystem lies Docker Hub—a centralized repository akin to GitHub—where developers can seamlessly access and share Docker images, fostering 
collaboration and accelerating software development cycles.

## who stands to benefit from Docker's prowess?

The answer is clear: virtually anyone involved in modern software development and IT practices. Software engineers leverage Docker to streamline application development and 
deployment. DevOps engineers harness its power for orchestrating continuous integration and continuous deployment (CI/CD) workflows using Docker Compose. Data analysts find 
value in Docker for virtualizing datasets, while cybersecurity experts craft Docker-Hacking labs for vulnerability testing, from static application security testing (SAST) to 
dynamic application security testing (DAST). Even network engineers find utility in Docker's versatility for creating and managing network environments.

In essence, Docker transcends traditional boundaries, empowering professionals across diverse domains to innovate, collaborate, and thrive in the ever-evolving 
landscape of technology.

So, are you ready to embark on your journey with Docker? The opportunities await.

You do not need to memorize this commands, my job is to point us, to how to use these commands

### How to install docker 
www.doc.docker.com

open a docker hub account  hub.docker.com

<img width="945" alt="image" src="https://github.com/Davix4u/DevOps/assets/130823585/1f644e64-0103-44b0-91d1-7dd69374e853">

How to pull for Docker hub 

Command : Docker pull tomcat

<img width="821" alt="Docker pull tomcat" src="https://github.com/Davix4u/DevOps/assets/130823585/a0bcb2ba-5645-4fa9-ace1-ea84ba578f7b">

To find the images : Docker --help  

<img width="917" alt="Docker --help" src="https://github.com/Davix4u/DevOps/assets/130823585/91e42658-4551-4d3a-9cb4-621e9534242c">

Docker images 

To list all the container running in the environment
docker ps -a

<img width="577" alt="docker ps -a" src="https://github.com/Davix4u/DevOps/assets/130823585/5062d46f-bf0b-43cc-a9d4-4ef4518eda0d">

to remove images ; docker rmi tomcat 

<img width="773" alt="docker rmi images" src="https://github.com/Davix4u/DevOps/assets/130823585/2b137239-5183-4586-8955-4197858bbd68">

Note if you do not have an images, you cannot run a container .  if you don't stop a container, you cannot delete a container or remove an image

Let's pull a Centos operating system

Docker pull centos 

<img width="502" alt="docker pull centos" src="https://github.com/Davix4u/DevOps/assets/130823585/74547d38-facb-4d42-8684-87ecf697f6b6">

Docker images centos

<img width="671" alt="docker images centos" src="https://github.com/Davix4u/DevOps/assets/130823585/a81c5a41-b25d-46e8-a761-85133f2333ac">

To run container 
docker run --help

<img width="880" alt="docker run --help" src="https://github.com/Davix4u/DevOps/assets/130823585/bc2be062-1373-47b5-9d94-a9a2dfaef514">

i means interactive , t means allocate a psceutte-tty #to remove d docker 
we re running the container in  -it

docker run -it centos 

<img width="269" alt="docker -run cent" src="https://github.com/Davix4u/DevOps/assets/130823585/02820dfd-5fe2-4693-b037-feac487cae7f">

we can see, we re inside centos
<img width="436" alt="cat centos" src="https://github.com/Davix4u/DevOps/assets/130823585/2a1126e9-1145-4d11-b77c-e9f8513e4035">

TO remove theb images . we have to first stop the container and delete the container 

Docker ps -a 
<img width="755" alt="docker ps-a cent" src="https://github.com/Davix4u/DevOps/assets/130823585/ff020edd-3529-4828-a47c-df41620a9a69">

to remove a container 
docker rm 077 (conatiner first 3 figure or letter ID)

<img width="755" alt="docker ps-a cent" src="https://github.com/Davix4u/DevOps/assets/130823585/901d516a-5fbd-4fe1-b165-959e3f179aa8">

Confirmination of removing centos container 

<img width="747" alt="confirmation it is removed cent" src="https://github.com/Davix4u/DevOps/assets/130823585/ee84e942-26ff-422f-af6d-15f0ec36fb6a">

let run centos in a bin bash mode or zzsh
docker run -it centos /bin/bash 

<img width="504" alt="centos in binlbash" src="https://github.com/Davix4u/DevOps/assets/130823585/94a637f5-8b03-441f-b4fe-77b78bbbb577">

Note: Always remember always use Docker --help























