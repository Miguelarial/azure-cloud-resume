# Cloud Resume Challenge - Progress Tracker

This repository tracks my progress on the Cloud Resume Challenge. While the project is still a work in progress, I have successfully implemented some key components. Below is an overview of my current progress and the steps I plan to complete next.

## Current Progress

### Static Website
I have deployed my CV as a static website using Azure Static Web Apps. The website is currently live and can be viewed [here](https://victorious-ground-0852d4903.5.azurestaticapps.net).

### CI/CD (Front-end)
I have set up GitHub Actions to automate deployments for my static website. Every time I push new front-end code, the changes are automatically deployed to Azure Static Web Apps. This demonstrates my understanding of CI/CD principles and version control.

## Upcoming Steps

### HTTPS
I plan to enable HTTPS for the Azure Storage website using Azure CDN to enhance security.

### DNS
I will set up a custom domain name that points to the Azure CDN endpoint using Azure DNS.

### JavaScript
I will add a visitor counter that displays how many people have accessed the site. This will require writing and integrating JavaScript into the website.

### Database
To store visitor count data, I will use the Table API of Azure CosmosDB, with serverless capacity mode to keep costs low.

### API
Instead of direct front-end interaction with CosmosDB, I will create an API using Azure Functions with an HTTP trigger. This API will manage the communication between the website and database.

### Python
The API logic will be written in Python and deployed using Azure Functions, which is well-suited for backend processing.

### Tests
I will implement tests for the Python code to ensure smooth functionality between the front-end, API, and database.

### Infrastructure as Code
I plan to define my infrastructure (Azure Functions, CosmosDB, etc.) using an Azure Resource Manager (ARM) template. This will allow me to manage resources efficiently and automate their deployment.

### CI/CD (Back-end)
I will create a separate GitHub repository for my backend code, and set up GitHub Actions to test and deploy the API and database infrastructure whenever updates are pushed.

---

As I continue working on the Cloud Resume Challenge, I am committed to completing the remaining steps to demonstrate a comprehensive understanding of cloud architecture and DevOps principles.

