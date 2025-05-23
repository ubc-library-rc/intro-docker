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
<br/>

## Computing concepts

* [application](https://en.wikipedia.org/wiki/Application_software) - the word "app" is widely used to mean many things, but overall it is any program or group of programs targeted towards computer end users

* [binary code](https://en.wikipedia.org/wiki/Binary_code) - referred to in some contexts as [machine code](https://en.wikipedia.org/wiki/Machine_code), these are terms for the instructions sent at the computing level (the information is coded in literal 1s and 0s, hence the term 'binary')

* [kernel](https://en.wikipedia.org/wiki/Kernel_(operating_system)) - in a computer's operating system, the kernel is the central program that holds control over all the other programs, up to the level of applications which the user interacts with

* [instance](https://en.wikipedia.org/wiki/Instance_(computer_science)) - a single running version of something in computing or a concrete occurrence; when I create a container, that is a sole *instance* of that container type, and when I download and setup a piece of software, my local copy is an *instance* of the program

* [library](https://en.wikipedia.org/wiki/Library_(computing)) - this is the set of fixed resources a computer can call upon while executing programs and commands; it's reasonably parallel to an *actual library*, as it's where an active computer obtains things like documentation and sets of routines it can run

* [operating system](https://en.wikipedia.org/wiki/Operating_system) - a computer's operating system is the software which manages the computing hardware and provides a platform for user-facing applications and services

* [process](https://en.wikipedia.org/wiki/Process_(computing)) - this is the term for the current instance of a running computer program

* [provisioning](https://en.wikipedia.org/wiki/Provisioning_(telecommunications)) - in computing, this usually means "setting up/initializing/giving access;" in other words, preparing an environment or set of requirements for a planned computing activity

* [registry](https://blogs.vmware.com/cloudnative/2017/06/21/what-is-a-container-registry/) - a central location for storing and accessing specific types of computing assets (in the case of Docker, we will be looking more at *container registries* later)

* [repository](https://techterms.com/definition/repository#:~:text=Terms%20%3A%20Repository%20Definition-,Repository,a%20central%20file%20storage%20location.&text=This%20may%20include%20multiple%20source,new%20versions%20of%20the%20program.) - a central location for file storage; the 'central' element is crucial for maintaining version control

* [version control](https://en.wikipedia.org/wiki/Version_control) - a component of technical collaboration in which we rigorously maintain a 'primary/live version' of a shared repository in order to make sure contributors' changes don't conflict

## Virtualization concepts

This section will introduce a few concepts and terms for you to be aware of before we dive into the specifics of Docker. 

[Virtualization](https://en.wikipedia.org/wiki/Virtualization) refers to anytime you create a purely virtual version of something.

![Virtualization meme](/content/figures/VIRTUALIZATION.png)

### Virtual machines (VMs)

[Virtual Machines (VMs)](https://en.wikipedia.org/wiki/Virtual_machine) are purely virtual instances of computers which run *on* another, **real**, computer. 

Virtual machines were first developed in the 1960s, to enable "time sharing" of computing hardware resources for multiple simultaneous users.

The real computer which the VM is running on is often called the 'host,' and the software running on it which creates virtual machines is called a [hypervisor](https://en.wikipedia.org/wiki/Hypervisor).

### Containers

Whereas a VM gives us virtualization all the way down to the kernel and hardware layers, a [container](https://en.wikipedia.org/wiki/OS-level_virtualization) is much more lightweight in comparison. 

![@b0rk on containers](/content/figures/b0rkcontainer.png)
Retrieved from the ["How Containers Work" zine](https://wizardzines.com/zines/containers/) produced by the awesome [Julia Evans, aka b0rk](https://jvns.ca/)

Often called "OS-level virtualization," containers sit on top of the host computer's kernel and merely virtualize from the level of binaries and libraries up to the user interface (see "Computing concepts" above for binary and library definitions). Just like shipping containers, Docker containers kare built to keep software and its dependencies together and ship them with ease. 


### Comparing VMs and Containers

Virtual machines virtualize the entire "tech stack" of a computer down to the hardware. They're a lot more resource-intensive than containers but can be necessary for certain computing tasks. Unlike containers, virtual machines typically contain a whole copy of the operating system and has to get booted up. 

![Containers versus VMs](/content/figures/containersvsvm.png)
Diagram by Chelsea Palmer, [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

Some of the benefits of containers over VMs: containers are more **lightweight** on computing resources, more **portable** between environments, and have **lower management overhead** as they run over top of the existing operating system.

On the negative side, containers are slightly **less fault tolerant** than virtual machines in some computing use cases, provide slightly **less security via isolation**, and are obviously not the right choice in instances where special OS or hardware configurations need to be specified.

![Containers versus VMs part 2](/content/figures/wikicommonsVMcontainer.png)
Another way to model containers vs. VMs, retrieved from [Natlibfi-arlehiko on Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Containers.png), [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

### Docker objects

A Docker **container** is an instance of a Docker **image**. You can run multiple containers, all as instances of the same image. 

The image's specifications provide the information needed to spawn its resulting containers, including their design, content, and constraints. If you need more detail on this, check out [Docker's documentation on Objects](https://docs.docker.com/get-started/overview/#docker-objects).
<br/>

## Virtualization in computing

Across both virtual machines and containers, a few broader principles apply: 

1. The importance of **resource allocation** - how do we ensure computing processes have access to the resources they need?

2. The problem of **isolation** - how do we protect our computing environments from security risks when introducing new computer processes, as well as protecting them from the negative impact of bugs?

3. The strategy of **layering** which we see in action in the first "VMs versus Containers" diagram above: permissions are restricted to lower-level systems layers, preventing containerized processes from touching the operating system.

## Granularity and Reproducibility

Granularity in containers allows for fine-grained control over resource allocation and isolation. It enables administrators and developers to allocate specific amounts of resources to different components within a container, ensuring optimal performance and isolation. It relates to the degree of control and separation that can be applied to different aspects of the container, such as CPU, memory, network, and file system. By adjusting the granularity settings, containerization platforms such as Docker provide flexibility in managing and optimizing resource allocation for different components within containers. This level of control helps in achieving efficient resource utilization, isolation between containers, and effective scaling of containerized applications.

Docker allows applications and their dependencies to be packaged into self-contained containers. Also, Docker images are immutable, meaning they are read-only and cannot be modified once created. Docker's containerization approach and immutable images contribute to achieving reproducibility in software development and deployment.
