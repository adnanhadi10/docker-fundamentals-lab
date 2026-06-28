\# Docker Fundamentals Lab



\## Project Overview



This project documents my hands-on journey learning Docker fundamentals using an Ubuntu virtual machine hosted on Google Cloud Platform (GCP).



The primary objective was to understand Docker from first principles rather than simply memorizing commands. Throughout the lab, I explored how images, containers, filesystems, and Docker resources work by performing practical experiments and verifying each concept through the command line.



\---



\## Objectives



\- Install Docker Engine on Ubuntu

\- Verify Docker installation

\- Pull images from Docker Hub

\- Understand the relationship between images and containers

\- Learn the Docker container lifecycle

\- Explore interactive containers

\- Understand container filesystem isolation

\- Verify data persistence after stopping containers

\- Learn Docker resource cleanup and dependency management



\---



\## Technologies Used



\- Google Cloud Platform (GCP)

\- Ubuntu 24.04 LTS

\- Docker Engine

\- Linux Command Line (Bash)



\---



\## Concepts Learned



\- Docker Images

\- Docker Containers

\- Docker Hub

\- Container Lifecycle

\- Interactive Containers (`docker run -it`)

\- Filesystem Isolation

\- Container Persistence

\- Docker Logs

\- Docker Inspect

\- Docker Cleanup (`docker rm`, `docker rmi`)

\- Image and Container Dependencies



\---



\## Lab Progress



\### 1. Provisioned an Ubuntu VM on Google Cloud



Configured a Linux virtual machine to serve as the Docker host.



\### 2. Installed Docker Engine



Added Docker's official repository and installed Docker Engine.



\### 3. Verified Docker Installation



Confirmed Docker was running successfully using version and test commands.



\### 4. Ran the Hello World Container



Pulled the official Docker image from Docker Hub and executed the container successfully.



\### 5. Explored Docker Images and Containers



Learned the difference between reusable images and running container instances.



\### 6. Investigated Container Isolation



Created a file inside an Ubuntu container and verified it was isolated from the host VM.



\### 7. Verified Container Persistence



Restarted the same container and confirmed the file remained available.



\### 8. Cleaned Up Docker Resources



Removed containers and images while observing Docker's dependency protection mechanisms.



\---



\## Screenshots



Screenshots documenting each milestone are available in the \*\*screenshots/\*\* directory.



\---



\## Key Takeaways



\- Images are reusable templates used to create containers.

\- Multiple containers can be created from a single image.

\- Containers have isolated filesystems.

\- Stopping a container preserves its filesystem.

\- Deleting a container removes its writable filesystem.

\- Docker prevents images from being deleted while dependent containers still exist.

\- Verifying every action is an important engineering practice.



\---



\## Skills Demonstrated



\- Docker installation and configuration

\- Linux command line

\- Container lifecycle management

\- Docker troubleshooting

\- Resource cleanup

\- Filesystem isolation

\- Docker fundamentals

