## Reference Architecture Context

This repository aligns with the reference architecture presented in the article "Reference Architecture for the Design and Implementation of AI Systems in Manufacturing" by Mateo-Casalía et al. This architecture facilitates the integration of AI systems in production environments, addressing the complexities of Industry 4.0 and ensuring compliance with standards such as ISO/IEC 42001.

The Helm charts provided here offer a practical implementation framework for deploying key components within a Kubernetes cluster, supporting the deployment of AI models, data management systems, and monitoring tools essential for modern manufacturing systems.

## Reference Architecture for the Design and Implementation of AI Systems in Manufacturing" by Mateo-Casalía et al.

The article 'Reference Architecture for the Design and Implementation of AI Systems in Manufacturing' discusses the adoption of Industry 4.0 in manufacturing, highlighting the integration of technologies such as IoT, artificial intelligence and advanced robotics to create smart factories. Despite these advances, digital asset management and the effective implementation of AI in industry remain complex challenges. To address these challenges, the authors present a framework based on standards such as ISO/IEC 42001 that provides practical guidelines for the selection and implementation of AI systems, and a case study of a metal manufacturing company in Valencia, Spain.

The proposal includes a reference architecture structured in four levels: model, AI system, AI system environment, and physical and digital environment. It describes 15 essential components for AI implementation, covering aspects such as user access control and performance monitoring. The article concludes that the adoption of a robust and standardised framework is crucial for digital transformation in industry, and suggests future research to incorporate emerging technologies and address the socio-economic implications of AI in the manufacturing sector.

## Overview

This repository contains a collection of Helm charts for deploying various applications within a Kubernetes cluster. The applications included are Node-RED, PostgreSQL, Grafana, Keycloak, Minio, MongoDB, MySQL, RabbitMQ, Kafka, and Prometheus.

These Helm charts are designed to streamline the deployment process and ensure that all necessary resources, services, and configurations are properly set up.

## Chart Structure

The directory structure of the Helm charts is as follows:

```
my-chart/
  ├── Chart.yaml
  ├── values.yaml
  ├── templates/
      ├── nodered-deployment.yaml
      ├── nodered-service.yaml
      ├── nodered-ingress.yaml
      ├── nodered-pvc.yaml
      ├── postgres-deployment.yaml
      ├── postgres-service.yaml
      ├── postgres-pvc.yaml
      ├── grafana-deployment.yaml
      ├── grafana-service.yaml
      ├── grafana-ingress.yaml
      ├── grafana-pvc.yaml
      ├── keycloak-deployment.yaml
      ├── keycloak-service.yaml
      ├── keycloak-ingress.yaml
      ├── keycloak-pvc.yaml
      ├── minio-deployment.yaml
      ├── minio-service.yaml
      ├── minio-pvc.yaml
      ├── mongodb-deployment.yaml
      ├── mongodb-service.yaml
      ├── mongodb-pvc.yaml
      ├── mysql-deployment.yaml
      ├── mysql-service.yaml
      ├── mysql-pvc.yaml
      ├── rabbitmq-deployment.yaml
      ├── rabbitmq-service.yaml
      ├── rabbitmq-pvc.yaml
      ├── kafka-deployment.yaml
      ├── kafka-service.yaml
      ├── kafka-pvc.yaml
      ├── prometheus-deployment.yaml
      ├── prometheus-service.yaml
      ├── prometheus-pvc.yaml
      └── prometheus-ingress.yaml
```

## Prerequisites

- Kubernetes 1.18+
- Helm 3.0+
- Persistent Volume provisioner support in the underlying infrastructure

## Installation

To install a chart with the release name `my-release`, use the following command:

```sh
helm install my-release ./my-chart
```

## Configuration

The `values.yaml` file contains the default configuration values for the charts. You can customize the values by editing this file or by providing your own `values.yaml` file during the installation.

### Example

To override values during the installation, use the `--values` or `-f` flag:

```sh
helm install my-release ./my-chart --values my-values.yaml
```

## Applications

### Node-RED

- **Deployment**: `templates/nodered-deployment.yaml`
- **Service**: `templates/nodered-service.yaml`
- **Ingress**: `templates/nodered-ingress.yaml`
- **Persistent Volume Claim**: `templates/nodered-pvc.yaml`

### PostgreSQL

- **Deployment**: `templates/postgres-deployment.yaml`
- **Service**: `templates/postgres-service.yaml`
- **Persistent Volume Claim**: `templates/postgres-pvc.yaml`

### Grafana

- **Deployment**: `templates/grafana-deployment.yaml`
- **Service**: `templates/grafana-service.yaml`
- **Ingress**: `templates/grafana-ingress.yaml`
- **Persistent Volume Claim**: `templates/grafana-pvc.yaml`

### Keycloak

- **Deployment**: `templates/keycloak-deployment.yaml`
- **Service**: `templates/keycloak-service.yaml`
- **Ingress**: `templates/keycloak-ingress.yaml`
- **Persistent Volume Claim**: `templates/keycloak-pvc.yaml`

### Minio

- **Deployment**: `templates/minio-deployment.yaml`
- **Service**: `templates/minio-service.yaml`
- **Persistent Volume Claim**: `templates/minio-pvc.yaml`

### MongoDB

- **Deployment**: `templates/mongodb-deployment.yaml`
- **Service**: `templates/mongodb-service.yaml`
- **Persistent Volume Claim**: `templates/mongodb-pvc.yaml`

### MySQL

- **Deployment**: `templates/mysql-deployment.yaml`
- **Service**: `templates/mysql-service.yaml`
- **Persistent Volume Claim**: `templates/mysql-pvc.yaml`

### RabbitMQ

- **Deployment**: `templates/rabbitmq-deployment.yaml`
- **Service**: `templates/rabbitmq-service.yaml`
- **Persistent Volume Claim**: `templates/rabbitmq-pvc.yaml`

### Kafka

- **Deployment**: `templates/kafka-deployment.yaml`
- **Service**: `templates/kafka-service.yaml`
- **Persistent Volume Claim**: `templates/kafka-pvc.yaml`

### Prometheus

- **Deployment**: `templates/prometheus-deployment.yaml`
- **Service**: `templates/prometheus-service.yaml`
- **Ingress**: `templates/prometheus-ingress.yaml`
- **Persistent Volume Claim**: `templates/prometheus-pvc.yaml`



