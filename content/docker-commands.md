---
layout: page
title: Docker Commands
permalink: /commands/
parent: Part 2 - Technical Overview
nav_order: 2
---

# Some useful Docker Commands

After installing Docker on your system, to check the installation, you can run the following command:

Input
{: .label .label-green}
~~~
`$ docker --version`
~~~
Output
{: .label .label-yellow}
~~~
`Docker version 18.09.6, build 481bc77`
~~~

Instead of finding docker images through the DockerHub website on your browser, you can use `docker search` in the command line. This command returns the specific information, including image name, description, and official stars.

To pull an image from the DockerHub, you can run the `docker pull` command.

Input
{: .label .label-green}
~~~
docker pull ubuntu
~~~

The tags are used to identify the images inside the Docker hub. If you do not specify a tag, it will use the `:latest` tag by default. To use an older version of Ubuntu, for example `20.04`, you should run the following command:

Input
{: .label .label-green}
~~~
docker pull ubuntu:20.04
~~~

Once the image is downloaded, the `docker run` command is utilized to generate a container based on the image. To keep the container running when you exit the terminal session, the container should be started in a detached mode. This is like running a process in the background.

Input
{: .label .label-green}
~~~
docker run -d ubuntu
~~~

Usually the output of `docker run` command shows the container ID and container name as well as any output generated by the container or error messages.

To list all the running containers on a Docker host, run the following command:

Input
{: .label .label-green}
~~~
`docker ps`
~~~
Output
{: .label .label-yellow}
~~~
CONTAINER ID   IMAGE           COMMAND                  CREATED          STATUS          PORTS     NAMES
de11dedbd972   ubuntu:latest   "/bin/sh -c 'echo Co…"   14 minutes ago   Up 14 minutes              naughty_faraday
~~~

This command will display a table with information about the active containers, including their container ID, image name, status (running, stopped, etc.), creation time, and port mappings. By default, `docker ps` only shows the running containers. If you want to see all containers (including the ones that have exited), you can use the `docker ps -a` command. 

When you run a Docker container, it will continue to run until it completes its execution or until it is explicitly stopper or terminated. `docker stop` command stops a container peacefully while `docker kill` immediately kills its execution. 

Downloading images and running containers can quickly fill up disk space. `docker rmi` followed by the images id is used to remove the image while `docker rm` followed by container name or id is used to remove containers. 