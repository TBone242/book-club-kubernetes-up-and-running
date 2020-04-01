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
    - How much can we ship while maintaining a highly maintainable service?
### Core Concepts
    1. Immutability
    2. Declarative configuration
    3. Online self-healing systems
## Scaling
### Decoupling
    - Kubernetes promotes serving everything as an API
### Easy System Scaling
    - Immutable, declarative services are easier to scale
    - Kubernetes is also good at managing resources efficently across a cluster
### Scaling Development Teams
    - Kubernetes "primitives" work well with small teams
      - e.g pods, ingresses, services, etc.
### Separation of concerns
    - Kubernetes encourages loose coupling between system layers
      - e.g. hardware, OS, cluster/K8s, application
    - Makes it easier for teams to specialize in one layer
