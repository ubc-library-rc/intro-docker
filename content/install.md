---
layout: page
title: Paths to installing Docker
permalink: /install/
parent: Part 2 - Technical Overview
nav_order: 1
---

# Paths to installing Docker

## Linux 

As Docker's design builds upon, and extends, the logic of Linux computing structures, Docker tooling is relatively well-integrated with mainstream Linux distributions.

The Docker documentation guide gives [instructions for installation on multiple Linux distros](https://docs.docker.com/engine/install/#server), including [CentOS](https://docs.docker.com/engine/install/centos/), [Debian](https://docs.docker.com/engine/install/debian/), [Fedora](https://docs.docker.com/engine/install/fedora/), and [Ubuntu](https://docs.docker.com/engine/install/ubuntu/). *Note that each installation page lists specific requirements or constraints for that distro*.

If you're an experienced Linux user on a unique distro not included above, there are also instructions to [Install Docker Engine from binaries](https://docs.docker.com/engine/install/binaries/).

![Docker whale made with lego](/content/figures/docker_lego.jpg)
Docker lego whale retrieved from [kyohei ito on Flickr](https://www.flickr.com/photos/134416355@N07/31518965950), [CC BY-SA 2.0](https://creativecommons.org/licenses/by-sa/2.0/).

## Windows and Mac

Beyond exploring [Docker Hub's Playground](https://labs.play-with-docker.com/) in the browser environment, the next easiest step for Mac and Windows user is installing **Docker Desktop** for your operating system. 

On both operating systems, for the purposes of our workshop attendees, it is best to choose **Stable** versions of Docker Desktop over **Edge** versions, which are better suited to experienced developers.
{: .warn}

Check out the [Docker Quickstart training module](https://docs.docker.com/get-started/) for useful information pertaining to getting started on both operating systems.

### Windows - Install

[Here](https://docs.docker.com/docker-for-windows/install/) you'll find the installation guide for Windows. You can also navigate to [this direct installation link for Windows Home edition](https://docs.docker.com/docker-for-windows/install-windows-home/). 

Basic installation requirements for Windows include *Windows 10 64-bit: Pro, Enterprise, or Education (Build 16299 or later)*, *64-bit processor with [SLAT](https://en.wikipedia.org/wiki/Second_Level_Address_Translation/) functionality*, *[Enabling Hyper-V](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v/)*, *[Enabling Containers](https://docs.microsoft.com/en-us/virtualization/windowscontainers/quick-start/set-up-environment?tabs=Windows-10-Client/)*, *virtualization support set in BIOS*, and *at least 4 gb of RAM*.

### Windows - Get Started

Docker Desktop also provides further documentation on [how to get started on Windows](https://docs.docker.com/docker-for-windows/) after installation, as well as a dedicated [troubleshooting page for Windows](https://docs.docker.com/docker-for-windows/troubleshoot/).

In particular, enabling virtualization on Windows 10 can vary between editions and devices. Here are a few links that can help you get started if you're encountering this issue:

* If you're using Windows 10 Pro, Education, or Enterprise, you can [enable virtualization using Hyper-V, as described here](https://docs.microsoft.com/en-gb/archive/blogs/canitpro/step-by-step-enabling-hyper-v-for-use-on-windows-10)
* If you're using Windows 10 Home on an HP computer, [these instructions will work for you to enable virtualization](https://thewebspark.com/2019/04/02/how-to-enable-virtualization-in-bios-of-windows-10-home-hp-systems-solved/)
* If you're using Windows 10 Home on another computer, you can adapt the virtualization-specific steps from the link above once you determine which keys you must press to enter BIOS on your computer, [using this guide based on hardware manufacturers](https://www.tomshardware.com/reviews/bios-keys-to-access-your-firmware,5732.html)

### Mac - Install

[Here](https://docs.docker.com/docker-for-mac/install/) you'll find the installation guide for Mac. 

Basic installation requirements for Mac include a *computer release year of 2010 or newer*, *macOS version 10.13 or newer*, and *at least 4 gb of RAM*.

Keep in mind that there are multiple pathways to install and interact with Docker on Mac, and as the install page flags early, some of these may conflict with one another. 
{: .warn}

Check out, for example, how [Docker Desktop compares with Docker Toolbox](https://docs.docker.com/docker-for-mac/docker-toolbox/) on Mac.

### Mac - Get Started

Docker Desktop also provides further documentation on [how to get started on Mac](https://docs.docker.com/docker-for-mac/) after installation, as well as a dedicated [troubleshooting page for Mac](https://docs.docker.com/docker-for-mac/troubleshoot/).

Once you have Docker tools installed on your computer of choice, you can check out our [extended learning resources](resources.md) for further useful documentation and tutorials.
