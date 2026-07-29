# Lab 02 – Azure Key Vault and RBAC

## Objective

Securely store and manage secrets in Azure Key Vault using Azure role-based access control.

## Resources Created

- Resource group: `rg-sc500-lab`
- Azure Key Vault: Standard tier
- Test secret: `TestPassword`
- RBAC role: `Key Vault Secrets Officer`

## Security Controls

- Configured Azure RBAC as the Key Vault permission model
- Assigned a least-privilege role for secret management
- Created and securely accessed a secret
- Verified secret versioning
- Used soft delete to support secret recovery

## What I Learned

- How Azure Key Vault protects sensitive information
- The difference between creating a vault and receiving permission to access its secrets
- How Azure RBAC controls Key Vault data access
- How secret versions are created when a secret is updated
- Why secrets should never be stored directly in code or public repositories

## Security Note

No secret values, passwords, subscription IDs, tenant IDs, or personal account information are included in this repository.

## Screenshots

### 1. Azure Key Vault Overview

![Azure Key Vault overview](screenshots/01-key-vault-overview.png)

### 2. RBAC Role Assignments

![Key Vault RBAC role assignments](screenshots/02-key-vault-rbac-role-assignments.png)

### 3. Secret Created

![Key Vault secret created](screenshots/03-key-vault-secret-created.png)

### 4. Secret Versioning

![Key Vault secret versioning](screenshots/04-key-vault-secret-versioning.png)
