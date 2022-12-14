# Cloud Native Application Architecture Nanodegree

## TechTrends Project

_TechTrends_ is an online website used as a news sharing platform, that enables consumers to access the latest news within the cloud-native ecosystem. In addition to accessing the available articles, readers are able to create new media articles and share them.

The web application is written using the `Python Flask framework`. It uses `SQLite`, a lightweight disk-based database to store the submitted articles.


I assumed the role of a platform engineer, to _package_ and _deploy_ TechTrends to _Kubernetes_ using a CI/CD pipeline.

# Project Steps Overview
1. Apply the best development practices and develop the status and health check endpoints for the TechTrends application.
2. Package the TechTrends application by creating a Dockefile and Docker image.
3. Implement the Continuous Integration practices, by using GitHub Actions to automate the build and push of the Docker image to DockerHub.
4. Construct the Kubernetes declarative manifests to deploy TechTrends to a sandbox namespace within a Kubernetes cluster. The cluster should be provisioned using k3s in a vagrant box.
5. Template the Kubernetes manifests using a Helm chart and provide the input configuration files for staging and production environments.
6. Implement the Continuous Delivery practices, by deploying the TechTrends application to staging and production environments using ArgoCD and the Helm chart.


## Technology Stack
### Web Application & Database
- [Python](https://www.python.org/downloads/)
- [Flask](https://flask.palletsprojects.com/)
- [SQLite](https://www.sqlite.org/)

## CI/CD tools

### Containerization & Virtualization
- [Docker](https://www.docker.com/)
- [Vagrant](https://www.vagrantup.com/)

### Automating Deployment & management of containerized applications
- [k3s](https://k3s.io/)

### CI stages tooling
- [Github Actions](https://github.com/features/actions)

### CD tooling
- [argo-cd](https://argoproj.github.io/argo-cd/)

### Deployment on multiple Kubernetes clusters
- [Helm](https://helm.sh/)

## Project Structure

### argocd 
- This folder contains the ArgoCD manifests

### helm 
- This folder contains the Helm chart files

### kubernetes 
- This folder contains Kubernetes declarative manifests

### screenshots 
- This folder contains all the screenshots that you take throughout the course

### docker_commands 
- This file is used to record any used Docker commands and outputs

### Dockerfile 
- This file contains the instructions to package the application

### .github 
- This folder contains the configuration for GitHub Actions workflows
