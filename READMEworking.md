#working flow
            👨‍💻 You
               │
      terraform apply
               │
               ▼
         Terraform
               │
               ▼
           AWS API
               │
               ▼
        EC2 Instance Created
               │
               ▼
      user_data Script Runs
               │
               ▼
 Install Docker + Docker Compose
               │
               ▼
 docker-compose up -d
               │
               ▼
 ┌──────────────────────────────────┐
 │          Docker Containers       │
 │                                  │
 │  Node Exporter                   │
 │  Prometheus                      │
 │  Alertmanager                    │
 │  Grafana                         │
 └──────────────────────────────────┘
               │
               ▼
 Node Exporter collects metrics
               │
               ▼
 Prometheus scrapes metrics
               │
               ▼
 Checks Alert Rules
               │
      ┌────────┴────────┐
      │                 │
  Rule False       Rule True
      │                 │
      │                 ▼
      │          Alertmanager
      │                 │
      │                 ▼
      │        📧 Email Alert
      │
      ▼
 Grafana (when opened)
      │
      ▼
 Dashboard
      │
      ▼
     👨‍💻 You
