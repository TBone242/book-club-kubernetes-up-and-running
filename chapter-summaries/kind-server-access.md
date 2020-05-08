# kind Server Access Instructions

## Logging Into the Server Using SSH

Contact Tom P. in the Slack channel for these instructions.

## Creating Your First Kubernetes Cluster

**Please note that you only have to create a cluster once.**

To execute the examples in the book you first need to create a cluster. Here's how
you do that with ``kind``:

1. SSH into the bookclub server as the ``lab`` user.
2. Become the ``root`` user like this:
  - ``sudo su - root``
3. Now you can create you cluster like so:
  - ``kind create cluster --name tom-p-cluster-1``
  - Ideally you should put something unique in the cluster name that you will remember

That's it! Now you can start using ``kubectl``

## Accessing Your Cluster

1. SSH into the bookclub server as the ``lab`` user.
2. Become the ``root`` user like this:
  - ``sudo su - root``
3. Find your cluster's exact name with thic command:
  - ``kubectl config get-contexts``
4. You should look for your cluster name and make a note of it.
5. Now you can execute the ``kubectl`` commands!

For example, let's say that your cluster name is ``kind-tom-p-cluster-1``. To interact with this cluster you would type the following command:

```
kubectl cluster-info --context kind-tom-p-cluster-1
```

To view your pods you would type this command:

```
kubectl get pods --context kind-tom-p-cluster-1
```

So basically, just append ``--context your-cluster-name`` to the end of every
``kubectl`` command.
