---
layout: page
title: Featured Projects
permalink: /projects/
description: Engineering platforms, cloud architectures, data automation pipelines, and AI research projects.
nav: true
nav_order: 2
---

<style>
:root {
  --proj-primary: #0284c7;
  --proj-primary-light: #e0f2fe;
  --proj-primary-border: #bae6fd;
  --proj-card-bg: #ffffff;
  --proj-border: #e2e8f0;
  --proj-text-main: #0f172a;
  --proj-text-muted: #475569;
  --proj-tag-bg: #f1f5f9;
  --proj-tag-text: #334155;
  --proj-mono: 'JetBrains Mono', monospace;
}

html[data-theme='dark'], body.dark-theme, [data-theme="dark"] {
  --proj-primary: #38bdf8;
  --proj-primary-light: #082f49;
  --proj-primary-border: #075985;
  --proj-card-bg: #131b2e;
  --proj-border: #1e293b;
  --proj-text-main: #f1f5f9;
  --proj-text-muted: #94a3b8;
  --proj-tag-bg: #1e293b;
  --proj-tag-text: #cbd5e1;
}

.projects-container {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  margin: 1.5rem 0 3rem;
}

.project-card-item {
  background: var(--proj-card-bg);
  border: 1px solid var(--proj-border);
  border-radius: 12px;
  padding: 1.5rem;
  transition: all 0.2s ease;
  box-shadow: 0 1px 3px 0 rgb(0 0 0 / 0.05);
}

.project-card-item:hover {
  border-color: var(--proj-primary-border);
  box-shadow: 0 8px 16px -4px rgb(0 0 0 / 0.08);
  transform: translateY(-2px);
}

.project-card-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-wrap: wrap;
  gap: 0.5rem 1rem;
  margin-bottom: 0.75rem;
}

.project-card-title {
  font-size: 1.2rem;
  font-weight: 700;
  color: var(--proj-text-main);
  margin: 0;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.project-card-title a {
  color: var(--proj-text-main);
  text-decoration: none;
  transition: color 0.15s ease;
}

.project-card-title a:hover {
  color: var(--proj-primary);
}

.project-badge {
  font-size: 0.78rem;
  font-weight: 600;
  padding: 0.25rem 0.65rem;
  border-radius: 20px;
  background: var(--proj-primary-light);
  color: var(--proj-primary);
  border: 1px solid var(--proj-primary-border);
  white-space: nowrap;
}

.project-card-body {
  font-size: 0.92rem;
  color: var(--proj-text-muted);
  line-height: 1.6;
  margin-bottom: 1rem;
}

.project-card-body ul {
  padding-left: 1.2rem;
  margin: 0.5rem 0 0;
}

.project-card-body li {
  margin-bottom: 0.35rem;
}

.project-card-body strong {
  color: var(--proj-text-main);
}

.project-tech-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.4rem;
}

.p-tag {
  font-family: var(--proj-mono);
  font-size: 0.76rem;
  font-weight: 500;
  padding: 0.2rem 0.55rem;
  background: var(--proj-tag-bg);
  color: var(--proj-tag-text);
  border-radius: 4px;
  border: 1px solid var(--proj-border);
}
</style>

