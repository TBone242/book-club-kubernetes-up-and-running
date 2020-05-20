Options for running Kubernetes locally
https://developer.ibm.com/technologies/containers/blogs/options-to-run-kubernetes-locally/

Install Docker

Installed using Package Manager

Add the Docker User Group
sudo usermod -aG docker $USER && newgrp docker


Install kubectl
Kubectl is Kubernetes command line tools allowing you to run commands against Kubernetes. 

https://kubernetes.io/docs/tasks/tools/install-kubectl/#install-kubectl-on-linux

Command
curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl

chmod +x ./kubectl

sudo mv ./kubectl /usr/local/bin/kubectl

Test: kubectl version --client



Install minikube
Minikube is a tool that runs a single-node Kubernetes cluster in a virtual machine on your personal computer.

Command
curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 && chmod +x minikube

sudo mkdir -p /usr/local/bin/

sudo install minikube /usr/local/bin/

Start using Docker
This needs to happen on the actual computer

Command
minikube start --driver=docker

Start using KVM or VirualBox
First install KVM or VirtualBox

Command
minikube start

— will download the ISO for Minikube and run. 

Install Web UI
https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard/

Command
kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.0.0/aio/deploy/recommended.yaml

kubectl proxy

Access:
http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/

Create a token for Web UI
https://www.replex.io/blog/how-to-install-access-and-add-heapster-metrics-to-the-kubernetes-dashboard

Command
kubectl create serviceaccount dashboard-admin-sa

kubectl create clusterrolebinding dashboard-admin-sa --clusterrole=cluster-admin --serviceaccount=default:dashboard-admin-sa

kubectl get secrets

Replace the 'xxxx' with what you find when you run the get secrets command. 

kubectl describe secret dashboard-admin-sa-token-xxxx

Copy the token and paste in the Kubernetes Web UI


Using MicroK8s
https://kubernetes.io/blog/2019/11/26/running-kubernetes-locally-on-linux-with-microk8s/


Deploy Web UI
https://www.techrepublic.com/article/how-to-deploy-the-kubernetes-webui-with-microk8s/

