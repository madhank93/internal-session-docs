---
marp: true
theme: default
---

![bg left:40% 100%](https://miro.medium.com/max/700/1*tP8OkC__HFt0ctvKVm3nvw.png)

# Scaling tests on Google Kubernetes Engine with Cloud Build

---

# Agenda

- Containerization
- Orchestration
- Kubernetes Architecture
- Kubernetes Objects
- Code walk through
- Demo time !!!

---

# Evolution

**Containerization** is the packaging together of software code with all it’s necessary components like libraries, frameworks, and other dependencies so that they are isolated in their own **container**.

![width:5000px height:12cm](https://github.com/madhank93/learn-docker/raw/master/img/history.png)

---

![width:5000px height:18cm](https://cdn.ttgtmedia.com/rms/onlineImages/microservices-vm_versus_docker.jpg)

---

# Docker architecture

![](https://docs.docker.com/engine/images/architecture.svg)

---

# Docker Components

- **Client** - is the primary way to interact with Docker. When commands such as `docker run` executed the client sends these commands to dockerd (daemon), which carries them out.
- **Daemon** - receives the commands from the client through CLI or REST API. It listens to requests and processes Docker commands related to images, containers, networks, and volumes.
- **Dockerfile** - is a text document that contains all the commands to build an image.
- **Image** - are read-only templates built from a set of instructions written in Dockerfile. Images contains application and its dependencies.
- **Registries** - is a repository (storage) for Docker images.
- **Containers** - is the instance of an image. We can create, run, stop, or delete a container using the Docker CLI.

---

# Why we need ?

![width:500px height:10cm](https://github.com/madhank93/learn-docker/raw/master/img/compatibility_dependency_issue.jpg)

- To avoid compatibility issues with an underlying OS or between the services & libraries dependencies with the OS. (**So no more - It works on my machine!**)
- To reduce local development environment setup time.

---

# What it does ?

![width:700px height:10cm](https://github.com/madhank93/learn-docker/raw/master/img/docker_ability.jpg)

- Containerize an applications

- Isolates apps from each other

- Run each service with its own dependencies in separate containers

---

# Some of the famous Containerization technology

- [Docker](https://www.docker.com/) - de facto standard
- [cri-o](https://cri-o.io/)
- [podman](https://podman.io/) - it is a daemon less container engine

---

# Demo Time !!!

---

# Orchestration

Container orchestration is the automation and management of the lifecycle of containers and services.

It solves the problem by automating the scheduling, deployment, scalability, load balancing, availability, and networking of containers.

---

# Some of the famous Orchestration tools

- [Kubernetes](https://kubernetes.io/) - de facto standard
- [OpenShift](https://www.openshift.com/)
- [Nomad](https://www.nomadproject.io/)
- [Docker swarm](https://docs.docker.com/engine/swarm/)
- [Apache Mesos](https://mesos.apache.org/)

---