<div class="projects-container">

  <!-- Project 1 -->
  <article class="project-card-item">
    <div class="project-card-header">
      <h3 class="project-card-title">
        <i class="fa-solid fa-layer-group" style="color: var(--proj-primary);"></i>
        <a href="https://github.com/USFAkbari/Work-State" target="_blank" rel="noopener">Work-State Enterprise Engine</a>
      </h3>
      <span class="project-badge">Full-Stack & Systems</span>
    </div>
    <div class="project-card-body">
      <ul>
        <li><strong>Core Purpose:</strong> Enterprise workflow, unit telemetry, and status orchestration engine built for high-reliability production environments.</li>
        <li><strong>Backend & Architecture:</strong> Modular async FastAPI backend, PostgreSQL with connection pooling & Alembic migrations, JWT session isolation, and bcrypt security.</li>
        <li><strong>Frontend & DevOps:</strong> React 18 SPA with real-time optimistic state mutations, containerized with multi-stage Docker builds and automated Pytest test suites.</li>
      </ul>
    </div>
    <div class="project-tech-tags">
      <span class="p-tag">FastAPI</span>
      <span class="p-tag">Python 3.11</span>
      <span class="p-tag">React 18</span>
      <span class="p-tag">PostgreSQL</span>
      <span class="p-tag">Docker</span>
      <span class="p-tag">Alembic</span>
      <span class="p-tag">Pytest</span>
    </div>
  </article>

  <!-- Project 2 -->
  <article class="project-card-item">
    <div class="project-card-header">
      <h3 class="project-card-title">
        <i class="fa-solid fa-satellite" style="color: var(--proj-primary);"></i>
        <a href="https://github.com/USFAkbari" target="_blank" rel="noopener">Automated Detection & Classification of Solar System Planets</a>
      </h3>
      <span class="project-badge">Applied AI & Computer Vision</span>
    </div>
    <div class="project-card-body">
      <ul>
        <li><strong>Core Purpose:</strong> Computer vision and machine learning pipeline for detecting and classifying solar system planets in NASA and ESA astronomical imagery.</li>
        <li><strong>Image Processing:</strong> Multi-stage filtering (Gaussian, median), contrast optimization (CLAHE), Canny edge detection, and OpenCV contour segmentation.</li>
        <li><strong>Feature Extraction & ML:</strong> Extracted shape moments, GLCM texture metrics, and color histograms; evaluated SVM and KNN multi-class classifiers for high-accuracy identification.</li>
      </ul>
    </div>
    <div class="project-tech-tags">
      <span class="p-tag">Python</span>
      <span class="p-tag">OpenCV</span>
      <span class="p-tag">scikit-learn</span>
      <span class="p-tag">NumPy</span>
      <span class="p-tag">Matplotlib</span>
      <span class="p-tag">Computer Vision</span>
    </div>
  </article>

  <!-- Project 3 -->
  <article class="project-card-item">
    <div class="project-card-header">
      <h3 class="project-card-title">
        <i class="fa-solid fa-fingerprint" style="color: var(--proj-primary);"></i>
        <a href="https://github.com/USFAkbari/Attendance_Ddashboard" target="_blank" rel="noopener">HR Biometric Attendance & Evaluation Pipeline</a>
      </h3>
      <span class="project-badge">Data Engineering & Automation</span>
    </div>
    <div class="project-card-body">
      <ul>
        <li><strong>Core Purpose:</strong> Production telemetry extraction system interfacing with ZKTeco hardware terminals via TCP/UDP socket protocols.</li>
        <li><strong>ETL & Data Processing:</strong> Pandas pipeline consolidating biometric attendance logs and Persian Word reports (.docx) into structured, audit-ready data.</li>
        <li><strong>KPI Analytics:</strong> Dynamic reporting engine tracking staff shift adherence, anomaly detection, and department SLA metrics.</li>
      </ul>
    </div>
    <div class="project-tech-tags">
      <span class="p-tag">Python</span>
      <span class="p-tag">FastAPI</span>
      <span class="p-tag">Pandas</span>
      <span class="p-tag">pyzk</span>
      <span class="p-tag">openpyxl</span>
      <span class="p-tag">React</span>
    </div>
  </article>

  <!-- Project 4 -->
  <article class="project-card-item">
    <div class="project-card-header">
      <h3 class="project-card-title">
        <i class="fa-solid fa-terminal" style="color: var(--proj-primary);"></i>
        <a href="https://github.com/USFAkbari/LVM_Disk_Extender" target="_blank" rel="noopener">LVM Disk Extender & Open-Source DevOps Utilities</a>
      </h3>
      <span class="project-badge">Cloud-Native & Linux Ops</span>
    </div>
    <div class="project-card-body">
      <ul>
        <li><strong>Core Purpose:</strong> Automated operational utility for dynamically inspecting, extending, and resizing Logical Volume Management (LVM) partitions in production Linux systems.</li>
        <li><strong>DevOps Toolkit:</strong> Part of an open-source suite including automated Mattermost Team Edition deployment, Docker environment bootstrap scripts, and proxy health checkers.</li>
      </ul>
    </div>
    <div class="project-tech-tags">
      <span class="p-tag">Bash</span>
      <span class="p-tag">Linux LVM</span>
      <span class="p-tag">Docker</span>
      <span class="p-tag">SysAdmin</span>
      <span class="p-tag">Shell Automation</span>
    </div>
  </article>

</div>
