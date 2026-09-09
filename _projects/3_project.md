---
layout: page
title: Attendant & Evaluation Dashboards
description: Real-time unit attendance monitoring, monthly KPI evaluation algorithms, ticket resolution analytics, and automated DOCX/Excel parsing.
img: assets/img/6.jpg
importance: 1
category: Data & Automation
related_publications: false
---

### System Architecture & Overview

A specialized technical management intelligence suite providing organizational visibility into staff attendance metrics, monthly performance scorecards, and helpdesk SLA ticketing.

### Key Engineering Features
- **Automated Persian DOCX Ingestion:** Custom parsing pipeline extracting data from unstructured Persian Word (`.docx`) reports and biometric hardware time-clocks, converting them into structured, uncorrupted Excel workbooks and relational database rows.
- **KPI Evaluation Engine:** Algorithmic calculation of monthly departmental performance indexes, attendance compliance rates, and trend projections over historical quarters.
- **Helpdesk Lifecycle Metrics:** Real-time ticketing dashboards tracking average time to resolution (MTTR), technician load heatmaps, and priority escalation workflows.
- **Reporting & Visualizations:** Dynamic data charts powered by Chart.js / ECharts with one-click export to PDF and cleanly formatted Excel files.

### Tech Stack
`Python` `FastAPI` `Pandas` `openpyxl` `python-docx` `React` `Docker` `ECharts`
