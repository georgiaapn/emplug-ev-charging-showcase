# EMPlug ⚡ SaaS EV Charging Aggregation Platform

> **Note:** This repository is a public showcase of the EMPlug academic project. Source code is intentionally not included, as the project remains under active academic development in a private team repository.

---

## Overview

**EMPlug** is a SaaS EV Charging Aggregation Platform designed to connect multiple independent EV charging providers into a single unified ecosystem. As the direct evolution and microservices-based expansion of **[EMPower](https://github.com/georgiaapn/empower-ev-charging-showcase)**, EMPlug allows electric vehicle users to discover, compare, navigate to, and reserve charging points across different provider networks via a unified web interface. 

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

#### Home page:
<img width="1895" height="865" alt="HP" src="https://github.com/user-attachments/assets/1ee8049f-dc37-41e5-8b82-a2b163d911a6" />

#### Health check:

* Failure: <img width="1881" height="1059" alt="failed service" src="https://github.com/user-attachments/assets/e235202c-6179-45e3-963a-fa64a5eb617c" />
* Success: <img width="1881" height="869" alt="success" src="https://github.com/user-attachments/assets/eabfb0f7-6dba-4c64-84b9-8381a4fd1bba" />

#### Operator's settings:
<img width="1900" height="627" alt="op_settings" src="https://github.com/user-attachments/assets/591eb282-6679-4dd1-a516-d6e413207cc0" />

#### Operator's analytics:
<img width="1763" height="1570" alt="op_analytics" src="https://github.com/user-attachments/assets/4b5ae674-626a-4bfb-a196-bf378fb27b35" />

#### Operator's providers:
<img width="1763" height="805" alt="op_providers" src="https://github.com/user-attachments/assets/c4b60e89-528f-43cf-8d28-36606318b146" />

#### Operator clicks on a provider's details:
<img width="1763" height="805" alt="op_prov_details" src="https://github.com/user-attachments/assets/96818ec3-aaa8-484b-b257-3a86524e7438" />

#### Provider admin's dashboard:
<img width="1903" height="772" alt="pr_admin" src="https://github.com/user-attachments/assets/80041ead-0626-41d1-9d1c-05203f0d2bfc" />

#### Provider admin's analytics:
<img width="1763" height="1251" alt="pr_analytics" src="https://github.com/user-attachments/assets/c485922e-7d10-40be-88b3-976cde8c0527" />

#### Provider admin's billing:
<img width="1763" height="933" alt="pr_billing" src="https://github.com/user-attachments/assets/72565645-52b5-4dd1-a5b2-fa9337beb147" />

#### Account configuration:
<img width="1763" height="1200" alt="account" src="https://github.com/user-attachments/assets/789df370-0a15-4307-ae47-ab55f5c9c87f" />












---

## Team [saas26-20]
Software-as-a-Service Technologies, 2025-2026
Electrical & Computer Engineering - NTUA
