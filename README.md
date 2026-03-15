
# Azure Cloud Resume Challenge — Frontend Website

This repository contains the frontend for the Azure Cloud Resume Challenge: a static resume website enhanced with a serverless visitor counter running on the backend API. 

The project demonstrates cloud architecture, Infrastructure as a Code, CI/CD automation, and secure cloud deployment practices. 

## Architecture Overview
The website is deployed as a static site on Azure Storage and available globalle thourhg Azure CDN. Frontend files connects with a backend API hosted on Azure Functions, recording and returning unique visitors count stored in CosmosDB.

Web browser
   │
   ▼
Azure CDN
   │
   ▼
Azure Storage Static Website ($web)
   │
   ▼
Visitor Counter JavaScript
   │
   ▼
Azure Function API
   │
   ▼
Azure Cosmos DB

## Technologies Used

### Frontend

HTML, CSS, JavaScript

### Cloud Platform
Azure Storage Static Website, Azure CDN, Azure Functions, Azure Cosmos DB

### Infrastructure as Code
Terraform, remote state stored in Azure Storage, 

###
CI/CD, GitHub Actions, automated deployments on push to main

### Testing

Cypress End-to-End tests

### Security

Service principals with least-privilege RBAC with separate identities for:
- Terraform state access
- frontend deployment

SBOM generation with Syft, vulnerability scanning with Grype
