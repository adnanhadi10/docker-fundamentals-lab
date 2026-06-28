\# Docker Fundamentals Lab



A hands-on Docker fundamentals project completed on an Ubuntu 24.04 virtual machine hosted on \*\*Google Cloud Platform (GCP)\*\*. This project focuses on understanding Docker concepts through practical experimentation rather than simply executing commands.



\---



\## Project Overview



The goal of this lab was to build a solid understanding of Docker by exploring how images, containers, filesystems, and Docker resources interact. Every concept was verified through command-line experiments, helping develop a practical understanding of Docker's architecture and lifecycle.



\---



\## Objectives



\- Install Docker Engine on Ubuntu

\- Verify Docker installation

\- Pull images from Docker Hub

\- Understand Docker images and containers

\- Learn the Docker container lifecycle

\- Explore interactive containers

\- Understand filesystem isolation

\- Verify container persistence

\- Learn Docker cleanup and dependency management



\---



\## Technologies Used



\- Google Cloud Platform (GCP)

\- Ubuntu 24.04 LTS

\- Docker Engine

\- Linux (Bash)

\- Git

\- GitHub



\---



\# Docker Architecture



```text

&#x20;                Docker Hub

&#x20;                     │

&#x20;                     ▼

&#x20;               Ubuntu Image

&#x20;                     │

&#x20;       ┌─────────────┴─────────────┐

&#x20;       ▼                           ▼

&#x20;Container 1                  Container 2

&#x20;  (Ubuntu)                  (Hello World)



Each container has its own isolated writable filesystem.

```



\---



\## Commands Used



```bash

docker --version

docker info

docker images

docker ps

docker ps -a

docker run hello-world

docker run -it ubuntu bash

docker start -i

docker logs

docker inspect

docker rm

docker rmi

```



\---



\## Lab Walkthrough



\### 1. Provisioned an Ubuntu Virtual Machine



Created an Ubuntu VM on Google Cloud Platform to serve as the Docker host.



\---



\### 2. Installed Docker Engine



Configured Docker's official repository and installed Docker Engine.



\---



\### 3. Verified Installation



Verified Docker was successfully installed and operational.



\---



\### 4. Executed the Hello World Container



Downloaded the official Docker image from Docker Hub and confirmed successful execution.



\---



\### 5. Explored Images and Containers



Learned the relationship between reusable Docker images and container instances.



\---



\### 6. Investigated Filesystem Isolation



Created a file inside an Ubuntu container and verified it was isolated from the host VM.



\---



\### 7. Verified Container Persistence



Stopped and restarted the same container to confirm its writable filesystem remained intact.



\---



\### 8. Cleaned Docker Resources



Removed containers and images while observing Docker's dependency protection mechanisms.



\---



\# Project Screenshots



\## Docker Installation



!\[Docker Installation](screenshots/04-docker-installation-success.png)



\---



\## Docker Container Lifecycle



!\[Container Lifecycle](screenshots/06-docker-container-lifecycle.png)



\---



\## Filesystem Isolation \& Persistence



!\[Filesystem Isolation](screenshots/07-container-filesystem-isolation-and-persistence.png)



\---



\## Docker Cleanup



!\[Docker Cleanup](screenshots/08-docker-cleanup-and-final-state.png)



\---



\# Lessons Learned



\- Docker images act as reusable blueprints.

\- Multiple containers can be created from a single image.

\- Containers have isolated filesystems.

\- Stopping a container preserves its writable layer.

\- Deleting a container removes its writable filesystem.

\- Docker prevents deleting images that are still referenced by containers.

\- Verifying every action after execution simplifies troubleshooting.



\---



\# Skills Demonstrated



\- Docker Installation

\- Docker Image Management

\- Docker Container Management

\- Linux Command Line

\- Docker Troubleshooting

\- Filesystem Isolation

\- Resource Cleanup

\- Git

\- GitHub Documentation



\---



\# Future Improvements



\- Learn Docker Volumes

\- Build a Dockerized Web Application

\- Deploy Multi-Container Applications using Docker Compose

\- Learn Kubernetes Container Orchestration

