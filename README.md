# Cloud Resume Challenge - Progress Tracker

This repository is where I am tracking my progress with the Cloud Resume Challenge. Although the project is still a work in progress, I plan to implement all the steps outlined below for the final product.

## Steps Followed for the Cloud Resume Challenge

### HTML
I have structured my resume using HTML.

### CSS
To enhance the appearance of the resume, I styled it using CSS.

### Static Website
I deployed the resume as a static website using Azure Storage and Azure Static Web Apps, utilizing Azure Storage to store the files.

### HTTPS
For added security, I enabled HTTPS on the Azure Storage website URL, using Azure CDN to assist with this. You can view my static website [here]

### DNS
I plan to create a custom domain name pointing to the Azure CDN endpoint using Azure DNS.

### JavaScript
To display how many people have visited the site, I will be adding a visitor counter, which will require writing some JavaScript.

### Database
The visitor counter will need to interact with a database to store and retrieve the visitor count. I will use the Table API of Azure CosmosDB, opting for serverless capacity mode to minimize costs.

### API
Rather than directly interacting with CosmosDB from the front-end, I will create an API that communicates with the database. I plan to build this using Azure Functions with an HTTP trigger.

### Python
The API logic, hosted in Azure Functions, will be written in Python, as it is a widely used language for back-end development and integrates well with the Azure SDK.

### Tests
I will test the Python code to ensure the functionality of the API and database interactions.

### Infrastructure as Code
To efficiently manage my resources, I will define my infrastructure, including the Azure Functions and CosmosDB, using an Azure Resource Manager (ARM) template. This setup will be on a Consumption plan to reduce manual configurations and save time in the future.

### Source Control
I have set up a GitHub repository for my front-end code, allowing for continuous integration and automated updates when I make changes to the website or API.

### CI/CD (Front-end)
I have created GitHub Actions that will automatically update the Azure Storage blob whenever I push changes to the front-end code.

### CI/CD (Back-end)
I will create a separate GitHub repository for the back-end code. GitHub Actions will trigger Python tests when changes are pushed. Once the tests pass, the ARM template and Python code will be packaged and deployed to Azure automatically.

