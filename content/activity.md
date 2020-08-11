---
layout: page
title: Learning activities
permalink: /activity/
parent: Part 2 - Technical Overview
nav_order: 3
---

# Hands-on Learning Activities

Even though mastering Docker can help you solve the many environment and dependency issues you'll come across in computing, getting Docker itself running on any given system can be quite a challenging task initially!

First, we're going to check in on everyone's install status, to see how many folks will be "coding along" with us today.

!["I have no idea what I'm doing" dog](/figures/dockerfile_activity.png)

### Dockerfiles Lifecycle

First we want to explore a bit more about the lifecycle of a Dockerfile.

In almost all use cases, you will not need to write a Dockerfile yourself, but can instead select one from a trusted Docker Registry.

The main registry used by most people is [Docker Hub](http://hub.docker.com), which provides a Github-like management platform for sharing Docker images. Additionally, Docker Hub curates "Official Images" for many popular programs and use cases.

Let's navigate together to the [Official Jekyll Docker Image](http://hub.docker.com/r/jekyll/jekyll/tags) to look into how these image's lifecycles are maintained, and how *tags* can specifically help us choose the best image for any given use case.
<br/>

### Creating a Dockerfile

If we wanted to ensure that a Dockerfile never changed, then pulling one from a public registry would not work for our use case, as they are regularly updated.

With guest contributor Clark Van Oyen from Countable Web Productions, we'll go through the actual content of the Jekyll Dockerfile and what it executes when running on your computer. 

This should provide a better mental model of how containers are constructed from image files, and start you on the path towards writing your own Dockerfiles down the road!

*Thanks to Clark and Countable for guidance on alllll the Docker things, while I constructed this workshop*
![www.countable.ca](/figures/Countable_Logo.png)