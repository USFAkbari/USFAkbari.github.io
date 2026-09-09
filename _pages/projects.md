---
layout: page
title: projects
permalink: /projects/
description: Featured engineering projects, cloud architectures, data automation pipelines, and AI research.
nav: true
nav_order: 2
---

<div class="projects-list my-3">

  <!-- Project 1 -->
  <div class="card mb-4 p-4 border shadow-sm hoverable">
    <div class="d-flex flex-wrap justify-content-between align-items-center mb-2">
      <h4 class="card-title font-weight-bold mb-1">
        <a href="/projects/1_project/" class="text-primary text-decoration-none">Work-State Enterprise Engine</a>
      </h4>
      <span class="badge badge-primary px-2 py-1">Full-Stack & Systems</span>
    </div>
    <p class="card-text text-muted mb-2" style="line-height: 1.5;">
      • <strong>Core Purpose:</strong> Enterprise workflow &amp; task status orchestration platform for high-concurrency environments.<br>
      • <strong>Key Capabilities:</strong> Modular async FastAPI backend, PostgreSQL with connection pooling &amp; Alembic migrations, React 18 SPA with real-time optimistic state mutations.<br>
      • <strong>Security &amp; Deploy:</strong> JWT token isolation, bcrypt password hashing, and multi-stage Docker containerization with automated Pytest suites.
    </p>
    <div class="d-flex flex-wrap gap-1 mt-2">
      <span class="badge badge-light border">FastAPI</span>
      <span class="badge badge-light border">Python 3.11</span>
      <span class="badge badge-light border">React 18</span>
      <span class="badge badge-light border">PostgreSQL</span>
      <span class="badge badge-light border">Docker</span>
      <span class="badge badge-light border">Alembic</span>
    </div>
  </div>

  <!-- Project 2 -->
  <div class="card mb-4 p-4 border shadow-sm hoverable">
    <div class="d-flex flex-wrap justify-content-between align-items-center mb-2">
      <h4 class="card-title font-weight-bold mb-1">
        <a href="/projects/2_project/" class="text-primary text-decoration-none">Appliance Store Platform</a>
      </h4>
      <span class="badge badge-primary px-2 py-1">Full-Stack & Systems</span>
    </div>
    <p class="card-text text-muted mb-2" style="line-height: 1.5;">
      • <strong>Core Purpose:</strong> High-performance e-commerce catalog and retail back-office engine for home appliance distribution.<br>
      • <strong>Key Capabilities:</strong> Multi-faceted relational filtering (brand, specs, price), real-time stock reservation, and ACID payment gateway checkout.<br>
      • <strong>Architecture:</strong> Mobile-first lightweight frontend optimized for low-bandwidth networks with role-based administrative inventory triggers.
    </p>
    <div class="d-flex flex-wrap gap-1 mt-2">
      <span class="badge badge-light border">Python</span>
      <span class="badge badge-light border">JavaScript</span>
      <span class="badge badge-light border">PostgreSQL</span>
      <span class="badge badge-light border">REST API</span>
      <span class="badge badge-light border">Docker</span>
      <span class="badge badge-light border">TailwindCSS</span>
    </div>
  </div>

  <!-- Project 3 -->
  <div class="card mb-4 p-4 border shadow-sm hoverable">
    <div class="d-flex flex-wrap justify-content-between align-items-center mb-2">
      <h4 class="card-title font-weight-bold mb-1">
        <a href="/projects/3_project/" class="text-primary text-decoration-none">Attendant &amp; Evaluation Dashboards</a>
      </h4>
      <span class="badge badge-success px-2 py-1">Data & Automation</span>
    </div>
    <p class="card-text text-muted mb-2" style="line-height: 1.5;">
      • <strong>Core Purpose:</strong> Automated technical unit management dashboard for staff attendance, monthly KPI scores, and helpdesk SLA ticketing.<br>
      • <strong>Key Capabilities:</strong> Custom parsing pipeline converting unstructured Persian Word (.docx) reports and biometric time-clocks into structured, clean Excel sheets.<br>
      • <strong>Analytics &amp; BI:</strong> Algorithmic calculation of monthly departmental KPIs, MTTR resolution time tracking, and dynamic interactive charts.
    </p>
    <div class="d-flex flex-wrap gap-1 mt-2">
      <span class="badge badge-light border">Python</span>
      <span class="badge badge-light border">FastAPI</span>
      <span class="badge badge-light border">Pandas</span>
      <span class="badge badge-light border">openpyxl</span>
      <span class="badge badge-light border">python-docx</span>
      <span class="badge badge-light border">React</span>
      <span class="badge badge-light border">ECharts</span>
    </div>
  </div>

  <!-- Project 4 -->
  <div class="card mb-4 p-4 border shadow-sm hoverable">
    <div class="d-flex flex-wrap justify-content-between align-items-center mb-2">
      <h4 class="card-title font-weight-bold mb-1">
        <a href="/projects/4_project/" class="text-primary text-decoration-none">Automated Detection &amp; Classification of Planets</a>
      </h4>
      <span class="badge badge-info px-2 py-1">Applied AI & Vision</span>
    </div>
    <p class="card-text text-muted mb-2" style="line-height: 1.5;">
      • <strong>Core Purpose:</strong> Computer vision and machine learning pipeline for detecting and classifying planets in astronomical imagery (NASA &amp; ESA archives).<br>
      • <strong>Methodology:</strong> Gaussian/median filtering, CLAHE, background subtraction, Canny edge detection, and OpenCV contour segmentation.<br>
      • <strong>Feature Engineering &amp; ML:</strong> Extracted GLCM texture descriptors, color histograms, and morphological moments; evaluated SVM and KNN multi-class classifiers.
    </p>
    <div class="d-flex flex-wrap gap-1 mt-2">
      <span class="badge badge-light border">OpenCV</span>
      <span class="badge badge-light border">Python</span>
      <span class="badge badge-light border">scikit-learn</span>
      <span class="badge badge-light border">NumPy</span>
      <span class="badge badge-light border">Matplotlib</span>
    </div>
  </div>

  <!-- Project 5 -->
  <div class="card mb-4 p-4 border shadow-sm hoverable">
    <div class="d-flex flex-wrap justify-content-between align-items-center mb-2">
      <h4 class="card-title font-weight-bold mb-1">
        <a href="/projects/5_project/" class="text-primary text-decoration-none">Enterprise DevOps &amp; Cloud Infrastructure</a>
      </h4>
      <span class="badge badge-secondary px-2 py-1">DevOps & Infra</span>
    </div>
    <p class="card-text text-muted mb-2" style="line-height: 1.5;">
      • <strong>Core Purpose:</strong> High-availability virtualization, Docker containerization, and disaster recovery automation for a platform with 100,000+ registered users.<br>
      • <strong>Infrastructure:</strong> Multi-node VMware ESXi cluster administration (~10 production VMs), 5+ containerized production services, and zero-downtime FreePBX VoIP telephony.<br>
      • <strong>Storage &amp; Backup:</strong> Automated TrueNAS ZFS storage arrays (1–10 TB) with snapshot replication and Veeam backup automation (saving 3–4 hours/week).
    </p>
    <div class="d-flex flex-wrap gap-1 mt-2">
      <span class="badge badge-light border">VMware ESXi</span>
      <span class="badge badge-light border">Docker</span>
      <span class="badge badge-light border">Docker Compose</span>
      <span class="badge badge-light border">Bash</span>
      <span class="badge badge-light border">TrueNAS ZFS</span>
      <span class="badge badge-light border">Veeam</span>
      <span class="badge badge-light border">FreePBX</span>
    </div>
  </div>

</div>
