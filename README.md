# Azure Container Apps (ACA) samples
Repo contains sample Azure Container App populating diagnostics data to [Microsoft Azure Application Insights](https://azure.microsoft.com/en-us/services/application-insights/)

* service-a
  Angular.js sample application with Node.js backend. 
* service-b
  node.js sample service.

# Configuration
Provide ```APPINSIGHTS_INSTRUMENTATIONKEY``` in the local.env and release.env
```
APPINSIGHTS_INSTRUMENTATIONKEY=488811fc-e1e1-4ba2-9278-f38ce88559c2
```
If no APPINSIGHTS_INSTRUMENTATIONKEY is provided, diagnostics collection will be disabled

# Stariting App locally
```
docker-compose -f docker-compose.local.yml up --build
```

# Deploying to ACS cluster
TBD