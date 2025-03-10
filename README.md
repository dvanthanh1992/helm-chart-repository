# 🚀 Helm Chart Repository for GitOps Workflow

This repository manages the Helm charts for deploying and managing applications using a **GitOps** workflow. It is structured to support multiple environments, ensuring seamless deployment across **Development, Staging, and Production**.

## 📂 Repository Structure

```plaintext
helm-chart-repository/
├── thanh-backend-chart/            # Helm Chart for Backend Service
│   ├── Chart.yaml                  # Metadata for the Helm Chart
│   ├── dev/                        # Dev specific values
│   │   └── values.yml
│   ├── staging/                    # Staging specific values
│   │   └── values.yml
│   ├── prod-hcm/                   # HCM-Production specific values
│   │   └── values.yml
│   ├── prod-hni/                   # HNI-Production specific values
│   │   └── values.yml
│   ├── templates/                  # Kubernetes resource templates
│   │   ├── deployment.yaml         # Deployment manifest
│   │   ├── service.yaml            # Service manifest
│   │   ├── _helpers.tpl            # Template helpers
│   │   └── tests/                  # Tests for Helm chart
│           └── test-connection.yaml
├── thanh-frontend-chart/    # Helm Chart for Frontend Service (same structure as backend)
│
└── README.md                # Documentation
