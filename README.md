# K8s-Demo

You will find the following files in this repo:

**Configmap configuration file:** an API object that stores configuration for other objects.

**Secret configuration file:** an object that has a small amount of sensitive data, like a password, token, or key.

**MongoDB configuration file:** a file for deploying containerized MongoDB on Kubernetes

**Webapp configuration file:** a file for deploying our containerized webapp on Kubernetes

**Note:** all the files are in yaml.

## Goal of the Project

The goal of the project is to deploy a MongoDB container and a simple webapp container on Kubernetes.

## Introduction

### Docker Container

A Docker container is a standardized unit of software that contains everything needed to run an application--including the code, a runtime, libraries, environment variables, and configurations. Containers are isolated from one another and bundle their own software, libraries, and configuration files; they can communicate with each other through well-defined channels. By contrast, a virtual machine (VM) runs a full-blown operating system in addition to its application, which means that it requires more memory and processing power than a container.

### Kubernetes

Kubernetes is a system for automating deployment, scaling, and management of containerized applications. It groups containers that make up an application into logical units for easy management and discovery. Kubernetes builds upon a decade and a half of experience at Google running production workloads at scale, combined with best-of-breed ideas and practices from the community.

## Prerequisite

To utilize this repo, the following must be available on your local machine:

* Docker. Learn how to install docker [Here](https://docs.docker.com/desktop/install/windows-install/). 

* Minikube and kubectl installed. Learn how to do that [Here](https://minikube.sigs.k8s.io/docs/start/).

## How to Use This Repo

1) Fork the repo, and clone it on our local device. 

2) Navigate to the project directory. 

3) Run
```
minikube start --driver=hyperv
```
**Note:** `virtualbox` can be used in place of hyperv as the driver, provided you have it installed. Also, `docker` can also be used.

4) Once minikube has started, run
```
kubectl apply -f mongo-config.yaml
```
5) Next, run 
```
kubectl apply -f mongo-secret.yaml
```
6) Then, run
```
kubectl apply -f mongo.yaml
```
7) Run
```
kubectl apply -f webapp.yaml
```
8) Finally, run
```
kubectl apply -f 
```
