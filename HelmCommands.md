# Helm Commands

A collection of useful Helm commands for managing Kubernetes packages.

## Table of Contents
- [Basic Commands](#basic-commands)
- [Release Management](#release-management)
- [Secrets and Values](#secrets-and-values)

### Basic Commands
1. **Create a Helm chart**:
    ```bash
    helm create <chart-name>
    ```

2. **Render templates for the current chart**:
    ```bash
    helm template .
    ```

### Release Management
1. **Install a Helm chart**:
    ```bash
    helm install <release-name> <chart-dir>
    ```

2. **List all releases**:
    ```bash
    helm list
    ```

3. **Upgrade a release**:
    ```bash
    helm upgrade <existing-release> <chart-dir>
    ```

4. **Rollback to a previous release**:
    ```bash
    helm rollback <release-name> <revision>
    ```

### Secrets and Values
1. **Edit Helm secrets**:
    ```bash
    helm secrets edit my-secrets.yaml
    ```

2. **Show chart values**:
    ```bash
    helm show values oci://xyz/helm-charts/my-app --version vX.XX.X
    ```

