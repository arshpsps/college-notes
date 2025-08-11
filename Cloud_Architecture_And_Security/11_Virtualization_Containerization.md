### Virtualization

- Abstracts computing resources from physical infrastructure.
- Creates virtual versions of hardware, OS, storate devices and networks.
- Multiple Virtual Machines (VMs) can run on a single physical server.
- Each VM operates independently with its own OS and applications.
- Cloud provides use Virtualization to efficiently manage resources.
- On-demand access over the internet.
- Enables flexibility, scalability, and cost-effectiveness in cloud computing.

##### VMWare ESX

- Baremetal Hypervisor
- Installed directly on physical Server.
- Manages system resources and provides them to virtual machines.
- ESX partitions resourecs like CPU, memory, storage and networking.

#### Benefits of Virtualization

- **Efficient resource utilization**: Multiple VMs on a single physical server
- **Cost Savings**
- **Scalability**: Easy to scale up or down VMs according to needs
- **Isolation**: VMs by nature don't allow interference.

---

### Containers and Microservices

- Containers package software with all its dependencies for consistent execution across environments.
- Microservices are an **architectural** approach where applications are built as a collection of small, independent services.
- Each microservice has its own container and communicates with other microservices via APIs.
- scalable, flexible, faster development and deployment cycles.

- **Docker** is an open platform for building shopping and running distributed applications.
- Containers are standardized unit of software that allow developers to isolate their app from outside environment, allowing consistent behavior across machines and environments.
- Benefits: rapid onboarding, easy CI, container images as build artifacts, decoupling, helps escape dependency hell.
- Dockerfile is build recipe file for Docker image, containing instructions of how to construct the image.
- Key Docker instructions: FROM, RUN, CMD, ENTRYPOINT, COPY, ADD, VOLUME, WORKDIR, ENV, EXPOSE, MAINTAINER
- .dockerignore

#### [Podman](https://docs.google.com/document/d/14wGQHC-cmJJToUg39Pr_xOkCXKkdN6H8Hiz6WFNB8QM/edit?tab=t.0)

Daemonless container engine for developing, managing and running OCI (Open Container Initiative) containers on a GNU/Linux system.

##### Advantages

- **Daemonless Architecture**: Unlike Docker, Podman doesn't run a daemon. Therefore, Less resource consumption & no single point of failure.
- **Rootless Containers**: Allows running containers as a non-root user.
- **Docker Compatibility**: Podman CLI is largely compatible with docker & so ofter you could alias docker to podman.
- **Pods**: Group of containers that share the same network namespace & resources, similar to kubernetes.
- **Kubernetes Integration**: Podman can generate Kubernetes YAML files from running containers & pods.
- **Systemd integration**: Containers can be managed as Systemd services.

#### Kubernetes - Not in Syllabus (i think)

Tool for managing and automating (Orchestration) containerized workloads in the cloud.

- **Auto-Scale**: Can scale containers across multiple machines.
- **Auto-Heal**: Automatically replace broken containers.
- **High Availability**: Maintains a "replica set" of Pods/Containers ready to go / replace others.

- **Cluster**: A system deployed on Kubernetes.
- **Nodes**: Worker Machines that make up a cluster.
- Nodes commmunicate with the parent using a **Kubelet**, running on each node.
- **Pods**: Smallest deployable unit, representing a single instance of a running process or a group of tightly coupled processes.
- Kubernetes runs a API server on the *Master* machine that all other Nodes communicate with (using a Kubelet).
