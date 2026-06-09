## Bookstore API - Kubernetes Deployment ##

Overview:
This project demonstrates containerization and deployment of a FastAPI-based bookstore application on a Kubernetes cluster. The application was converted into a multi-container setup using PostgreSQL as the database and Adminer for database access.

1. Architecture:
Client -> Ingress (NGINX) -> Service -> FastAPI Pods -> PostgreSQL

2. Key Components:
- FastAPI API service
- PostgreSQL database
- Adminer UI
- Kubernetes for orchestration
- NGINX Ingress for routing

3. Features:
- Multi-container deployment
- ConfigMaps and Secrets for configuration
- Database initialization using SQL
- Ingress-based routing
- Scalable API (multiple replicas)

4. Setup Summary:
I. Build Docker image
II. Create cluster using kind
III. Load image into cluster
IV. Apply Kubernetes manifests
V. Install Ingress Controller
VI. Access application via Ingress

5. Improvements Made:
- Fixed dependency issues
- Resolved Pydantic compatibility
- Improved imports for container runtime
- Fixed API response serialization
- Externalized configuration
