---
layout: page
title: Learning activities
permalink: /activity/
parent: Part 2 - Technical Overview
nav_order: 3
---

# Hands-on learning activities

Even though mastering Docker can help you solve the many environment and dependency issues you'll come across in computing, getting Docker itself running on any given system can be quite a challenging task initially!

In the interest of time, we'll be exploring a few different browser-based implementations of Docker containers instead of doing a live install, but we welcome you to reach out for a follow-up appointment if you need one-on-one troubleshooting.

### Jupyter and Binder

[Project Jupyter](https://jupyter.org) produces open source software, and is best known for [Jupyter Notebooks](https://jupyter.org/try) which provide an interactive and reusable playground for documentation and code.

Again, rather than installing everything locally, we'll be utilizing in-browser instances of Jupyter [hosted on Binder](https://jupyter-docker-stacks.readthedocs.io/en/latest/using/running.html#using-binder), which allows us to explore a pre-made instance of [Jupyter Docker Stacks](https://jupyter-docker-stacks.readthedocs.io).
<br/>

### Primary Activity

Please navigate to [Jupyter Docker Stacks hosted on MyBinder.org](https://mybinder.org/v2/gh/jupyter/docker-stacks/master?filepath=README.ipynb). *It may take up to a few minutes to successfully generate the repository in the link's virtual environment.*

Once the environment has loaded, you'll see the Jupyter notebook content, with six executable lines of code demonstrating the sorts of commands and inquiries users can make within the Jupyter Docker Stacks workflow.

For each line in the Jupyter Notebook which has "In [#]" to its left, you can click on that line and then ">Run" in the top bar of the browser window in order to execute the code.

The notebook's content makes reference to [Conda](https://docs.conda.io/en/latest/)- this is a package manager for the Python environment. 

As you explore the output of notebook lines, compare to your previous experiences with hands-on computing. Some of these commands are somewhat universal: **ls**, for example, is frequently invoked to "list files" in a computing context.
<br/>

### Optional Additional Activity

If you're interested, feel free to explore [Docker Hub's Playground](https://labs.play-with-docker.com/) as well. You need to set up a free Docker Hub ID on their site, which will allow you to access the Hub's repository of shared Docker images in the future as well.

While the Docker Hub playground appears to have a lot more room for functionality than the single use case of the Jupyter Docker Stacks explored above, the link is not always reliable to load and there is not much guidance provided for newcomers to Docker on what to explore within this playground.