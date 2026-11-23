# Project 18 - GitOps Infrastructure Deployment Using GitHub Actions

## Overview

This project demonstrates a GitOps-based infrastructure deployment workflow using GitHub Actions and GitHub Environments.

The deployment process is automatically triggered when a Pull Request is merged into the main branch. Prior to deployment execution, an approval gate is enforced using GitHub Environment protection rules to ensure controlled and secure infrastructure changes.

This implementation reflects industry-standard GitOps practices commonly adopted in modern DevOps environments.

---

## Objectives

- Implement GitOps workflow automation
- Trigger deployments after Pull Request merges
- Configure deployment approval gates
- Simulate infrastructure deployment using GitHub Actions
- Demonstrate controlled production deployment practices

---

## Technologies Used

- Git
- GitHub
- GitHub Actions
- GitHub Environments
- YAML

---

## Repository Structure

```text
project18-manjusrikalapala-gitops-infra-deployment
│
├── README.md
│
└── .github
    └── workflows
        └── gitops.yml
```

---

## Workflow Process

Developer Change
        ↓
Feature Branch
        ↓
Pull Request
        ↓
Code Review
        ↓
Merge to Main
        ↓
GitHub Actions Trigger
        ↓
Approval Required
        ↓
Infrastructure Apply Job
        ↓
Deployment Complete

---

## Deployment Strategy

The workflow listens for Pull Request closure events. If the Pull Request is successfully merged into the main branch, GitHub Actions initiates the deployment workflow.

A protected GitHub Environment named `production` is configured with mandatory reviewer approvals before deployment execution.

---

## Expected Outcome

- Automated deployment execution after PR merge
- Manual approval before deployment
- Successful workflow execution
- Deployment logs available within GitHub Actions

---

## Deliverables

- GitHub Actions Workflow
- Protected Production Environment
- Pull Request Merge Process
- Approval-Based Deployment
- Successful Workflow Run Screenshot

---

## Author

Manjusri Kalapala

Advanced App Engineering Analyst

## Change History

### Update 1

Added deployment approval workflow demonstration for GitOps implementation.

