## Introduction to Servers

- Server is a computer designed to **process requests** and **deliver data** over a network.
- Dedicated computer that provides services on behalf of clients.
- Can be classified based on **architecture**, **size**, and **purpose**.
- Web Server, Database server, E-mail server
- Server processors support "ECC" RAM (Error Correction Code)
- ECC detects if data was processed correctly
- Servers run hard drives in [RAID](./21_RAID.md) setup.

#### Types of Servers

##### Standalone Servers

Self-contained units with independent resources. Simplest server architecture.

##### Blade Servers

Modular units in a chassis, sharing power and cooling. High density but less flexible.

##### Stateless Servers

Client data is not stored between requests. Enables scalability and fault tolerance.

#### Stateful & Stateless architecture

##### Stateful

eg. User data is maintained in the server (session, etc)
Here, if the specific server instance goes down, the session won't exist anymore. State is lost.

- Availability Issues
- Scalability concerns

##### Stateless

Data is maintained in a shared storage space and so any server instance could request the data at any time.
Load balancing across individual requests is made possible / easy.

#### Clustering, Scaling, Optimization

- Clustering: A group of servers working together to handle requests as a single system.
- Load Balancing: Distribute traffic across multiple servers to improve performance and reliability
- Horizontal Scaling: Adding more servers
- Vertical Scaling: Upgrading existing server resources
- Optimization Techniques: Caching, Compression, using efficient algorithms

#### Limitations of Traditional Servers

- **Physical Space**: required dedicated space, power, and cooling.
- **Scalability**: Difficult and time consuming to scale up or down.
- **Single point of failure**
- **Maintenance Overhead**: Required ongoing management and updates.
- **Cost Inefficiency**: High upfront costs and ongoing expenses.

#### Modern Solutions

- Scalable, flexible, on-demand cloud resources
- Containers: lightweight, portable environments for apps
- Pre-built cloud solutions for dbs, storage and networking
- Serverless
- Kubernetes

#### Cloud Applications in Finance and Databases

- Streamline financial modeling and risk analysis using scalable cloud resources
- Disaster Recovery and Data Backup
- Scalable, high-performance trading platforms
- Cloud-based DBs for real-time transaction processing and analytics
- AI/ML for fraud detection and prevention
