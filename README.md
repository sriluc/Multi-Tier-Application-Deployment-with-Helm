Set-Content -Path "README.md" -Value @'
# Multi-Tier Application Deployment with Helm

This project demonstrates how to deploy a multi-tier application (frontend, backend, and database) using Helm charts.

## Folder Structure

- `charts/`: Contains Helm charts for the frontend, backend, and database.
  - `frontend/`: Helm chart for the frontend web application.
  - `backend/`: Helm chart for the backend REST API.
  - `database/`: Helm chart for the PostgreSQL database.

## How to Use

1. Install Helm: https://helm.sh/docs/intro/install/
2. Deploy the charts:
   ```bash
   helm install frontend ./charts/frontend
   helm install backend ./charts/backend
   helm install database ./charts/database
Verify the deployment:

bash
Copy
kubectl get pods
kubectl get services
