# class_31
## Docker
With Docker it doesn’t matter if you are using a Mac, Windows, or Linux computer anymore. The entire development environment is isolated: programming language, software packages, databases, and more.

<br>

### Linux Containers

Virtualization has its roots at the beginning of computer science when large, expensive mainframe computers were the norm. How could multiple programmers use the same single machine? The answer was virtualization and specifically virtual machines which are complete copies of a computer system from the operating system on up.
<br>
### Containers vs Virtual Environments
<img src='https://www.backblaze.com/blog/wp-content/uploads/2018/06/bb-bh-VMs-vs.-Containers-3.jpg'/>
Virtual environments are used to isolate Python software packages locally. We can create an isolated box for individual projects so one can use Python 2.7 and Django 1.5 while another can use Python 3.5 and Django 2.1 on the same computer. Virtual environments are great.
<br>
But…virtual environments can only isolate Python packages.

### Install Docker
**sudo pip install docker-compose**
**docker-compose --version**
docker run hello-world. This will download an official image and then run the container.<br>
A good command to inspect Docker is docker info which we can run now. It will contain a lot of output but focus on the top lines which show we now have 1 container which is stopped and 1 image

### Images and Containers
When we ran hello-world we used an official Docker image. We did not have to create the image ourself. But typically we will create custom images and we do so using a Dockerfile. We also will use docker-compose.yml files to run the containers.

A baking analogy we can use here is as follows:

* A Dockerfile is the recipe for a cake
* An image is a snapshot of the recipe at a given time
* A docker-compose.yml says how to make the cake
* And the container is the actual, baked cake

## Library Website and API
### Django REST Framework
Django REST Framework is added just like any other third-party app.
<br> **pipenv install djangorestframework~=3.11.0**
