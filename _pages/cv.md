---
layout: page
title: Curriculum Vitae
permalink: /cv/
description: Academic CV of Yousef Akbari &bull; Prospective M.Sc. Candidate in Computer Science & Software Engineering.
nav: true
nav_order: 1
---

<style>
:root {
    --cv-bg: #f8fafc;
    --cv-surface: #ffffff;
    --cv-text-main: #0f172a;
    --cv-text-muted: #475569;
    --cv-text-light: #64748b;
    --cv-primary: #0284c7;
    --cv-primary-dark: #0369a1;
    --cv-primary-light: #e0f2fe;
    --cv-primary-border: #bae6fd;
    --cv-border: #e2e8f0;
    --cv-border-hover: #cbd5e1;
    --cv-tag-bg: #f1f5f9;
    --cv-tag-text: #334155;
    --cv-accent: #0d9488;
    --cv-radius-sm: 6px;
    --cv-radius-md: 10px;
    --cv-radius-lg: 14px;
    --cv-shadow-sm: 0 1px 2px 0 rgb(0 0 0 / 0.05);
    --cv-shadow-md: 0 4px 6px -1px rgb(0 0 0 / 0.07), 0 2px 4px -2px rgb(0 0 0 / 0.05);
    --cv-font-mono: 'JetBrains Mono', monospace;
}

html[data-theme='dark'], body.dark-theme, [data-theme="dark"] {
    --cv-bg: #0b0f19;
    --cv-surface: #131b2e;
    --cv-text-main: #f1f5f9;
    --cv-text-muted: #94a3b8;
    --cv-text-light: #64748b;
    --cv-primary: #38bdf8;
    --cv-primary-dark: #0284c7;
    --cv-primary-light: #082f49;
    --cv-primary-border: #075985;
    --cv-border: #1e293b;
    --cv-border-hover: #334155;
    --cv-tag-bg: #1e293b;
    --cv-tag-text: #cbd5e1;
    --cv-accent: #2dd4bf;
    --cv-shadow-sm: 0 1px 2px 0 rgb(0 0 0 / 0.3);
    --cv-shadow-md: 0 4px 12px 0 rgb(0 0 0 / 0.4);
}

.cv-container {
    max-width: 860px;
    margin: 1rem auto 3rem;
    background: var(--cv-surface);
    border: 1px solid var(--cv-border);
    border-radius: var(--cv-radius-lg);
    box-shadow: var(--cv-shadow-md);
    padding: 2.5rem 2.25rem;
    line-height: 1.65;
    color: var(--cv-text-main);
}

/* Header */
.cv-header {
    border-bottom: 2px solid var(--cv-border);
    padding-bottom: 1.75rem;
    margin-bottom: 2.25rem;
}

.header-top {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    flex-wrap: wrap;
    gap: 1rem;
}

.name-title h1 {
    font-size: 2.1rem;
    font-weight: 700;
    letter-spacing: -0.025em;
    color: var(--cv-text-main);
    line-height: 1.2;
    margin-bottom: 0.35rem;
}

.target-role {
    font-size: 1.05rem;
    font-weight: 500;
    color: var(--cv-primary);
    margin-bottom: 0.5rem;
}

.contact-grid {
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem 1.5rem;
    margin-top: 1rem;
    font-size: 0.9rem;
    color: var(--cv-text-muted);
}

.contact-item {
    display: inline-flex;
    align-items: center;
    gap: 0.4rem;
    text-decoration: none;
    color: var(--cv-text-muted) !important;
    transition: color 0.15s ease;
}

.contact-item i {
    color: var(--cv-primary);
    font-size: 0.95rem;
}

.contact-item:hover {
    color: var(--cv-primary) !important;
}

.header-actions {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
}

.cv-btn {
    display: inline-flex;
    align-items: center;
    gap: 0.4rem;
    font-size: 0.85rem;
    font-weight: 600;
    padding: 0.5rem 0.9rem;
    border-radius: var(--cv-radius-sm);
    cursor: pointer;
    text-decoration: none !important;
    transition: all 0.15s ease;
    border: 1px solid var(--cv-border);
    background: var(--cv-surface);
    color: var(--cv-text-main) !important;
}

.cv-btn:hover {
    border-color: var(--cv-primary);
    color: var(--cv-primary) !important;
    background: var(--cv-primary-light);
}

