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
