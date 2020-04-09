# Docker 102 Presentation

## Meta
### What do I want my audience...
- To know?
  - Where they can run Docker containers for free
  - How to run a simple version of the Kuard container using either the CLI or Portainer
  - That there are other free tools that solve some of the problem that Kubernetes
    solves
- To do?
  - Create the Kuard container etiher on the bookclub server or on their own hardware 
  - Poke around in some version of Portainer
- To feel?
  - Comfortable with logging into Portainer
  - Confident cerating a simple Kuard container
### Outline
#### Introduction
- There were some stumbling blocks last week with the Docker-related chapter in the
  book
- I'm here to help the group get past some of those stumbling blocks
#### Points
0. Here's a recap of how Docker's different that VM's
1. You no longer need to install your own Docker server software
   - We now have a shared Docker server that everyone in the group can access using
     either an SSH or web interface
   - Please contact Tom for the credentials
2. Demo of creating a Kuard container and connecting with SSH forwarding
3. ??? Lots of tools exist to solve the problems that Kubernetes is trying to solve ???
#### Conclusion
- We have a nice set of free tools to make it easier to experiment with Docker

## Presentation
### Why?
- There were some stumbling blocks last week with the Docker-related chapter in the
  book
- I'm here to help the group get past some of those stumbling blocks
### Recap
- Docker a framework for managing lightweight containers
- It is the most popular "compute unit" that you can manage with Kubernetes
- You retrieve an **image** so you can run it as a **container**.
  - Analogous to how you store an executable (image) on disk but invoke it to create
    a process (container).
### How Can I Experiment With Docker?
- You can install it on your desktop or home server, but it turns on Hyper-V
  - This could break tools like VirtualBox
- It can also be tricky to install on Linux and OS X
### Book Club Sandbox
- We have a shared Docker server that anyone in the group can use
  - bookclub.tompurl.com
- You can complete the exercises from chapter 2 using either the CLI or a web
  interface (Portainer)
- Please contact Tom Purl if you want the credentials
### Demos
#### Creating a Kuard Container
#### Accessing the Container From My Laptop Using an SSH Tunnel
### Resources
- [Chapter 2 Examples](./chapter-2-examples.md)
  - Cheatsheet to help you complete the Chapter 2 exercises on our shared server.
### Questions?
### Thank you!
