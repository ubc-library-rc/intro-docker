---
layout: page
title: Paths to installation and troubleshooting 
permalink: /install/
parent: Part 2 - Technical Overview
nav_order: 1
---

# Get started with Docker Desktop

Beyond exploring [Docker Hub's Playground](https://labs.play-with-docker.com/) in the browser environment, the next easiest step for Mac and Windows user is installing **Docker Desktop** for your operating system. 

On both operating systems, for the purposes of our workshop attendees, it is best to choose **Stable** versions of Docker Desktop over **Edge** versions, which are better suited to experienced developers.
{: .warn}

Check out the [Docker Quickstart training module](https://docs.docker.com/get-started/) for useful information pertaining to getting started on both operating systems.

### Docker Desktop for Windows

[Here](https://docs.docker.com/docker-for-windows/install/) you'll find the installation guide for Windows. 

Basic installation requirements for Windows include *Windows 10 64-bit: Pro, Enterprise, or Education (Build 16299 or later)*, *64-bit processor with [SLAT](https://en.wikipedia.org/wiki/Second_Level_Address_Translation) functionality*, *[Enabling Hyper-V](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v)*, *[Enabling Containers](https://docs.microsoft.com/en-us/virtualization/windowscontainers/quick-start/set-up-environment?tabs=Windows-10-Client)*, *virtualization support set in BIOS*, and *at least 4 gb of RAM*.

Docker Desktop also provides further documentation on [how to get started on Windows](https://docs.docker.com/docker-for-windows/) after installation, as well as a dedicated [troubleshooting page for Windows](https://docs.docker.com/docker-for-windows/troubleshoot/).

### Docker Desktop for Mac

[Here](https://docs.docker.com/docker-for-mac/install/) you'll find the installation guide for Mac. 

Basic installation requirements for Mac include a *computer release year of 2010 or newer*, *macOS version 10.13 or newer*, and *at least 4 gb of RAM*.

Keep in mind that there are multiple pathways to install and interact with Docker on Mac, and as the install page flags early, some of these may conflict with one another. 
{: .warn}

Check out, for example, how [Docker Desktop compares with Docker Toolbox](https://docs.docker.com/docker-for-mac/docker-toolbox/) on Mac.

Docker Desktop also provides further documentation on [how to get started on Mac](https://docs.docker.com/docker-for-mac/) after installation, as well as a dedicated [troubleshooting page for Mac](https://docs.docker.com/docker-for-mac/troubleshoot/).

# What About Linux?

Unsurprisingly, there is no "Docker Desktop" for Linux- those Desktop applications were designed in part as a workaround on Windows and Mac for the Linux-native operations of Docker itself.

The Docker documentation guide gives [instructions for installation on multiple Linux distros](https://docs.docker.com/engine/install/#server), including [CentOS](https://docs.docker.com/engine/install/centos/), [Debian](https://docs.docker.com/engine/install/debian/), [Fedora](https://docs.docker.com/engine/install/fedora/), and [Ubuntu](https://docs.docker.com/engine/install/ubuntu/). Note that each distro's installation page lists any specific requirements or constraints.

If you're an experienced Linux user and/or particularly brave, there are also instructions to [Install Docker Engine from binaries](https://docs.docker.com/engine/install/binaries/).