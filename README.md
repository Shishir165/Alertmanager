Prometheus Monitoring Lab
Overview

This project demonstrates a basic monitoring stack using Prometheus and Alertmanager running in Docker.
It simulates application metrics, collects them with Prometheus, and triggers alerts that are sent to a webhook receiver.

The goal of this lab is to practice modern DevOps monitoring concepts such as metrics collection, alerting, and containerized observability setups.

Tech Stack

Prometheus (metrics collection)

Alertmanager (alert routing and notification)

Node Exporter (system metrics)

Docker & Docker Compose

Webhook Sink (simulated alert receiver)

Architecture

Application → Prometheus → Alertmanager → Webhook Receiver

Prometheus scrapes metrics from the application and exporters, evaluates alert rules, and sends alerts to Alertmanager which then forwards notifications.

How to Run

Clone the repository and start the monitoring stack:

docker compose up -d

Check running services:

docker compose ps
Web Interfaces

Prometheus UI
http://localhost:9090

Alertmanager UI
http://localhost:9093

Webhook Sink (alert receiver)
http://localhost:9999

Learning Goals

Understand Prometheus architecture

Configure monitoring targets and alert rules

Use Docker Compose to orchestrate monitoring services

Troubleshoot container networking and port conflicts

Author
Shishir Pariyar

DevOps / Cloud Engineering Learning Project