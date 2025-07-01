# Kubernetes Core K8s Modules

## This module is part of the kubernetes.core collection (version 5.3.0).

You might already have this collection installed if you are using the ansible package. It is not included in ansible-core. To check whether it is installed, run ansible-galaxy collection list.

To install it, use: ansible-galaxy collection install kubernetes.core. You need further requirements to be able to use this module, see Requirements for details.

To use it in a playbook, specify: kubernetes.core.k8s.

<br/>

## Synopsis:
Use the Kubernetes Python client to perform CRUD operations on K8s objects. 
Pass the object definition from a source file or inline. See examples for reading files and using Jinja templates or vault-encrypted files.
Access to the full range of K8s APIs.
Use the kubernetes.core.k8s_info module to obtain a list of items about an object of type kind
Authenticate using either a config file, certificates, password or token
Supports check mode.

<br/>

---------------
## Requirements:
python >= 3.9

kubernetes >= 24.2.0

PyYAML >= 3.11

jsonpatch

---------

<br/>


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

<br/>

### This collection provides a powerful foundation for Kubernetes infrastructure automation, enabling teams to implement reliable, repeatable, and scalable cluster management workflows through Ansible's familiar declarative syntax.
