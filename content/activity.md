---
layout: page
title: Learning activities
permalink: /activity/
parent: Part 2 - Technical Overview
nav_order: 3
---

# Hands-on Learning Activities

![Doing a Docker Install](/figures/dockerinstall.png)

### Dockerfiles Lifecycle

First we want to explore a bit more about the lifecycle of a Dockerfile.

In almost all use cases, you will not need to write a Dockerfile yourself, but can instead select one from a trusted Docker Registry.

The main registry used by most people is [Docker Hub](http://hub.docker.com), which provides a Github-like management platform for sharing Docker images. Additionally, Docker Hub curates "Official Images" for many popular programs and use cases.

Let's navigate together to the [Official Jekyll Docker Image](http://hub.docker.com/r/jekyll/jekyll/tags) to look into how these image's lifecycles are maintained, and how *tags* can specifically help us choose the best image for any given use case.
<br/>

<!---
### Installing Docker/Q&A

Even though mastering Docker can help you solve the many environment and dependency issues you'll come across in computing, getting Docker itself running on any given system can be quite a challenging task initially!

First, we're going to check in on everyone's install status, to see who already has Docker installed. (No worries if you don't, it's not required- just gaining an understanding of our experience levels!)

Next, if you're interested in getting started with your install *now*, we'll allot this time to step through [the first steps of installation, as designated here](install.md), and to answer any questions that arise when reviewing these instructions.

Additionally, [this thorough guide](https://www.ezzeddinabdullah.com/posts/penguins-in-docker-a-tutorial-on-why-we-use-docker) was just published yesterday, walking through the basics of Docker up to creating Dockerfiles from a data engineering perspective!
--->