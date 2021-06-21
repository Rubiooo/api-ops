# API Ops
> EKS cluster, ECR repository, and Flux management for `Rubiooo/api`

## About

This repository contains a GitHub Actions workflow ([`setup.yaml`](.github/workflows/setup.yml)) that creates an EKS cluster and ECR repository upon `workflow_dispatch`. Self hosted runner "ECR Create" is used in this workflow to communicate to a pre-configured instance of Vault using an AppRole with the `ecr-create` policy. See [`rubiooo/vault-runner-setup`](https://github.com/Rubiooo/vault-runner-setup) for details.

The EKS cluster infrastructure definition is in [`cluster.yaml`](cluster.yaml).

