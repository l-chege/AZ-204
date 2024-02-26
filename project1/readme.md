# Develop for Azure Compute Solutions
Azure Resources:
- Azure container registry
- Azure container instance
- Azure container apps
- Azure app service web apps
- Azure functions

## Project - Weather Tracker
A web app that allows users to track weather udates in real-time for their chosen cities. The system also triggers azure functions for alerts when a specified weather threshold is met (ie if its going to rain).

### Infrastructure used:
- Azure App Service Web App (Hosting the web application)
- Azure Container Registry (Storing Docker images for the app)
- Azure Container Instance (Running the containers for development/testing)
- Azure Functions (Weather alert system)
- Azure Container Apps (Running the containers in production)

### Implementation Guide 
1. Create an Azure App Service Web App.
2. Develop a basic web application that uses weather APIs.
3. Containerize the application.
4. Publish the container image to Azure Container Registry.
5. Test the application using Azure Container Instance.
6. Implement an Azure Function to send alerts when a specified weather threshold is met.
7. Integrate Azure Function with your web application.
8. Deploy the web application to Azure Container Apps.
9. Setup a CI/CD pipeline for your application and Function.
10. Setup Application insights and Azure monitor
11. Push to GitHub
12. Document
