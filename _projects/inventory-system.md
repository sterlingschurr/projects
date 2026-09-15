---
title: Inventory Management System
skills: [python, postgresql, docker, rest-api]
date: 2024-03-01
---

A backend service for tracking warehouse inventory in real time. Built a REST
API in Python, backed by PostgreSQL, containerized with Docker for easy
deployment.

## What it does

- Tracks stock levels across multiple warehouse locations
- Sends low-stock alerts
- Exposes a REST API for integration with other tools

## Notable challenges

Handling concurrent stock updates without race conditions was the trickiest
part — solved with row-level locking in Postgres.