.cv-btn-primary {
    background: var(--cv-primary);
    color: #ffffff !important;
    border-color: var(--cv-primary);
}

.cv-btn-primary:hover {
    background: var(--cv-primary-dark);
    color: #ffffff !important;
}

/* Sections */
.cv-section {
    margin-bottom: 2.5rem;
}

.cv-section:last-child {
    margin-bottom: 0;
}

.section-header {
    display: flex;
    align-items: center;
    gap: 0.65rem;
    margin-bottom: 1.25rem;
    padding-bottom: 0.45rem;
    border-bottom: 1px solid var(--cv-border);
}

.section-title {
    font-size: 1.1rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    color: var(--cv-text-main);
    margin: 0;
}

.section-icon {
    color: var(--cv-primary);
    font-size: 1.1rem;
}

/* Research Interests */
.interests-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 0.75rem;
}

.interest-card {
    background: var(--cv-tag-bg);
    border-left: 3px solid var(--cv-primary);
    padding: 0.85rem 1.15rem;
    border-radius: 0 var(--cv-radius-sm) var(--cv-radius-sm) 0;
    font-size: 0.93rem;
}

.interest-card strong {
    color: var(--cv-text-main);
    font-weight: 600;
}

.interest-card p {
    color: var(--cv-text-muted);
    margin-top: 0.2rem;
    margin-bottom: 0;
    font-size: 0.88rem;
}

/* Entries */
.entry {
    margin-bottom: 1.6rem;
}

.entry:last-child {
    margin-bottom: 0;
}

.entry-header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    flex-wrap: wrap;
    gap: 0.25rem 1rem;
    margin-bottom: 0.2rem;
}

.entry-title {
    font-size: 1.02rem;
    font-weight: 600;
    color: var(--cv-text-main);
}

.entry-date {
    font-size: 0.82rem;
    font-family: var(--cv-font-mono);
    font-weight: 500;
    color: var(--cv-text-light);
    white-space: nowrap;
}

.entry-subtitle {
    font-size: 0.9rem;
    font-weight: 500;
    color: var(--cv-primary);
    margin-bottom: 0.45rem;
}

.entry-subtitle span {
    color: var(--cv-text-muted);
    font-weight: 400;
}

.entry-description {
    font-size: 0.9rem;
    color: var(--cv-text-muted);
    margin-bottom: 0.5rem;
}

.entry-list {
    list-style: none;
    padding-left: 0;
    margin-bottom: 0.5rem;
    display: flex;
    flex-direction: column;
    gap: 0.4rem;
}

.entry-list li {
    position: relative;
    padding-left: 1.25rem;
    font-size: 0.9rem;
    color: var(--cv-text-muted);
}

.entry-list li::before {
    content: "•";
    position: absolute;
    left: 0.25rem;
    color: var(--cv-primary);
    font-weight: bold;
}

.entry-list li strong {
    color: var(--cv-text-main);
}

/* Tech Tags */
.tech-stack {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
    margin-top: 0.55rem;
}

.tag {
    font-family: var(--cv-font-mono);
    font-size: 0.76rem;
    font-weight: 500;
    padding: 0.18rem 0.55rem;
    background: var(--cv-tag-bg);
    color: var(--cv-tag-text);
    border-radius: 4px;
    border: 1px solid var(--cv-border);
}

.tag-accent {
    background: var(--cv-primary-light);
    color: var(--cv-primary-dark);
    border-color: var(--cv-primary-border);
}

/* Skills Matrix */
.skills-matrix {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 1.15rem;
}

.skill-group {
    background: var(--cv-tag-bg);
    border: 1px solid var(--cv-border);
    border-radius: var(--cv-radius-md);
    padding: 1.1rem;
}

.skill-group-title {
    font-size: 0.85rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.03em;
    color: var(--cv-text-main);
    margin-bottom: 0.6rem;
}

.skill-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.35rem;
}

/* Projects Grid */
.projects-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.15rem;
}

.project-card {
    border: 1px solid var(--cv-border);
    border-radius: var(--cv-radius-md);
    padding: 1.15rem;
    transition: border-color 0.2s ease, box-shadow 0.2s ease;
}

.project-card:hover {
    border-color: var(--cv-primary-border);
    box-shadow: var(--cv-shadow-sm);
}

.project-header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-bottom: 0.35rem;
}

.project-name {
    font-size: 0.98rem;
    font-weight: 600;
    color: var(--cv-text-main);
}

