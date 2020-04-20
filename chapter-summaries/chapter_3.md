# Chapter 3

## Errata

Not all of the examples in the book work on the latest version of Kubernetes. Also,
different Kubernetes "distributions" may require slightly different versions of the
commands. Here's some notes from different providers.

### Digital Ocean

#### Installing Kubernetes on a Public Cloud Provider

I setup my hosted Kubernetes cluster using Digital Ocean, which isn't documented in
the book. Here's how I did it.

TODO

#### Kubernetes DNS

You should use these commands to look at the DNS service:

``` bash
kubectl get deployments --namespace=kube-system coredns
kubectl get services --namespace=kube-system kube-dns
```

#### Kubernetes UI

I couldn't get any of the examples under this section working.
