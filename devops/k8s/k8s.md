---
marp: true
theme: default
---

![bg left:40% 100%](https://miro.medium.com/max/700/1*tP8OkC__HFt0ctvKVm3nvw.png)

# Scaling tests on Google Kubernetes Engine with Cloud Build

---

# Agenda

- Containerization and Orchestration
- Kubernetes Architecture
- Kubernetes Objects
- Code walk through
- Demo time !!!

---

# Containerization

Containerization is the packaging together of software code with all it’s necessary components like libraries, frameworks, and other dependencies so that they are isolated in their own **container**.

![width:5000px height:12cm](https://github.com/madhank93/learn-docker/raw/master/img/history.png)

---

# Some of the famous Container run times

- [Docker](https://www.docker.com/) - de facto standard
- [cri-o](https://cri-o.io/)
- [podman](https://podman.io/) - it is a daemonless container engine

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

# Orchestration

It solves the problem by automating the scheduling, deployment, scalability, load balancing, availability, and networking of containers.

Container orchestration is the automation and management of the lifecycle of containers and services.

---

# Some of the famous Orchestration tools

- [Kubernetes](https://kubernetes.io/) - de facto standard
- [OpenShift](https://www.openshift.com/)
- [Nomad](https://www.nomadproject.io/)
- [Docker swarm](https://docs.docker.com/engine/swarm/)
- [Apache Mesos](https://mesos.apache.org/)

---
