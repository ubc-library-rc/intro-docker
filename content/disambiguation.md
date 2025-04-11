---
layout: default
title: Disambiguating Docker Terms
permalink: /disambiguation/
parent: Part 1 - What's Docker?
nav_order: 3
---

# So many 'Dockers', so little time

One of the first barriers in learning Docker is identifying all the elements of its ecosystem, many of which share the same core name. This walkthrough aims to disambiguate those pieces of the puzzle.

![What's Docker meme](/content/figures/whatsdocker.png)

Docker operates using a client-server setup, where the Docker client can connect to the Docker host either locally or remotely. Both the Docker client and host (daemon) can reside on the same machine, or they can be on separate systems and communicate through sockets or a REST API.

The **Docker client** serves as the primary means of interaction for many Docker users. By issuing commands such as "docker run", the client sends instructions to the **Docker daemon** which then executes them. The **Docker API** is used by the Docker command (CLI). It is possible for the Docker client to connect with multiple daemons simultaneously

## Docker Engine

[Docker Engine](https://www.docker.com/products/container-runtime) can be thought of, appropriately enough, as the "engine" upon which Docker images and their resulting containers are run. 


Built on [containerd](https://containerd.io/) and robustly interoperable across systems, this is the "main event" of Docker, with three main subcomponents:

#### dockerd Daemon

[dockerd](https://docs.docker.com/engine/reference/commandline/dockerd/) is the name for the persistent process, or *daemon*, behind the Docker Engine. This is also sometimes referred to as the Docker client.

#### Docker CLI

[Docker CLI](https://docs.docker.com/engine/reference/commandline/cli/) is the command line interface that you run in a terminal or shell with the simple command 'docker'. Following Linux norms, once you have Docker CLI installed you can enter 'docker help' to view its [man page](https://en.wikipedia.org/wiki/Man_page), or list of available commands and options.

#### Docker API

[Docker Engine API](https://docs.docker.com/engine/api/) is a Representational State Transfer Application Programming Interface, or a [REST API](https://ubc-library-rc.github.io/intro-api/content/01_what-is-an-api.html#restful-apis). 

This makes it easier for programmers to build applications which interface with Docker Engine. Learn more about [Web APIs here](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Introduction).

## Docker Desktop

[Docker Desktop](https://www.docker.com/products/docker-desktop) is a desktop application available for MacOS or Windows, to provide an easier workflow for the Linux-centric Docker ecosystem.

## Docker Apps

[Docker App](https://docs.docker.com/app/working-with-app/) provides Docker Engine's CLI with a plug-in allowing the 'docker app' command to essentially containerize app development, making it simpler to build the Docker workflow into application development.

## Docker-Compose

Docker-Compose is the most frequently used tool across environments for more complex interaction with Docker Apps. Check out the [Compose documentation](https://docs.docker.com/compose/) for more.

## Docker Hub

[Docker Hub](https://www.docker.com/products/docker-hub) is the most prominent of available registries for exploring and sharing container images, kind of like [Github](https://www.github.com) for Docker.

## Docker Swarm

Rather than a tool or platform, [Docker Swarm, or swarm mode](https://docs.docker.com/engine/swarm/), is exactly what it sounds like: central management of a cluster of Docker Engines controlled through Docker CLI.

![Docker Swarm isn't that widely adopted](/content/figures/dockerswarm.png)


## Docker Platform Beyond Docker Variants

The Docker platform also contains other crucial tooling, not all of which has the name "Docker" in it. One example is [Kubernetes](https://www.docker.com/products/kubernetes), an "orchestration platform" for coordinating shared infrastructure and operations around containers. 

Similarly, [Notary](https://docs.docker.com/notary/getting_started/) is a Docker platform tool which enables users to sign collections of content, verify their integrity, and confirm their origin. 

Finally, [Docker Credential Helpers](https://github.com/docker/docker-credential-helpers/) is a suite of smaller programs to help keep login credentials safe.

# Putting It All Together

If you're still confused about the different moving parts when interacting with Docker, their documentation has a [great diagram of the overall architecture](https://docs.docker.com/get-started/overview/#docker-architecture).
