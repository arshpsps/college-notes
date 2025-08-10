**Cloud Computing architecture** referes to the components and subcomponents required for cloud computing.

Types: Public, Private, Hybrid, Community

Service Models: IaaS, PaaS, SaaS

Benefits: Scalability, Cost Effectiveness, Flexibility, Business Agility

Challenges: Privacy, Security, Vendor lock-in

Virtualization enables cloud computing by **abstracting resources** from hardware.

---

#### Architecture

##### Frontend components

User Interface (UI) - Web browsers, Mobile apps

##### Backend Components

- Servers
- Storage
- Networking
- Operating Systems

##### Cloud-Based Delivery

Network of remote servers hosted on the Internet to **store**, **manage** and **process** data.

##### Service-Oriented Architecture

Modular approach for software design that enables creation of **scalable** and **reusable** services.

---

#### Types

##### Public Cloud

###### Pros

- Cost-effective
- Scalable
- No Maintenance

###### Cons

- Less Secure
- Less Customizable

##### Private Cloud

###### Pros

- Highly Secure
- Customizable

###### Cons

- Expensive
- Require Maintenance

##### Hybrid Cloud

###### Pros

- Combines benefits of **Public** and **Private** Clouds

###### Cons

- Complex to set-up and manage

---

#### Service Models

##### Infrastructure as a Service (IaaS)

Provides virtualized computing resources over the internet.

##### Platform as a Service (PaaS)

A platform for developing, running and managing applications.

##### Software as a Service (SaaS)

Software applications over the internet on a **subscription** basis.

---

#### Benefits of Cloud Computing

- Scalability
- Flexibility
- Cost-effectiveness
- Reliability
- Security

---

#### Challenges of Cloud Computing

- Security
- Privacy
- Compliance
- Vendor lock-in
- Cost Management

---

#### Cloud Architecture

##### Benefits

- Agility: Allows businesses to rapidly scale resources.
- Reduced time-to-market for new products and features.
- Increased collaboration and innovation through shared resources.
- Faster disaster recovery.
- Improved business continuity.

##### Challenges

- Data Security
- Privacy
- Potential Vendor lock-in

---

#### Virtualization

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

---

#### Containers and Microservices

- Containers package software with all its dependencies for consistent execution across environments.
- Microservices are an **architectural** approach where applications are built as a collection of small, independent services.
- Each microservice has its own container and communicates with other microservices via APIs.
- scalable, flexible, faster development and deployment cycles.

- Docker is an open platform for building shopping and running distributed applications.
- Containers are standardized unit of software that allow developers to isolate their app from outside environment, allowing consistent behavior across machines and environments.
- Benefits: rapid onboarding, easy CI, container images as build artifacts, decoupling, helps escape dependency hell.
- Dockerfile is build recipe file for Docker image, containing instructions of how to construct the image.
- Key Docker instructions: FROM, RUN, CMD, ENTRYPOINT, COPY, ADD, VOLUME, WORKDIR, ENV, EXPOSE, MAINTAINER
- .dockerignore
