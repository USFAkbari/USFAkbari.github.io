---
layout: page
permalink: /repositories/
title: repositories
description: Open-source DevOps automation tools, cloud scripts, system utilities, and machine learning models.
nav: true
nav_order: 3
---

<style>
.repositories-container {
  display: flex;
  flex-direction: column;
  gap: 1.15rem;
  margin: 1.5rem 0 3rem;
}

.repo-card-item {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: var(--radius-md);
  padding: 1.25rem 1.4rem;
  transition: all 0.2s ease;
  box-shadow: var(--shadow-sm);
}

.repo-card-item:hover {
  border-color: var(--primary-border);
  box-shadow: var(--shadow-md);
  transform: translateY(-2px);
}

.repo-card-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 0.5rem 1rem;
  margin-bottom: 0.65rem;
}

.repo-card-title {
  font-size: 1.1rem;
  font-weight: 700;
  margin: 0;
  display: flex;
  align-items: center;
  gap: 0.45rem;
}

.repo-card-title a {
  color: var(--primary);
  text-decoration: none;
  transition: color 0.15s ease;
}

.repo-card-title a:hover {
  color: var(--primary-dark);
}

.repo-badge {
  font-size: 0.78rem;
  font-weight: 600;
  padding: 0.2rem 0.6rem;
  border-radius: 20px;
  background: var(--primary-light);
  color: var(--primary-dark);
  border: 1px solid var(--primary-border);
  white-space: nowrap;
}

html[data-theme='dark'] .repo-badge {
  color: var(--primary);
}

.star-badge {
  font-size: 0.75rem;
  font-family: var(--font-mono);
  font-weight: 600;
  padding: 0.18rem 0.55rem;
  border-radius: var(--radius-sm);
  background: #fef3c7;
  color: #92400e;
  border: 1px solid #fde68a;
}

html[data-theme='dark'] .star-badge {
  background: #451a03;
  color: #fde68a;
  border: 1px solid #78350f;
}

.repo-card-body {
  font-size: 0.91rem;
  color: var(--text-muted);
  line-height: 1.55;
  margin-bottom: 0.75rem;
}

.repo-card-body p {
  margin: 0;
}

.repo-tech-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.35rem;
}
</style>

