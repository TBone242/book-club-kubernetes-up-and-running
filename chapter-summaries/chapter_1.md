# Chapter 1 Notes

## Meta
- **Presenter**: Tom Purl
- **Date**: 4/1/2020
## Main Benefits
- Velocity
- Scaling (software and teams)
- Abstracting your infrastructure
- Efficiency
## Velocity
- How frequently can we ship while maintaining a highly maintainable service?
  - Big data 3 v's - velocity, volume, veracity
### Core Concepts
1. Immutability
   - Data perspective - Data doesn't change, store it as you get it
   - Docker / LXE 
2. Declarative  configuration
   - YAML / JSON config, not code 
   - Idempotent
   - Easily specify/enforce the number of services
3. Online self-healing systems
## Scaling
### Decoupling
- Kubernetes promotes serving everything as an API
### Easy System Scaling
- Immutable, declarative services are easier to scale
- Kubernetes is also good at managing resources efficently across a cluster
  - Not necessarily expensive
### Scaling Development Teams
- Kubernetes "primitives" work well with small teams
  - e.g pods, ingresses, services, etc.
### Separation of concerns
- Kubernetes encourages loose coupling between system layers
  - e.g. hardware, OS, cluster/K8s, application
- Makes it easier for teams to specialize in one layer

## Q & A
- How can I change my mindeset from VMWare-centric to container-centric?
- How do we convert an existing app to a Kubernetes-hosted app?
- What are some good ideas for a small kubernetes project?
  - Selenium grid?
  - PHP/web app?
  - "Bare metal" cluster :-) 
  - Work as a team on different components?
  - It's OK if you don't want to actively work on a shared project 😼
- Does kubernetes make it easier to upgrade code?
- Walter will run chapter 2!
