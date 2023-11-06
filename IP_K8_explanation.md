# Kubernetes Project on Google Kubernetes Engine (GKE)

Welcome to our Kubernetes project hosted on Google Kubernetes Engine (GKE). This project aims to deploy an application on GKE and leverages various Kubernetes concepts to ensure reliability and performance. The following sections provide an overview of the project and its key objectives.

## Table of Contents

- [Objectives](#objectives)
- [Getting Started](#getting-started)
- [Kubernetes Objects](#kubernetes-objects)
- [Exposing Pods](#exposing-pods)
- [Persistent Storage](#persistent-storage)
- [Git Workflow](#git-workflow)
- [Running the Application](#running-the-application)
- [Docker Image Tagging](#docker-image-tagging)
- [Repository Structure](#repository-structure)
- [Feedback and Contributions](#feedback-and-contributions)
- [License](#license)

## Objectives

Our project encompasses the following key objectives:

### 1. Choice of Kubernetes Objects for Deployment

For deploying our application on GKE, we have thoughtfully selected Kubernetes objects. Notably, we embrace StatefulSets to address the requirements of applications that demand stable network identifiers and persistent storage.

### 2. Method for Exposing Pods to Internet Traffic

We ensure that our application is accessible to the public by employing Kubernetes Services of type LoadBalancer. This technique effectively routes internet traffic to our pods. Additionally, NodePort can be used for different use cases where it maps a port on each node to a port on the pods.

### 3. Use of Persistent Storage

Our application mandates the use of persistent storage to retain data. To meet this requirement, we have configured Persistent Volume Claims (PVCs) and Persistent Volumes (PVs). PVCs enable pods to request specific storage resources, while PVs provide the actual storage and manage its lifecycle.

### 4. Git Workflow

We maintain a structured Git workflow to efficiently manage our project. Our workflow includes creating feature branches for code changes, committing regularly with descriptive messages, and initiating pull requests for code review. To ensure code stability, we maintain separate branches for development and production.

