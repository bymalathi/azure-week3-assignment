# Azure Week 3 Assignment

## Objective

This project demonstrates how to build a Docker image and push it to Azure Container Registry (ACR) using Azure DevOps CI pipelines.

---

## Project Structure

```
azure-week3-assignment
│
├── Dockerfile
├── index.html
├── azure-pipelines.yml
└── README.md
```

---

## Technologies Used

- Azure DevOps
- Azure Container Registry (ACR)
- Docker
- GitHub
- Nginx

---

## Microsoft-hosted Agent vs Self-hosted Agent

| Microsoft-hosted Agent | Self-hosted Agent |
|-------------------------|-------------------|
| Managed by Microsoft | Managed by the user |
| Automatically provisioned | Installed on your own machine or VM |
| Clean environment for every run | Reuses the same machine |
| No maintenance required | Requires maintenance and updates |
| Best for most CI/CD pipelines | Best for custom software or private networks |

---

## CI Pipeline Workflow

```
Developer

     │

Git Push

     │

     ▼

GitHub Repository

     │

     ▼

Azure DevOps Pipeline

     │

Checkout Code

     │

Build Docker Image

     │

Push Image

     │

     ▼

Azure Container Registry (ACR)
```

---

## Files

- Dockerfile
- index.html
- azure-pipelines.yml

---

## Outcome

- Docker image built successfully.
- Docker image pushed to Azure Container Registry.
- Azure DevOps pipeline configured for CI.


---

## Docker Image

The application is packaged into a Docker image using the provided Dockerfile.

The Azure DevOps pipeline automatically builds the image and pushes it to Azure Container Registry (ACR).

Image Name:

```
myapp
```

Registry:

```
malathiweek3acr.azurecr.io
```