# Cloud Observability Monitoring Stack

A complete cloud-native monitoring and alerting solution built using Prometheus, Grafana, Alertmanager, Docker, and Node Exporter.

## Tech Stack

- Docker
- Docker Compose
- Prometheus
- Grafana
- Alertmanager
- Node Exporter
- Gmail SMTP

---

## Architecture

Application / Server
        │
        ▼
Node Exporter
        │
        ▼
Prometheus
        │
        ▼
Alertmanager
        │
        ▼
Gmail Notifications

---

## Features

- Real-time CPU Monitoring
- Memory Monitoring
- Storage Monitoring
- Email Alerts
- Alert Recovery Notifications
- Grafana Dashboards
- Dockerized Deployment

---

## Alerts Configured

- High CPU Usage
- High Memory Usage
- High Disk Usage
- Test Alert

---

## Email Notification

Configured using Gmail SMTP with App Password authentication.

---

## Docker Containers

- prometheus
- grafana
- node-exporter
- alertmanager


## Future Improvements

- Slack Notifications
- Microsoft Teams Integration
- Telegram Alerts
- AWS EC2 Deployment
- Terraform Automation
- GitHub Actions CI/CD
