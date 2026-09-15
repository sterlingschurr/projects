---
title: Deployment Toolkit
skills: [docker, bash, github-actions]
date: 2024-06-15
---

A set of scripts and GitHub Actions workflows for automating deployments to
a small self-hosted server fleet.

## What it does

- One-command deploys triggered by a GitHub Action on merge to `main`
- Automatic rollback if health checks fail
- Zero-downtime container swaps via Docker
