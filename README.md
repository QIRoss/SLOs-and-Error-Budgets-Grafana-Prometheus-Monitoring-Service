# SLOs and Error Budgets Grafana Prometheus Monitoring Service

Studies based in day 43-44 of 100 Days System Design for DevOps and Cloud Engineers.

https://deoshankar.medium.com/100-days-system-design-for-devops-and-cloud-engineers-18af7a80bc6f

Days 41–50: Reliability Engineering

Day 43–44: Study and set up Service Level Objectives (SLOs) and Error Budgets for critical services.

## Project Overview

The goal of this project is to help teams define, monitor, and manage service reliability through SLOs and Error Budgets. It uses Prometheus for gathering metrics and Grafana for visualizing and tracking the performance of the application. By setting SLOs, you can define the acceptable threshold for system reliability, and Error Budgets help balance the risk of new deployments against reliability commitments.

Key Components:
* FastAPI: A simple API that serves as the monitored service.
* Prometheus: Collects metrics and exports them for analysis.
* Grafana: Visualizes the metrics, allowing for easy monitoring of SLOs.
* Docker Compose: Manages the multi-service setup.

## How to Use

Prerequisites:

Docker and Docker Compose installed on your machine.
Steps to Run:
Clone this repository:
```
git clone https://github.com/your-repo/slo-monitoring.git
cd slo-monitoring
```
Start the services using Docker Compose:
```
docker-compose up --build
```
Access the services:

* FastAPI service at ```http://localhost:8000``` .
* Prometheus dashboard at ```http://localhost:9090``` .
* Grafana dashboard at ```http://localhost:3000``` .

To monitor the SLOs:

* Login to Grafana with default credentials (admin/admin).
* Configure Prometheus as a data source in Grafana.
* Import or create dashboards to visualize the SLO and Error Budget metrics.

Customize your prometheus.yml file to set specific targets for the SLOs or import pre-configured Grafana dashboards to get started.

To stop all running containers:
```
docker-compose down
```

## Author
This project was implemented by [Lucas de Queiroz dos Reis][2]. It is based on the [100 Days System Design for DevOps and Cloud Engineers][1].

[1]: https://deoshankar.medium.com/100-days-system-design-for-devops-and-cloud-engineers-18af7a80bc6f "Medium - Deo Shankar 100 Days"
[2]: https://www.linkedin.com/in/lucas-de-queiroz/ "LinkedIn - Lucas de Queiroz"