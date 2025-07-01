# Kubernetes Core K8s Modules

## Overview:
The kubernetes.core.k8s collection provides a comprehensive set of Ansible modules for managing Kubernetes resources. These modules enable infrastructure-as-code approaches to Kubernetes cluster management, allowing you to declaratively define, deploy, and manage Kubernetes objects through Ansible playbooks.

## Collection Structure:
The kubernetes.core collection contains modules that interact with Kubernetes API servers to perform CRUD (Create, Read, Update, Delete) operations on Kubernetes resources. The primary module is k8s, which serves as a universal interface for managing any Kubernetes resource type.

## Key Modules:

The main module for managing Kubernetes resources. It can handle any Kubernetes API object including:

Deployments
Services
ConfigMaps
Secrets
Pods
Namespaces
Ingress resources
Custom Resource Definitions (CRDs)
And any other Kubernetes resource

## k8s_info Module:
Used for gathering information about existing Kubernetes resources. This module is essential for:

## Querying resource states:
Retrieving configuration details
Fact gathering for conditional operations
Monitoring and validation tasks

## State Management:
The modules follow Ansible's idempotent principles:

present: Ensures the resource exists with specified configuration
absent: Ensures the resource is removed
patched: Applies specific modifications to existing resources

## Key Modules:

The main module for managing Kubernetes resources. It can handle any Kubernetes API object including:

Deployments
Services
ConfigMaps
Secrets
Pods
Namespaces
Ingress resources
Custom Resource Definitions (CRDs)
And any other Kubernetes resource

## This collection provides a powerful foundation for Kubernetes infrastructure automation, enabling teams to implement reliable, repeatable, and scalable cluster management workflows through Ansible's familiar declarative syntax.
