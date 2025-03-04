# helm-chart-repository


# 🚀 Helm Chart Repository for GitOps Workflow

This repository manages the Helm charts for deploying and managing applications using a **GitOps** workflow. It is structured to support multiple environments, ensuring seamless deployment across **Development, Staging, and Production**.

## 📂 Repository Structure

```plaintext
helm-chart-repository/
├── thanh-backend-chart/            # Helm Chart for Backend Service
│   ├── Chart.yaml                  # Metadata for the Helm Chart
│   ├── values.yml                  # Default values for the chart
│   ├── dev/                        # Dev specific values
│   ├── staging/                    # Staging specific values
│   ├── prod-hcm/                   # HCM-Production specific values
│   ├── prod-hni/                   # HNI-Production specific values
│   ├── templates/                  # Kubernetes resource templates
│   │   ├── deployment.yaml         # Deployment manifest
│   │   ├── service.yaml            # Service manifest
│   │   ├── ingress.yaml            # Ingress rules
│   │   ├── hpa.yaml                # Horizontal Pod Autoscaler
│   │   ├── _helpers.tpl            # Template helpers
│   │   ├── serviceaccount.yaml     # Service Account
│   │   ├── NOTES.txt               # Notes for Helm users
│   │   └── tests/                  # Tests for Helm chart
│   └── values.yml                  # Global values
│
├── thanh-frontend-chart/    # Helm Chart for Frontend Service (same structure as backend)
│
└── README.md                # Documentation
