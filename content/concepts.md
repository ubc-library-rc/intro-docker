---
layout: default
title: Origins and High Level Concepts
permalink: /concepts/
parent: Part 1 - What's Docker?
nav_order: 1
---

# Origins of containerization

Docker itself is incredibly "young," as it was first launched to the open source development community in 2013. However, containers pre-date Docker as a norm for isolating environments in Linux. 

While Docker built upon the pre-established Linux concepts surrounding containers and virtualization, the platform's persistent centralization of related tooling began to deeply impact technology deployment norms. 

Now, instead of learning all the low-level minutia of customizing containers in Linux, developers just needed to get Docker running, and they could create Docker containers from a number of different interfaces.

# Virtualization concepts
This section will introduce a few concepts and terms for you to be aware of before we dive into the specifics of Docker.

Cover [namespaces](https://docs.docker.com/get-started/overview/#namespaces) and [control groups](https://docs.docker.com/get-started/overview/#control-groups)
{: .warn}


### Virtualization in computing

TODO type from written notes
{: .warn}

### Virtual machines (VMs)

Virtual Machines (VMs) virtualize the entire "tech stack" of a computer, down to the hardware. They're a lot more resource-intensive than containers but can be necessary for certain computing tasks. 

### Containers

Whereas a VM gives us virtualization all the way down to the kernel and hardware layers, a container is much more lightweight in comparison, sitting on top of the host computer's kernel and merely virtualizing from the level of binaries and libraries upward. 

![Containers versus VMs](figures/containersvsvm.png)

TODO type rest from written notes
{: .warn}

#### Docker objects

Discuss the difference between **images**, **containers**, and **services** as per [their docs breakdown](https://docs.docker.com/get-started/overview/#docker-objects).
{: .warn}
