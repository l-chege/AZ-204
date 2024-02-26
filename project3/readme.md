# Implement Azure Security
Azure reources:
- Microsoft Identity platform (for user authentication and authorization)
- Microsoft Azure Active Directory (Azure AD)
- Microsoft Graph (for solutions that interact with it)
- Azure Key Vault (for securing app configuration data)
- Managed Identities for Azure resources

## Project - Secrets Notes Viewer
A web app that displays secret notes from Azure keyvault only when user logins.

### Infrastructure Used
- Microsoft Azure Active Directory (User authentication)
- Azure Key Vault (Storing sensitive data)
- Azure App Service (Hosting the portal)

### Implemetation Guide
- Set up an Azure AD instance for user authentication.
- Create several test users in Azure AD.
- Create several secrets in Azure KeyVault.
- Assign permissions to users in Azure AD such that each user has access to different secrets.
- Develop a web application that integrates with Azure AD for login functionality.
- Integrate Azure Key Vault in the application to fetch configuration data.
- Display the information in the web app once user logins.
- Deploy the application on Azure App Service.
- Setup a CI/CD pipeline for your application
- Setup Application insights and Azure monitor
- Push to GitHub
- Document