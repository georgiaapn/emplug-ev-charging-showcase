# EMPlug ⚡ SaaS EV Charging Aggregation Platform

> **Note:** This repository is a public showcase of the EMPlug academic project. Source code is intentionally not included, as the project remains under active academic development in a private team repository.

---

## Overview

**EMPlug** is a SaaS EV Charging Aggregation Platform designed to connect multiple independent EV charging providers into a single unified ecosystem. Evolving from the EMPower platform, EMPlug allows electric vehicle users to discover, compare, navigate to, and reserve charging points across different provider networks via a unified web interface. 

In parallel, it offers dedicated provider management, billing, and API integration capabilities, while empowering platform operators with microservices-based system monitoring, provider oversight, and global analytics.

---

## ✨ Key Features

### 🚗 For EV Drivers
* **Unified Discovery:** Browse and compare charging points from multiple charging provider networks through an interactive map.
* **Secure Authentication:** Sign in securely using a Google account.
* **Advanced Filtering:** Filter charging stations dynamically by availability, charging speed, and connector type.
* **External Navigation:** Seamlessly obtain routing directions to a selected charging point.
* **Real-Time Reservations:** Secure available chargers instantly and track reservation statuses live.

### 🏢 For Charging Providers
* **Provider Dashboard:** Manage company profile, internal users, and API configurations through a dedicated interface.
* **Analytics & Reports:** View provider-specific usage statistics and export analytics data in CSV format.
* **Billing & Invoices:** Inspect detailed invoices, monitor billing records, and settle outstanding balances.

### ⚙️ For Platform Operators
* **Operator Administration:** Access a comprehensive platform administration dashboard to manage registered charging providers.
* **Microservices Monitoring:** Track overall platform health, system metrics, and provider synchronization status in real time.
* **Global Insights:** View aggregate platform analytics and system-wide usage statistics.

---

## 🏗️ Architecture & Technology Stack

EMPlug implements a robust microservices architecture utilizing separate databases per bounded context and asynchronous event-driven communication:

* **Frontend:** Responsive web application for users, providers, and operators built with *Next.js (React, TypeScript), Tailwind CSS, shadcn/ui, MapLibre GL,* and *Recharts*.
* **API Gateway:** Single frontend-facing entry point routing requests and exposing public REST endpoints (*Python, FastAPI, Pydantic, Uvicorn*).
* **Microservices:** Domain-driven independent services (*auth, provider-management, provider-integration, provider-sync, points, reservation, analytics, billing*) built with *Python, FastAPI, SQLAlchemy, Pydantic,* and *Uvicorn*.
* **Databases & Messaging:** Isolated *PostgreSQL* databases per bounded context combined with *RabbitMQ* for asynchronous event handling.
* **Deployment:** Fully containerized multi-service development and deployment environment via *Docker* and *Docker Compose*.

---

## 🌐 Demo



---

## Team [saas26-20]
Software-as-a-Service Technologies, 2025-2026
Electrical & Computer Engineering - NTUA
