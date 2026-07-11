# Merch Deployment Modernization

## Overview

Modernized a collection of manually managed Merch environments into a repeatable, automated deployment platform.

## The problem

Merch instances were initially provisioned and maintained manually by a small number of administrators. This created inconsistent configurations, operational dependencies, and limited scalability.

## Constraints

- Existing production workloads
- Authentication through Active Directory
- TLS and security requirements
- Backup and upgrade requirements
- Multiple independently managed environments
- Need for incremental migration rather than a complete replacement

## Approach

The platform evolved in stages:

1. Documented and standardized existing deployment requirements.
2. Automated server configuration and Merch installation with Ansible.
3. Containerized the database deployment.
4. Migrated suitable workloads into Kubernetes.
5. Introduced Helm-based configuration and CI/CD-managed delivery.

## Technologies

- Merch
- Kubernetes
- Helm
- Ansible
- Docker
- GitHub Actions
- Active Directory and LDAP
- TLS

## Results

This section will describe improvements in repeatability, deployment consistency, operational ownership, recovery, and scalability.

## Lessons learned

This section will cover the benefits of incremental modernization and the tradeoffs involved in operating stateful services in Kubernetes.