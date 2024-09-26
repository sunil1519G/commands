# GCloud Commands

A collection of Google Cloud CLI commands for managing service accounts and Kubernetes integrations.

## Table of Contents
- [Service Accounts](#service-accounts)
- [Kubernetes Service Accounts](#kubernetes-service-accounts)

### Service Accounts
1. **List Google Cloud service accounts**:
    ```bash
    gcloud iam service-accounts list --project=my-google-project
    ```

### Kubernetes Service Accounts
1. **List Kubernetes service accounts**:
    ```bash
    kubectl get serviceaccounts -n my-namespace
    ```

