## tsys-bookstore-app ##
This project containerizes and deploys a FastAPI-based bookstore application using Docker and Kubernetes. The application is deployed as a multi-container setup with PostgreSQL as the backend database and Adminer for database access.


## Bookstore API – Kubernetes Deployment ##

1. Overview:
This project demonstrates containerization and deployment of a FastAPI-based bookstore application on a Kubernetes cluster. The application was converted into a multi-container setup using PostgreSQL as the database and Adminer for database access.

2. Architecture:
Client -> Ingress (NGINX) -> Service -> FastAPI Pods -> PostgreSQL

3. Key Components:
- FastAPI API service
- PostgreSQL database
- Adminer UI
- Kubernetes for orchestration
- NGINX Ingress for routing

4. Features:
- Multi-container deployment
- ConfigMaps and Secrets for configuration
- Database initialization using SQL
- Ingress-based routing
- Scalable API (multiple replicas)

5. Setup Summary:
I. Build Docker image
II. Create cluster using kind
III. Load image into cluster
IV. Apply Kubernetes manifests
V. Install Ingress Controller
VI. Access application via Ingress

6. Improvements Made:
- Fixed dependency issues
- Resolved Pydantic compatibility
- Improved imports for container runtime
- Fixed API response serialization
- Externalized configuration
