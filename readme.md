# Kubernetes clusteer

What? - System for running many different contains over multiple different machines
Why? - When you need to run many different containers with different images, and scaling concerns

Master with one or more nodes (VM) running n number of containers

master controls what does nodes is running at any given time, we developers interact with the master, to control those nodes.

Outside the cluster we have a load balancer which receives outside traffic (request)

## Working with Kubernetes

In development - we use minikube (CLI tool)
In production - Elastic Container Service for Kubernetes (EKS), Goggle Cloud Kubernetes Engine (GKE), do it your self option

**Minikube (LOCAL ONLY)**
Will create a mini cluster (VM) on your machine, used for creating and running a mini cluster on your machine

**kubectl (BOTH LOCAL AND PROD)**
use for managing containers in the node, what set of containers it should run/manage

## Docker Compose -> Kubernetes

- Each entry can optionally get docker-compose to build an image -> Kubrnetese expect all images to already be built

- Each entry represent a container we want to create -> one config file per object we want to create

- Each entry defines thee networking requirements (ports) -> We have to manually set up all networking

### Get a simple container running on our local kubernetes cluster running

- We have the images built already and published to docker hub in previous app
