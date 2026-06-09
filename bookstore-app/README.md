Bookstore API – Kubernetes Deployment

Overview
This project demonstrates containerization and deployment of a FastAPI-based bookstore application on a Kubernetes cluster. The application was converted into a multi-container setup using PostgreSQL as the database and Adminer for database access.

Architecture
Client -> Ingress (NGINX) -> Service -> FastAPI Pods -> PostgreSQL

Key Components
- FastAPI API service- PostgreSQL database- Adminer UI- Kubernetes for orchestration- NGINX Ingress for routing
Features
- Multi-container deployment- ConfigMaps and Secrets for configuration- Database initialization using SQL- Ingress-based routing- Scalable API (multiple replicas)
Setup Summary
1. Build Docker image2. Create cluster using kind3. Load image into cluster4. Apply Kubernetes manifests5. Install Ingress Controller6. Access application via Ingress
Improvements Made
- Fixed dependency issues- Resolved Pydantic compatibility- Improved imports for container runtime- Fixed API response serialization- Externalized configuration
