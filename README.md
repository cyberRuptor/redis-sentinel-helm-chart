# Redis Sentinel Helm Chart
![redis](https://github.com/user-attachments/assets/193abfcd-1d28-4e42-8d8b-2eb668064e1d)


## Introduction

This guide provides step-by-step instructions to deploy Redis Sentinel on a Kubernetes cluster using Helm. Redis Sentinel provides high availability and monitoring capabilities for Redis. By using Helm, we simplify the deployment process and manage configurations effortlessly.

## Prerequisites

Before you begin, ensure you have the following:
- A Kubernetes cluster (v1.18+)
- Helm (v3.0+)
- The Image Pull Secret of the registry you are using and add the name of the secret in your service account inside values.yaml.

```shell
  serviceAccount:
  imagePullSecrets:
    name1: <name of your Image Pull Secret>
```

## Installation Process

1. **Add the Helm Repository**

   ```sh
   helm repo add my-repo https://charts.example.com/
   helm repo update
```
