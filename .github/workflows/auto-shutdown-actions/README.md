# Autoshutdown System for Azure Resources

### Purpose
This system is created to automatically shutdown resources any time when you want to set it. It's purpose is to turn off certain resources in azure to stop them from incurring cost when it is unused. It shutdowns AKS, PSQL servers and VMs. It also have its manual action that you have the option to shutdown or start a specific resource in a specific environment.

### Configuration
The whole system refers to environment variables configured in a repository. This is to dynamically manage resources and enable reusability.

### Example
An example schenario for this is it automatically shutdowns non-production systems every weekend when no user is working or using the resources. If ever, someone needs it there is a manual option to turn on the resources in github actions. Mitigating the action to turn it manually using CLI or in Azure portal.
