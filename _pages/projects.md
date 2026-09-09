---
layout: page
title: Featured Projects
permalink: /projects/
description: Engineering platforms, cloud architectures, data automation pipelines, and AI research projects.
nav: true
nav_order: 2
---

<style>
.projects-container {
  display: flex;
  flex-direction: column;
  gap: 1.25rem;
  margin: 1.5rem 0 3rem;
}

.project-card-item {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: var(--radius-md);
  padding: 1.35rem 1.5rem;
  transition: all 0.2s ease;
  box-shadow: var(--shadow-sm);
}

.project-card-item:hover {
  border-color: var(--primary-border);
  box-shadow: var(--shadow-md);
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
  font-size: 1.15rem;
  font-weight: 700;
  color: var(--text-main);
  margin: 0;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.project-card-title a {
  color: var(--text-main);
  text-decoration: none;
  transition: color 0.15s ease;
}

.project-card-title a:hover {
  color: var(--primary);
}

.project-badge {
  font-size: 0.78rem;
  font-weight: 600;
  padding: 0.22rem 0.65rem;
  border-radius: 20px;
  background: var(--primary-light);
  color: var(--primary-dark);
  border: 1px solid var(--primary-border);
  white-space: nowrap;
}

html[data-theme='dark'] .project-badge {
  color: var(--primary);
}

.project-card-body {
  font-size: 0.92rem;
  color: var(--text-muted);
  line-height: 1.6;
  margin-bottom: 0.85rem;
}

.project-card-body ul {
  padding-left: 1.2rem;
  margin: 0.5rem 0 0;
}

.project-card-body li {
  margin-bottom: 0.35rem;
}

.project-card-body strong {
  color: var(--text-main);
}

.project-tech-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.4rem;
}

.p-tag {
  font-family: var(--font-mono);
  font-size: 0.76rem;
  font-weight: 500;
  padding: 0.2rem 0.55rem;
  background: var(--tag-bg);
  color: var(--tag-text);
  border-radius: var(--radius-sm);
  border: 1px solid var(--border);
}

.p-tag-accent {
  background: var(--primary-light);
  color: var(--primary-dark);
  border-color: var(--primary-border);
}

html[data-theme='dark'] .p-tag-accent {
  color: var(--primary);
}
</style>

<div class="projects-container">

  <!-- Project 1: Work-State -->
  <article class="project-card-item">
    <div class="project-card-header">
      <h3 class="project-card-title">
        <i class="fa-solid fa-layer-group" style="color: var(--primary);"></i>
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
      <span class="p-tag p-tag-accent">FastAPI</span>
      <span class="p-tag p-tag-accent">Python 3.11</span>
      <span class="p-tag">React 18</span>
      <span class="p-tag">PostgreSQL</span>
      <span class="p-tag">Docker</span>
      <span class="p-tag">Alembic</span>
      <span class="p-tag">Pytest</span>
    </div>
  </article>

  <!-- Project 2: Planets Detection -->
  <article class="project-card-item">
    <div class="project-card-header">
      <h3 class="project-card-title">
        <i class="fa-solid fa-satellite" style="color: var(--primary);"></i>
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
      <span class="p-tag p-tag-accent">Python</span>
      <span class="p-tag p-tag-accent">OpenCV</span>
      <span class="p-tag">scikit-learn</span>
      <span class="p-tag">NumPy</span>
      <span class="p-tag">Matplotlib</span>
      <span class="p-tag">Computer Vision</span>
    </div>
  </article>

  <!-- Project 3: Attendance Dashboard -->
  <article class="project-card-item">
    <div class="project-card-header">
      <h3 class="project-card-title">
        <i class="fa-solid fa-fingerprint" style="color: var(--primary);"></i>
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
      <span class="p-tag p-tag-accent">Python</span>
      <span class="p-tag">FastAPI</span>
      <span class="p-tag">Pandas</span>
      <span class="p-tag">pyzk</span>
      <span class="p-tag">openpyxl</span>
      <span class="p-tag">React</span>
    </div>
  </article>

  <!-- Project 4: Enterprise DevOps & Cloud Infrastructure -->
  <article class="project-card-item">
    <div class="project-card-header">
      <h3 class="project-card-title">
        <i class="fa-solid fa-server" style="color: var(--primary);"></i>
        <a href="https://github.com/USFAkbari" target="_blank" rel="noopener">Enterprise DevOps & Cloud Infrastructure Operations</a>
      </h3>
      <span class="project-badge">Cloud-Native & Systems</span>
    </div>
    <div class="project-card-body">
      <ul>
        <li><strong>High-Availability Cluster Operations:</strong> Maintained multi-node VMware ESXi production environments hosting ~10 production VMs serving over <strong>100,000 registered users</strong> with zero unplanned downtime.</li>
        <li><strong>Containerization & Automation:</strong> Containerized 15+ production services using Docker Compose, automated backup pipelines via Bash and TrueNAS ZFS snapshots.</li>
        <li><strong>Telephony & Storage:</strong> Zero-downtime FreePBX VoIP communications and TrueNAS ZFS storage arrays (1–10 TB) with automated snapshot replication.</li>
      </ul>
    </div>
    <div class="project-tech-tags">
      <span class="p-tag p-tag-accent">VMware ESXi</span>
      <span class="p-tag p-tag-accent">Docker</span>
      <span class="p-tag">TrueNAS ZFS</span>
      <span class="p-tag">FreePBX</span>
      <span class="p-tag">Bash</span>
      <span class="p-tag">Ubuntu Server</span>
    </div>
  </article>

  <!-- Project 5: LVM Disk Extender & DevOps Utilities -->
  <article class="project-card-item">
    <div class="project-card-header">
      <h3 class="project-card-title">
        <i class="fa-solid fa-terminal" style="color: var(--primary);"></i>
        <a href="https://github.com/USFAkbari/LVM_Disk_Extender" target="_blank" rel="noopener">LVM Disk Extender & Open-Source DevOps Utilities</a>
      </h3>
      <span class="project-badge">Linux Operations</span>
    </div>
    <div class="project-card-body">
      <ul>
        <li><strong>Core Purpose:</strong> Automated operational utility for dynamically inspecting, extending, and resizing Logical Volume Management (LVM) partitions in production Linux systems.</li>
        <li><strong>DevOps Toolkit:</strong> Part of an open-source suite including automated Mattermost Team Edition deployment, Docker environment bootstrap scripts, and proxy health checkers.</li>
      </ul>
    </div>
    <div class="project-tech-tags">
      <span class="p-tag p-tag-accent">Bash</span>
      <span class="p-tag">Linux LVM</span>
      <span class="p-tag">Docker</span>
      <span class="p-tag">SysAdmin</span>
      <span class="p-tag">Shell Automation</span>
    </div>
  </article>

</div>
