# Docker and microservices workshop 

## What is Docker?
Docker is a platform for developers and sysadmins to build, run, and share applications with containers. The use of containers to deploy applications is called containerization. Containers are not new, but their use for easily deploying applications is. Source:[Docker Docs](https://docs.docker.com/get-started/). 

## What is a container?
Fundamentally, a container is nothing but a running process, with some added encapsulation features applied to it in order to keep it isolated from the host and from other containers.
![Docker arrchitecture](https://docs.docker.com/images/Container%402x.png)

## Installation

First of all you need to install Docker, the steps will depend on your OS:

### Windows 
**note:** You need Windows 10 Pro, Enterprise or Education (tip: if you have an educational email email, you are elegible to have a Windows 10 Education license)

**update:** Windows 10 home is now supported but you need to update to 2004 release an enable [wsl2](https://docs.microsoft.com/en-us/windows/wsl/wsl2-index).

* In my opinion,  the easiest way to install doccker in windows is using [chocolatey](https://chocolatey.org/packages/docker-desktop/2.3.0.4)

* The second method to install directly from [Dockerhub](https://docs.docker.com/docker-for-windows/install/)

* A third alternative is to install a linux virtual machine (any distro) and install docker on it.

### Mac OS

* you can install Docker from [Dockerhub](https://docs.docker.com/docker-for-mac/install/)

### Linux

The installation on Linux has variations according to the distribution,  there is an [installation page](https://docs.docker.com/engine/install/) with instructions for the more pupular distributions.

After the installations you should run some [configuration steps](https://docs.docker.com/engine/install/linux-postinstall/) to secure your docker execution

## Testing the installation

A successfull docker installation can be tested in two ways:

1. On a terminal execute  `docker -v` or `docker --version` you should get an output like:

![output version](http://i.imgur.com/EUKqOL2l.png)

2. On a terminal execute: `docker run hello-world` you should get an output like:

![output hello-world](https://i.imgur.com/sDAHnAC.png)


## Using an interactive container

Now let's use an interactive nodeJs container, for this we will use the command:  `docker run -it node`. There is an example of couple of code lines.

![output interactive node](https://i.imgur.com/vBHibYM.png)
