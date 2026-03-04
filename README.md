# Prometheus & Grafana Monitoring Stack with Alertmanager

## Overview

This project demonstrates a monitoring stack using **Prometheus, Grafana, and Alertmanager** running in Docker.

The stack collects system and application metrics, evaluates alert rules, and visualizes metrics through dashboards. Alerts are routed through Alertmanager and sent to a webhook receiver.

This lab helps practice modern **DevOps monitoring and observability concepts** such as metrics collection, alerting pipelines, and containerized monitoring infrastructure.

---

## Tech Stack

- Prometheus – Metrics collection and monitoring  
- Grafana – Metrics visualization dashboards  
- Alertmanager – Alert routing and notification management  
- Node Exporter – System metrics exporter  
- Docker & Docker Compose – Container orchestration  
- Webhook Sink – Simulated alert receiver  

---

## Architecture

Application / VM  
↓  
Node Exporter  
↓  
Prometheus (scrapes metrics & evaluates alerts)  
↓  
Alertmanager (alert routing)  
↓  
Webhook Receiver  
↓  
Grafana (visualization dashboards)

---

## Project Structure
prometheus-lab/
│
├── alertmanager/
│ └── alertmanager.yml
│
├── prometheus/
│ ├── prometheus.yml
│ └── rules/
│ └── alerts.yml
│
├── docker-compose.yml
└── README.me

---

## How to Run

Start the monitoring stack:
docker compose up -d


Verify running services:
docker compose ps

---

## Web Interfaces

Prometheus  
http://localhost:9090  

Alertmanager  
http://localhost:9093  

Grafana  
http://localhost:3000  

Webhook Receiver  
http://localhost:9999  

---

## Screenshots

### Prometheus Targets
![Prometheus Targets](screenshots/Targets.png)

### Grafana Dashboard
![Grafana Dashboard](screenshots/Grafana.png)

### Alertmanager UI
![Alertmanager UI](screenshots/Alert.png)

---

## Learning Goals

- Understand Prometheus architecture  
- Configure monitoring targets and alert rules  
- Deploy a containerized monitoring stack  
- Visualize metrics using Grafana dashboards  
- Implement alerting workflows using Alertmanager  

---

## Author

Shishir Pariyar  

DevOps / Cloud Engineering Learning Project


