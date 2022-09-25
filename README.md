# K8s manifesto for Go Todo App
The simple k8s manifesto for Go Todo App

## prerequisite for Local Env
[Docker Desktop](https://docs.docker.com/desktop/install/mac-install/)
    * You can also install from [here](https://formulae.brew.sh/formula/docker#default)

## How to setup
Before you started check the document below and enable Docker Desktop's Kubernetes
[Deploy on Kubernetes](https://docs.docker.com/desktop/kubernetes/)

After the setup, you can deploy app through _kubectl_

1. apply config

> kubectl apply -f todo-go-config.yaml

2. apply secret

> kubectl apply -f todo-go-secret.yaml

3. apply deployment & service

> kubectl apply -f todo-go.yaml

After the setup, you can check status via

> kubectl get all

then, access kubernetes app from host machine's browser via

> kubectl port-forward {pod NAME} :8080

with Forwarding address
