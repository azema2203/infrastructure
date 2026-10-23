# DevOps Infrastructure Repository

Полноценный DevOps-репозиторий: Infrastructure as Code, конфигурация серверов,
контейнеризация, оркестрация и CI/CD.

## 📚 Стек

| Компонент      | Технология              |
|----------------|-------------------------|
| IaC            | Terraform               |
| Configuration  | Ansible                 |
| Orchestration  | Kubernetes              |
| Containers     | Docker                  |
| Monitoring     | Prometheus              |
| CI/CD          | GitHub Actions          |

## 📂 Структура

```
infrastructure/
├── terraform/        # IaC (AWS S3 + EC2)
├── ansible/          # Provisioning
├── kubernetes/       # Manifests
├── docker/           # Dockerfile
├── monitoring/       # Prometheus config
├── docs/             # Документация
└── .github/workflows # CI
```

## 🚀 Быстрый старт

```bash
git clone https://github.com/<you>/infrastructure.git
cd infrastructure

# Terraform
cd terraform && terraform init && terraform plan

# Ansible
cd ../ansible && ansible-playbook -i inventory.ini playbook.yml

# Docker
cd ../docker && docker build -t infra-app:latest .

# Kubernetes
kubectl apply -f ../kubernetes/
```

## 🔀 Ветвление

- `main` — стабильная ветка (protected)
- `feature/*` — новая функциональность
- `fix/*` — исправления

## 📖 Документация

- [Deployment Guide](docs/DEPLOYMENT.md)
- [Contributing](docs/CONTRIBUTING.md)

## 📜 Лицензия

MIT