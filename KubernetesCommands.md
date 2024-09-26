# Kubernetes Commands

A list of commonly used Kubernetes (K8s) commands for managing containers, jobs, services, and more.

## Table of Contents
- [Pod Management](#pod-management)
- [Cronjobs and Jobs](#cronjobs-and-jobs)
- [Services](#services)
- [Other Useful Commands](#other-useful-commands)
- [K8s Dashboard](#k8s-dashboard)
- [Port-Forwarding](#port-forwarding)

### Pod Management
1. **Restart the container in K8s**:
    ```bash
    kubectl -n <namespace> rollout restart deploy <pod-name/application-name>
    ```

2. **See PODs logs**:
    ```bash
    kubectl logs -n <namespace> <POD-name>
    ```

3. **Describe the POD**:
    ```bash
    kubectl -n <namespace> describe pod <POD-name>
    ```

### Cronjobs and Jobs
1. **Trigger a cronjob manually**:
    ```bash
    kubectl create job --from=cronjob/<cronjob-name> <job-name> -n <namespace-name>
    ```

2. **Get all cronjobs**:
    ```bash
    kubectl get cronjobs -n <namespace>
    ```

3. **Get all jobs**:
    ```bash
    kubectl get jobs -n <namespace>
    ```

### Services
1. **Get all services**:
    ```bash
    kubectl get service -n <namespace>
    ```

### Other Useful Commands
- Get context:
    ```bash
    kubectl config get-contexts
    ```

- Use a specific context:
    ```bash
    kubectl config use-context docker-desktop
    ```

- Get nodes:
    ```bash
    kubectl get nodes
    ```

### K8s Dashboard
1. **Add the Kubernetes dashboard repository**:
    ```bash
    helm repo add kubernetes-dashboard https://kubernetes.github.io/dashboard/
    ```

2. **Install the dashboard**:
    ```bash
    helm upgrade --install kubernetes-dashboard kubernetes-dashboard/kubernetes-dashboard --create-namespace --namespace kubernetes-dashboard
    ```

### Port-Forwarding
1. **Switch context and forward ports**:
    ```bash
    kubectl config use-context $CONTEXT
    kubectl -n $NAMESPACE port-forward service/<service-name> 8088:80
    ```

