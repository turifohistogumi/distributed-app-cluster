# Distributed Application Cluster

This project contains the configuration and source code for deploying a highly available, distributed application environment. 

## Architecture Overview
To ensure high availability and proper load balancing, the infrastructure is divided into multiple nodes across different regions:
* **Load Balancers (2 Nodes):** To distribute incoming traffic efficiently.
* **Web/Application Servers (8 Nodes):** Running the core application instances to handle user requests.
* **Database Cluster (6 Nodes):** Setting up a replication cluster (Primary/Secondary) for data redundancy.
* **Caching & Queue Nodes (4 Nodes):** Redis/RabbitMQ nodes for session management and background tasks.

Total requested resources: **20 Nodes**.

## Technology Stack
* **OS:** Ubuntu 22.04 LTS / Debian
* **Web Server:** Nginx / Apache
* **Containerization:** Docker & Docker Compose
* **Database:** PostgreSQL / MySQL
