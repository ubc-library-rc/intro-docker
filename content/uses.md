---
layout: default
title: Main Use Cases
permalink: /uses/
parent: Part 1 - What's Docker?
nav_order: 2
---

# What is Docker useful for?

Docker lets you create *static* and *reproducible* environments, saved into an image which will run the same way on any computer with Docker set up ([agnostic](https://www.techopedia.com/definition/31685/hardware-agnostic) to hardware and operating system).

Docker has a number of useful qualities which apply across all industries and applications:

* **"things just work"** - once you've covered the initial learning curve for virtual containers, the process of interacting with them stays consistent
* **no more struggling for dependencies** - you can include all libraries, packages, and dependencies that a piece of software or a dataset needs in an accompanying Docker image, so it will work 'right out of the box' for its recipient
* **enables reproducible computing** - when sharing software, research, or other data, you can provide a Docker image to ensure your recipients do not have to scramble to duplicate the development environment in which it can work most optimally. Additionally, when others create containers from your Docker image, any actions they take within that container will not alter the original Docker image for others.

Across use cases, Docker essentially provides most of the benefits of Virtual Machines, but it's much faster and easier to spin up a new Docker container from an image than it is to set up a virtual machine. 

[Some developers argue](https://countable-ops-manual.readthedocs.io/devops/WHY_DOCKER.html#think-git-for-dev-environments) that Docker is a successful "environment version management system" in parallel to [Git](https://ubc-library-rc.github.io/intro-git/) as a "file version management system."
<br/>

### Use cases for academia

Whether you're conducting research or creating software outputs, setting up a Docker workflow can ensure that your scripts are *readable*, *usable*, and can be easily opened and explored by others.

Academics using containers for reproducible computing must maintain vigilance around data privacy and security in these workflows. Check out the [Resources section on Docker security](https://ubc-library-rc.github.io/intro-docker/resources/#docker-security).

Additionally, there's clearly a learning curve for onboarding to Docker, which will impact academic collaboration. However, that learning curve is likely preferable to the existing state of 'reproducible computing' in which we have to manually document myriad workarounds for our peers and colleagues.
<br/>

### Use cases for programmers

Programmers spend a lot of their time filling in the gaps for environmental dependencies. In a coder's workflow, the majority of little details that go wrong when trying to execute code relate to missing packages in your computing environment.

Remember, computers are very smart in a few specific ways, but they lack a lot of elements of what humans would consider "common sense." A computer will query exactly where it expects files to be, and will usually stop in its tracks if it cannot locate necessary dependencies.

By centralizing all necessary files to related Docker images for a code repository, programmers can include that image *within* the repository folder itself, and simply run a Docker command [usually 'docker-compose up' or 'docker-compose run filename'] upon navigating into the folder to begin working on it.
<br/>

### Use cases for developer operations

Developer operations, or [DevOps](https://resources.collab.net/devops-101/what-is-devops), is the combination of software development and real-world deployment. The main problem DevOps arose to solve is the threat of inconsistency when updating already-deployed software projects.

By designing a consistent workflow which utilizes more complex Docker tooling (like Swarm and Kubernetes, covered briefly in [Docker Disambiguation](disambiguation.md)), DevOps practitioners can ensure low or zero "downtime" for their active projects. This fits perfectly with the DevOps methodology of [CI/CD](https://www.atlassian.com/continuous-delivery/principles/continuous-integration-vs-delivery-vs-deployment), which stands for "Continuous Integration & Continuous Delivery/Deployment".
<br/>



