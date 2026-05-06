# 3-Tier Finance Application

## Overview

The 3-Tier Finance Application is a microservices-based application designed to provide a seamless experience for managing financial transactions. This sample app includes three primary services: User Service, Transaction Service, and Notification Service, along with a Frontend that allows users to interact with the backend services. This application is developed and deployed using Docker and Kubernetes, with Google Cloud Platform (GCP) as the cloud provider.

## Architecture

This application follows a 3-tier architecture:

1. **Frontend**: A React-based UI that interacts with backend services.
2. **Backend Services**:
   - **User Service**: Manages user authentication and profiles.
   - **Transaction Service**: Handles financial transactions and related operations.
   - **Notification Service**: Sends notifications (e.g., email, SMS) for transaction updates and alerts.
3. **Database**: SQLite is used for data persistence in this example.

## Technology Stack

- **Frontend**: React
- **Backend**: FastAPI
- **Containerization**: Docker
- **Orchestration**: Kubernetes
- **Cloud Provider**: Google Cloud Platform (GCP)
- **CI/CD**: GitHub Actions for automated Docker builds and Kubernetes deployments
- **Infrastructure as Code**: Terraform for creating GKE clusters and managing resources
- **Secrets Management**: Google Secrets Manager for secure configuration management

## CI/CD Pipeline

- **CI**: GitHub Actions automates Docker image building and pushes to Google Container Registry (GCR). It includes linting and testing workflows.
- **CD**: GitHub Actions deploys the services to Google Kubernetes Engine (GKE).
- **Infrastructure**: Terraform is used to create and manage GKE clusters and other necessary resources.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- [Docker](https://www.docker.com/get-started)
- [Kubernetes](https://kubernetes.io/docs/setup/)
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
- [Helm](https://helm.sh/docs/intro/install/) (for monitoring setup)
- [Terraform](https://www.terraform.io/downloads.html)
an start exploring metrics for CPU, memory usage, request rate, and other Kubernetes and application metrics.
