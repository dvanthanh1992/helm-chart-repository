# 🚀 Helm Chart Repository for GitOps Workflow

This repository manages the Helm charts for deploying and managing applications using a **GitOps** workflow. It is structured to support multiple environments, ensuring seamless deployment across **Development, Quality Control, Staging, and Production**.

## 📂 Repository Structure

```plaintext
helm-chart-repository/
├── thanh-backend-chart
│   ├── Chart.yaml
│   └── env
│       ├── dev
│       │   └── values.yaml
│       ├── prod-hcm
│       │   └── values.yaml
│       ├── prod-hni
│       │   └── values.yaml
│       ├── qc
│       │   └── values.yaml
│       ├── staging
│       │   └── values.yaml
│       └── templates
│           ├── app-deployment.yaml
│           ├── app-service.yaml
│           ├── _helpers.tpl
│           ├── redis-deployment.yaml
│           ├── redis-pvc.yaml
│           ├── redis-service.yaml
│           └── tests
│               └── test-connection.yaml
|
| # Helm Chart for Frontend Service
| # (same structure as backend)
|
├── thanh-frontend-chart/
│   ├── ...
│   └── ...
└── README.md