.project-link {
    display: inline-flex;
    align-items: center;
    gap: 0.25rem;
    font-size: 0.8rem;
    font-family: var(--cv-font-mono);
    color: var(--cv-primary) !important;
    text-decoration: none;
    font-weight: 500;
}

.project-link:hover {
    text-decoration: underline !important;
}

/* Two Column Grid */
.two-col-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1.5rem;
}

@media print {
    .cv-container {
        border: none;
        box-shadow: none;
        padding: 0;
        margin: 0;
        max-width: 100%;
    }
    .header-actions, nav, footer, .navbar {
        display: none !important;
    }
    .cv-section {
        page-break-inside: avoid;
    }
}

@media (max-width: 640px) {
    .cv-container {
        padding: 1.5rem 1.1rem;
    }
    .two-col-grid {
        grid-template-columns: 1fr;
    }
}
</style>

<div class="cv-container">
    <!-- Header -->
    <header class="cv-header">
        <div class="header-top">
            <div class="name-title">
                <h1>Yousef Akbari</h1>
                <div class="target-role">Prospective M.Sc. Candidate &bull; Computer Science / Software Engineering</div>
            </div>
            <div class="header-actions">
                <a class="cv-btn cv-btn-primary" href="{{ '/assets/pdf/Yousef_Akbari_Academic_CV.pdf' | relative_url }}" target="_blank">
                    <i class="fa-solid fa-file-pdf"></i> Download PDF
                </a>
                <button class="cv-btn" onclick="window.print()">
                    <i class="fa-solid fa-print"></i> Print
                </button>
            </div>
        </div>

        <div class="contact-grid">
            <div class="contact-item">
                <i class="fa-solid fa-location-dot"></i>
                <span>Mashhad, Iran</span>
            </div>
            <a class="contact-item" href="mailto:usfakbari@gmail.com">
                <i class="fa-solid fa-envelope"></i>
                <span>usfakbari@gmail.com</span>
            </a>
            <a class="contact-item" href="https://linkedin.com/in/yousefakbari" target="_blank" rel="noopener">
                <i class="fa-brands fa-linkedin"></i>
                <span>linkedin.com/in/yousefakbari</span>
            </a>
            <a class="contact-item" href="https://github.com/USFAkbari" target="_blank" rel="noopener">
                <i class="fa-brands fa-github"></i>
                <span>github.com/USFAkbari</span>
            </a>
        </div>
    </header>

    <!-- Research Interests -->
    <section class="cv-section">
        <div class="section-header">
            <span class="section-icon"><i class="fa-solid fa-compass"></i></span>
            <h2 class="section-title">Research Interests</h2>
        </div>
        <div class="interests-grid">
            <div class="interest-card">
                <strong>Applied AI & Computer Vision</strong>
                <p>Image processing, object detection, and pattern recognition across real-world and scientific datasets.</p>
            </div>
            <div class="interest-card">
                <strong>Machine Learning Operations (MLOps)</strong>
                <p>Bridging ML model development and production-grade deployment via automated pipelines, containerization, and CI/CD quality gates.</p>
            </div>
            <div class="interest-card">
                <strong>Software Reliability & Release Engineering</strong>
                <p>Empirical evaluation of deployment strategies (canary/blue-green), fault tolerance, and system observability under non-deterministic workloads.</p>
            </div>
            <div class="interest-card">
                <strong>Cloud-Native Systems & Intelligent Automation</strong>
                <p>Distributed containerized architectures and AI-driven decision-making in cluster orchestration.</p>
            </div>
        </div>
    </section>

    <!-- Education -->
    <section class="cv-section">
        <div class="section-header">
            <span class="section-icon"><i class="fa-solid fa-graduation-cap"></i></span>
            <h2 class="section-title">Education</h2>
        </div>
        <div class="entry">
            <div class="entry-header">
                <span class="entry-title">Bachelor of Engineering in Computer Engineering (Artificial Intelligence)</span>
                <span class="entry-date">Sep 2016 – Sep 2021</span>
            </div>
            <div class="entry-subtitle">Azad University, North Tehran Branch <span>&bull; Tehran, Iran</span></div>
            <div class="entry-description">
                <strong>Relevant Coursework:</strong> Artificial Intelligence, Computer Vision, Image Processing, Data Structures & Algorithms, Software Engineering, Database Systems, Computer Networks, Operating Systems, Discrete Mathematics, Probability & Statistics.
            </div>
        </div>
    </section>

    <!-- Technical Skills -->
    <section class="cv-section">
        <div class="section-header">
            <span class="section-icon"><i class="fa-solid fa-code"></i></span>
            <h2 class="section-title">Technical Skills</h2>
        </div>
        <div class="skills-matrix">
            <div class="skill-group">
                <div class="skill-group-title">Programming & Scripting</div>
                <div class="skill-tags">
                    <span class="tag tag-accent">Python</span>
                    <span class="tag tag-accent">Bash / Shell</span>
                    <span class="tag">JavaScript</span>
                    <span class="tag">TypeScript</span>
                    <span class="tag">HTML / CSS</span>
                    <span class="tag">SQL</span>
                </div>
            </div>
            <div class="skill-group">
                <div class="skill-group-title">DevOps & Cloud-Native</div>
                <div class="skill-tags">
                    <span class="tag tag-accent">Docker</span>
                    <span class="tag tag-accent">Docker Compose</span>
                    <span class="tag tag-accent">CI/CD (GitLab / GitHub)</span>
                    <span class="tag">Kubernetes (CKA prep)</span>
                    <span class="tag">Linux / Ubuntu Server</span>
                    <span class="tag">VMware ESXi</span>
                </div>
            </div>
            <div class="skill-group">
                <div class="skill-group-title">AI/ML & Data Engineering</div>
                <div class="skill-tags">
                    <span class="tag tag-accent">OpenCV</span>
                    <span class="tag tag-accent">NumPy & Pandas</span>
                    <span class="tag">scikit-learn</span>
                    <span class="tag">Image Preprocessing</span>
                    <span class="tag">pyzk (Biometrics)</span>
                </div>
            </div>
            <div class="skill-group">
                <div class="skill-group-title">Systems & Infrastructure</div>
                <div class="skill-tags">
                    <span class="tag">TrueNAS / ZFS</span>
                    <span class="tag">MikroTik RouterOS</span>
                    <span class="tag">VLAN & Firewall</span>
                    <span class="tag">FreePBX / VoIP</span>
                    <span class="tag">Veeam Backup</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Academic & Research Projects -->
    <section class="cv-section">
        <div class="section-header">
            <span class="section-icon"><i class="fa-solid fa-flask"></i></span>
            <h2 class="section-title">Academic & Research Projects</h2>
        </div>

        <div class="entry">
            <div class="entry-header">
                <span class="entry-title">Automated Detection and Classification of Solar System Planets</span>
                <span class="entry-date">2020 – 2021</span>
            </div>
            <div class="entry-subtitle">Bachelor's Capstone Project <span>&bull; Azad University, North Tehran Branch</span></div>
            <ul class="entry-list">
                <li>Designed a computer vision pipeline for detecting and classifying planets in astronomical imagery from NASA and ESA archives.</li>
                <li>Built a multi-stage preprocessing workflow including Gaussian/median filtering, CLAHE contrast enhancement, and background subtraction.</li>
                <li>Extracted shape descriptors (circularity, eccentricity), color histograms, and GLCM texture features; trained multi-class SVM and KNN classifiers for accurate celestial identification.</li>
            </ul>
            <div class="tech-stack">
                <span class="tag">Python</span>
                <span class="tag">OpenCV</span>
                <span class="tag">scikit-learn</span>
                <span class="tag">NumPy</span>
                <span class="tag">Matplotlib</span>
            </div>
        </div>

        <div class="entry">
            <div class="entry-header">
                <span class="entry-title">HR Biometric Attendance & Telemetry System</span>
                <span class="entry-date">2025 – Present</span>
            </div>
            <div class="entry-subtitle">Independent Engineering Project <span>&bull; Khademan Emam Zaman</span></div>
            <ul class="entry-list">
                <li>Developed Python services interfacing with ZKTeco biometric terminals via socket communication (pyzk) for real-time record synchronization across remote sites.</li>
                <li>Built automated Pandas data transformation pipelines to process logs and identify attendance anomalies.</li>
            </ul>
            <div class="tech-stack">
                <span class="tag">Python</span>
                <span class="tag">Pandas</span>
                <span class="tag">pyzk</span>
                <span class="tag">Networking (TCP/UDP)</span>
            </div>
        </div>
    </section>

    <!-- Professional Experience -->
    <section class="cv-section">
        <div class="section-header">
            <span class="section-icon"><i class="fa-solid fa-briefcase"></i></span>
            <h2 class="section-title">Professional Experience</h2>
        </div>

        <div class="entry">
            <div class="entry-header">
                <span class="entry-title">Systems & DevOps Engineer</span>
                <span class="entry-date">Jan 2025 – Present</span>
            </div>
            <div class="entry-subtitle">Khademan Emam Zaman <span>&bull; Mashhad, Iran</span></div>
            <ul class="entry-list">
                <li>Administered a multi-node VMware ESXi environment hosting ~10 production VMs for a nationally distributed platform serving <strong>100,000+ registered users</strong>.</li>
                <li>Containerized 15+ production services using Docker, reducing deployment cycle times by ~20% and eliminating configuration drift.</li>
                <li>Automated backup orchestration via Bash scripting and TrueNAS ZFS snapshots, recovering ~3–4 engineering hours/week.</li>
                <li>Maintained 100% uptime over 6+ months for a FreePBX VoIP communications infrastructure.</li>
            </ul>
        </div>

        <div class="entry">
            <div class="entry-header">
                <span class="entry-title">DevOps Engineer</span>
                <span class="entry-date">Apr 2024 – Jan 2025</span>
            </div>
            <div class="entry-subtitle">Part Software Group <span>&bull; Mashhad, Iran</span></div>
            <ul class="entry-list">
                <li>Managed infrastructure operations for <strong>200+ virtual machines</strong> across dev, staging, QA, and production environments.</li>
                <li>Standardized multi-environment Docker workflows, reducing deployment discrepancy across tiers.</li>
                <li>Automated Linux fleet maintenance, security patching, and coordinated weekly application releases with engineering teams.</li>
            </ul>
        </div>
    </section>

    <!-- Open Source & Selected Projects -->
    <section class="cv-section">
        <div class="section-header">
            <span class="section-icon"><i class="fa-solid fa-code-branch"></i></span>
            <h2 class="section-title">Open-Source & Technical Projects</h2>
        </div>
        <div class="projects-grid">
            <div class="project-card">
                <div class="project-header">
                    <span class="project-name">LVM Disk Extender & DevOps Utilities</span>
                    <a href="https://github.com/USFAkbari/LVM_Disk_Extender" target="_blank" rel="noopener" class="project-link">GitHub &rarr;</a>
                </div>
                <p class="entry-description">Automated Bash tool for dynamically detecting, extending, and resizing Logical Volume Management (LVM) partitions in production Linux systems.</p>
                <div class="tech-stack">
                    <span class="tag">Bash</span>
                    <span class="tag">Linux LVM</span>
                    <span class="tag">SysAdmin</span>
                </div>
            </div>

            <div class="project-card">
                <div class="project-header">
                    <span class="project-name">Audio Signal Processing & Feature Extraction</span>
                    <a href="https://github.com/USFAkbari/Audio_Signal_Processing" target="_blank" rel="noopener" class="project-link">GitHub &rarr;</a>
                </div>
                <p class="entry-description">Signal analysis pipelines for acoustic feature extraction, spectrogram calculation, and ML preprocessing.</p>
                <div class="tech-stack">
                    <span class="tag">Python</span>
                    <span class="tag">Signal Processing</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Two Columns: Certifications & Languages -->
    <div class="two-col-grid">
        <section class="cv-section">
            <div class="section-header">
                <span class="section-icon"><i class="fa-solid fa-award"></i></span>
                <h2 class="section-title">Certifications</h2>
            </div>
            <ul class="entry-list">
                <li><strong>Crash Course on Python</strong> &bull; Google / Coursera (Completed)</li>
                <li><strong>Using Python to Interact with the OS</strong> &bull; Google / Coursera</li>
                <li><strong>Kubernetes Administration (CKA Path)</strong> &bull; Self-study</li>
            </ul>
        </section>

        <section class="cv-section">
            <div class="section-header">
                <span class="section-icon"><i class="fa-solid fa-language"></i></span>
                <h2 class="section-title">Languages</h2>
            </div>
            <ul class="entry-list">
                <li><strong>Persian (Farsi):</strong> Native</li>
                <li><strong>English:</strong> Professional working proficiency (IELTS in prep)</li>
            </ul>
        </section>
    </div>
</div>
