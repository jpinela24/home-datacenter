# Home-Datacenter Architecture

## Purpose

This document describes the architecture of Home-Datacenter.

Rather than presenting a single large diagram, the infrastructure is documented using multiple focused diagrams. Each diagram explains one aspect of the environment, making the system easier to understand, maintain, and expand over time.

---

## Architecture Diagrams

The following diagrams will be created:

- Physical Infrastructure
- Network Topology
- Service Architecture
- Storage Layout
- Security Model
- Remote Access


Physical Infrastructure Overview

The Home-Datacenter is built around two primary computing devices that separate infrastructure services from application workloads.

Raspberry Pi 4

Role: Infrastructure Node

The Raspberry Pi hosts lightweight infrastructure services that support the overall environment. Keeping these services separate helps reduce resource usage on the primary application server.

Lenovo ThinkCentre

Role: Application Server

The Lenovo ThinkCentre is the primary Docker host, running self-hosted applications and services used daily.

Network Infrastructure

The environment is connected through a DD-WRT-powered router and a dedicated Gigabit switch, providing reliable internal connectivity between all devices.

The physical layout is documented in the Physical Infrastructure Overview diagram.