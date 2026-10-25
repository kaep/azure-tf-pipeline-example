# Deploy Azure infra using Terraform and GitHub actions

Using a managed identity and federated identity credentials.

## Useful resources

- https://docs.github.com/en/actions/how-tos/secure-your-work/security-harden-deployments/oidc-in-azure
- https://learn.microsoft.com/en-us/entra/workload-id/workload-identity-federation-create-trust-user-assigned-managed-identity?pivots=identity-wif-mi-methods-azp
- https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/guides/service_principal_oidc

## Random notes

- The federated credential entity must be branch for `workflow_dispatch`
- GitHub repo ID can be found in repo page source searching for "octolytics-dimension-repository_id"