<div class="repositories-container">

  <!-- DnsMnager -->
  <article class="repo-card-item">
    <div class="repo-card-header">
      <h3 class="repo-card-title">
        <a href="https://github.com/USFAkbari/DnsMnager" target="_blank" rel="noopener">
          <i class="fa-brands fa-github"></i> DnsMnager
        </a>
      </h3>
      <div class="d-flex align-items-center gap-1">
        <span class="star-badge">⭐ 1 Star</span>
        <span class="repo-badge">DevOps &amp; Networking</span>
      </div>
    </div>
    <div class="repo-card-body">
      <p>
        • <strong>Core Purpose:</strong> Automated DNS record management and upstream nameserver switching utility for Linux servers.<br>
        • <strong>Key Capabilities:</strong> Rapid CLI-based host resolution updates, upstream DNS health verification, and zero-downtime cache flushing.<br>
        • <strong>Tech &amp; Stack:</strong> Shell, Bash, Systemd-resolved, Linux Network Stack.
      </p>
    </div>
    <div class="repo-tech-tags">
      <span class="tag tag-accent">Bash</span>
      <span class="tag">Linux</span>
      <span class="tag">DNS</span>
      <span class="tag">Systemd</span>
    </div>
  </article>

  <!-- LVM_Disk_Extender -->
  <article class="repo-card-item">
    <div class="repo-card-header">
      <h3 class="repo-card-title">
        <a href="https://github.com/USFAkbari/LVM_Disk_Extender" target="_blank" rel="noopener">
          <i class="fa-brands fa-github"></i> LVM_Disk_Extender
        </a>
      </h3>
      <div class="d-flex align-items-center gap-1">
        <span class="star-badge">⭐ 1 Star</span>
        <span class="repo-badge">Storage &amp; Systems</span>
      </div>
    </div>
    <div class="repo-card-body">
      <p>
        • <strong>Core Purpose:</strong> Automated zero-downtime Linux LVM logical volume resize and partition expansion tool.<br>
        • <strong>Key Capabilities:</strong> Scans unallocated block devices, auto-resizes physical/volume groups, and grows ext4/xfs filesystems online.<br>
        • <strong>Tech &amp; Stack:</strong> Bash, LVM2, parted, resize2fs, xfs_growfs.
      </p>
    </div>
    <div class="repo-tech-tags">
      <span class="tag tag-accent">Bash</span>
      <span class="tag">LVM2</span>
      <span class="tag">Storage Automation</span>
      <span class="tag">Linux</span>
    </div>
  </article>

  <!-- docker_Initiation -->
  <article class="repo-card-item">
    <div class="repo-card-header">
      <h3 class="repo-card-title">
        <a href="https://github.com/USFAkbari/docker_Initiation" target="_blank" rel="noopener">
          <i class="fa-brands fa-github"></i> docker_Initiation
        </a>
      </h3>
      <div class="d-flex align-items-center gap-1">
        <span class="star-badge">⭐ 1 Star</span>
        <span class="repo-badge">DevOps &amp; Cloud</span>
      </div>
    </div>
    <div class="repo-card-body">
      <p>
        • <strong>Core Purpose:</strong> Production-ready Docker Engine &amp; Docker Compose provisioning and security hardening script.<br>
        • <strong>Key Capabilities:</strong> Automated daemon.json registry mirror configuration, log rotation caps, non-root user groups, and systemd tuning.<br>
        • <strong>Tech &amp; Stack:</strong> Shell, Docker CE, Docker Compose, Linux Security.
      </p>
    </div>
    <div class="repo-tech-tags">
      <span class="tag tag-accent">Docker</span>
      <span class="tag">Docker Compose</span>
      <span class="tag">Shell</span>
      <span class="tag">Provisioning</span>
    </div>
  </article>

  <!-- proxy-health-checker -->
  <article class="repo-card-item">
    <div class="repo-card-header">
      <h3 class="repo-card-title">
        <a href="https://github.com/USFAkbari/proxy-health-checker" target="_blank" rel="noopener">
          <i class="fa-brands fa-github"></i> proxy-health-checker
        </a>
      </h3>
      <div class="d-flex align-items-center gap-1">
        <span class="star-badge">⭐ 1 Star</span>
        <span class="repo-badge">Observability &amp; Reliability</span>
      </div>
    </div>
    <div class="repo-card-body">
      <p>
        • <strong>Core Purpose:</strong> High-frequency health probe &amp; latency benchmark utility for reverse proxies, CDN edge nodes, and load balancers.<br>
        • <strong>Key Capabilities:</strong> Multi-target status code assertions, SSL expiry checks, response time histograms, and automatic failover hooks.<br>
        • <strong>Tech &amp; Stack:</strong> Bash, cURL, jq, Nginx monitoring, Cron automation.
      </p>
    </div>
    <div class="repo-tech-tags">
      <span class="tag tag-accent">Bash</span>
      <span class="tag">cURL</span>
      <span class="tag">Observability</span>
      <span class="tag">Nginx</span>
    </div>
  </article>

  <!-- Push_Notification -->
  <article class="repo-card-item">
    <div class="repo-card-header">
      <h3 class="repo-card-title">
        <a href="https://github.com/USFAkbari/Push_Notification" target="_blank" rel="noopener">
          <i class="fa-brands fa-github"></i> Push_Notification
        </a>
      </h3>
      <div class="d-flex align-items-center gap-1">
        <span class="star-badge">⭐ 1 Star</span>
        <span class="repo-badge">Backend &amp; Messaging</span>
      </div>
    </div>
    <div class="repo-card-body">
      <p>
        • <strong>Core Purpose:</strong> Multi-channel push notification backend and client subscription lifecycle service.<br>
        • <strong>Key Capabilities:</strong> Web Push protocol implementation with VAPID authentication, payload encryption, and subscriber queue dispatching.<br>
        • <strong>Tech &amp; Stack:</strong> Python, WebPush, Service Workers, RESTful API.
      </p>
    </div>
    <div class="repo-tech-tags">
      <span class="tag tag-accent">Python</span>
      <span class="tag">WebPush</span>
      <span class="tag">Service Workers</span>
      <span class="tag">REST API</span>
    </div>
  </article>

  <!-- Excel_Service -->
  <article class="repo-card-item">
    <div class="repo-card-header">
      <h3 class="repo-card-title">
        <a href="https://github.com/USFAkbari/Excel_Service" target="_blank" rel="noopener">
          <i class="fa-brands fa-github"></i> Excel_Service
        </a>
      </h3>
      <div class="d-flex align-items-center gap-1">
        <span class="star-badge">⭐ 1 Star</span>
        <span class="repo-badge">Data Automation</span>
      </div>
    </div>
    <div class="repo-card-body">
      <p>
        • <strong>Core Purpose:</strong> Automated spreadsheet ingestion, reconciliation, and structured report generation microservice.<br>
        • <strong>Key Capabilities:</strong> Persian/RTL layout formatting, automated column matching across heterogeneous exports, and formula preservation.<br>
        • <strong>Tech &amp; Stack:</strong> Python, openpyxl, Pandas, FastAPI.
      </p>
    </div>
    <div class="repo-tech-tags">
      <span class="tag tag-accent">Python</span>
      <span class="tag">Pandas</span>
      <span class="tag">openpyxl</span>
      <span class="tag">ETL</span>
    </div>
  </article>

  <!-- Bia_Pain_Bache -->
  <article class="repo-card-item">
    <div class="repo-card-header">
      <h3 class="repo-card-title">
        <a href="https://github.com/USFAkbari/Bia_Pain_Bache" target="_blank" rel="noopener">
          <i class="fa-brands fa-github"></i> Bia_Pain_Bache
        </a>
      </h3>
      <span class="repo-badge">Networking &amp; Core</span>
    </div>
    <div class="repo-card-body">
      <p>
        • <strong>Core Purpose:</strong> Cross-platform network proxy management GUI panel and subscription aggregator.<br>
        • <strong>Key Capabilities:</strong> TCP fragmentation tuning, Cloudflare WARP configuration, and unified routing rules for sing-box &amp; Xray clients.<br>
        • <strong>Tech &amp; Stack:</strong> Go, Node.js, singbox-core, xray-core, Web GUI.
      </p>
    </div>
    <div class="repo-tech-tags">
      <span class="tag tag-accent">Go</span>
      <span class="tag">Node.js</span>
      <span class="tag">sing-box</span>
      <span class="tag">xray-core</span>
    </div>
  </article>

  <!-- Audio_Signal_Processing -->
  <article class="repo-card-item">
    <div class="repo-card-header">
      <h3 class="repo-card-title">
        <a href="https://github.com/USFAkbari/Audio_Signal_Processing" target="_blank" rel="noopener">
          <i class="fa-brands fa-github"></i> Audio_Signal_Processing
        </a>
      </h3>
      <div class="d-flex align-items-center gap-1">
        <span class="star-badge">⭐ 1 Star</span>
        <span class="repo-badge">AI &amp; Signal Processing</span>
      </div>
    </div>
    <div class="repo-card-body">
      <p>
        • <strong>Core Purpose:</strong> Audio digital signal processing (DSP) and feature extraction toolkit for machine learning models.<br>
        • <strong>Key Capabilities:</strong> Computes Mel-spectrograms, MFCC coefficients, chroma features, spectral roll-off, and zero-crossing rates.<br>
        • <strong>Tech &amp; Stack:</strong> Python, Librosa, NumPy, SciPy, Matplotlib.
      </p>
    </div>
    <div class="repo-tech-tags">
      <span class="tag tag-accent">Python</span>
      <span class="tag">Librosa</span>
      <span class="tag">DSP</span>
      <span class="tag">NumPy</span>
    </div>
  </article>

  <!-- house-price-prediction-linear-regression -->
  <article class="repo-card-item">
    <div class="repo-card-header">
      <h3 class="repo-card-title">
        <a href="https://github.com/USFAkbari/house-price-prediction-linear-regression" target="_blank" rel="noopener">
          <i class="fa-brands fa-github"></i> House Price Prediction (Linear Regression)
        </a>
      </h3>
      <div class="d-flex align-items-center gap-1">
        <span class="star-badge">⭐ 1 Star</span>
        <span class="repo-badge">Applied AI</span>
      </div>
    </div>
    <div class="repo-card-body">
      <p>
        • <strong>Core Purpose:</strong> Multivariate linear regression pipeline with exploratory data analysis and statistical validation.<br>
        • <strong>Key Capabilities:</strong> Outlier detection, multicollinearity mitigation (VIF), gradient descent optimization, and regression diagnostics.<br>
        • <strong>Tech &amp; Stack:</strong> Python, scikit-learn, Pandas, Seaborn, Matplotlib.
      </p>
    </div>
    <div class="repo-tech-tags">
      <span class="tag tag-accent">Python</span>
      <span class="tag">scikit-learn</span>
      <span class="tag">Pandas</span>
      <span class="tag">EDA</span>
    </div>
  </article>

  <!-- ToValet -->
  <article class="repo-card-item">
    <div class="repo-card-header">
      <h3 class="repo-card-title">
        <a href="https://github.com/USFAkbari/ToValet" target="_blank" rel="noopener">
          <i class="fa-brands fa-github"></i> ToValet
        </a>
      </h3>
      <div class="d-flex align-items-center gap-1">
        <span class="star-badge">⭐ 1 Star</span>
        <span class="repo-badge">DevOps &amp; Tooling</span>
      </div>
    </div>
    <div class="repo-card-body">
      <p>
        • <strong>Core Purpose:</strong> Zero-configuration local web development server environment for Linux inspired by Laravel Valet.<br>
        • <strong>Key Capabilities:</strong> Automatic site discovery, wildcard local DNS routing (.test domains), on-the-fly Nginx vhost generation, and local SSL certificates.<br>
        • <strong>Tech &amp; Stack:</strong> Shell, Nginx, Dnsmasq, OpenSSL.
      </p>
    </div>
    <div class="repo-tech-tags">
      <span class="tag tag-accent">Shell</span>
      <span class="tag">Nginx</span>
      <span class="tag">Dnsmasq</span>
      <span class="tag">Local Dev</span>
    </div>
  </article>

</div>
