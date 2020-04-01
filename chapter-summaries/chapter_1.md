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
