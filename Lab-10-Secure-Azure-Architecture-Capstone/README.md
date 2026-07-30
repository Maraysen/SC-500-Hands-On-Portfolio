
# Lab 10 – Secure Azure Architecture Capstone

## Objective

Combine identity, secret management, RBAC, governance, networking, and monitoring controls into one secure Azure environment.

## Architecture Overview

The environment includes:

- Azure App Service
- System-assigned managed identity
- Azure Key Vault
- Azure RBAC
- Azure Policy
- Log Analytics workspace
- Diagnostic settings
- Network security groups
- Virtual network
- Storage account

## What I Implemented

1. Reviewed all resources inside `rg-sc500-lab`.
2. Confirmed the Web App had a system-assigned managed identity.
3. Granted the Web App the `Key Vault Secrets User` role.
4. Stored a test secret securely in Azure Key Vault.
5. Configured the Web App to use a Key Vault reference.
6. Confirmed the Key Vault reference resolved successfully.
7. Applied an Azure Policy restricting deployments to `Australia East`.
8. Configured Key Vault diagnostic logs to flow into Log Analytics.
9. Confirmed Key Vault audit events were successfully collected.

## Secure Access Flow

The Web App uses its managed identity to authenticate to Microsoft Entra ID.

Azure Key Vault checks the identity’s RBAC permissions before allowing access to the secret.

The application uses a Key Vault reference instead of storing the actual secret in its configuration.

```text
Azure Web App
      |
      | Managed Identity
      v
Microsoft Entra ID
      |
      | Access token
      v
Azure Key Vault
      |
      | Key Vault Secrets User
      v
Secret securely retrieved
