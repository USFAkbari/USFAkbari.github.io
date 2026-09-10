---
layout: page
title: about
permalink: /
description: Academic portfolio & CV of Yousef Akbari • Prospective M.Sc. Candidate in Computer Science & Software Engineering.
---

<style>
.post-header {
  display: none !important;
}

.about-hero-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 2rem;
  padding: 1.5rem 0 2rem;
  border-bottom: 2px solid var(--border);
  margin-bottom: 2rem;
}

.about-hero-info {
  flex: 1;
}

.about-hero-name {
  font-size: 2.35rem;
  font-weight: 800;
  letter-spacing: -0.03em;
  color: var(--text-main);
  line-height: 1.15;
  margin: 0 0 0.35rem;
}

.about-hero-role {
  font-size: 1.05rem;
  font-weight: 600;
  color: var(--primary);
  margin-bottom: 0.75rem;
}

.about-hero-summary {
  font-size: 0.95rem;
  color: var(--text-muted);
  line-height: 1.6;
  margin-bottom: 1rem;
}

.about-contact-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 0.6rem 1.25rem;
  font-size: 0.88rem;
  color: var(--text-muted);
}

.about-contact-item {
  display: inline-flex;
  align-items: center;
  gap: 0.4rem;
  text-decoration: none !important;
  color: var(--text-muted) !important;
  transition: color 0.15s ease;
}

.about-contact-item a {
  color: inherit !important;
  text-decoration: none !important;
  font-weight: 500;
}

.about-contact-item i {
  color: var(--primary);
}

.about-contact-item:hover, .about-contact-item a:hover {
  color: var(--primary) !important;
}

.about-hero-photo-wrap {
  flex-shrink: 0;
  width: 170px;
  height: 170px;
  border-radius: var(--radius-lg);
  overflow: hidden;
  border: 2px solid var(--border);
  box-shadow: var(--shadow-md);
  background: var(--surface);
  transition: border-color 0.2s ease, transform 0.2s ease;
}

.about-hero-photo-wrap:hover {
  border-color: var(--primary-border);
  transform: translateY(-2px);
}

.about-hero-photo {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.hero-actions {
  display: flex;
  flex-wrap: nowrap;
  overflow-x: auto;
  gap: 0.5rem;
  margin: 1.25rem 0 2rem;
  padding-bottom: 4px;
  -webkit-overflow-scrolling: touch;
}

.hero-btn {
  display: inline-flex;
  align-items: center;
  gap: 0.45rem;
  font-size: 0.84rem;
  font-weight: 600;
  padding: 0.5rem 0.85rem;
  border-radius: var(--radius-sm);
  text-decoration: none !important;
  white-space: nowrap;
  flex-shrink: 0;
  transition: all 0.15s ease;
  border: 1px solid var(--border);
  background: var(--surface);
  color: var(--text-main) !important;
}

.hero-btn-primary {
  background: var(--primary);
  color: #ffffff !important;
  border-color: var(--primary);
}

.hero-btn-primary:hover {
  background: var(--primary-dark);
  box-shadow: 0 4px 10px rgba(2, 132, 199, 0.25);
  color: #ffffff !important;
}

.hero-btn-outline:hover {
  border-color: var(--primary);
  color: var(--primary) !important;
  background: var(--primary-light);
}

/* Research Interests in a single horizontal row */
.research-single-line {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 0.75rem;
  margin: 1.25rem 0 2.25rem;
}

.research-card-compact {
  background: var(--surface);
  border: 1px solid var(--border);
  border-top: 3px solid var(--primary);
  border-radius: var(--radius-sm);
  padding: 0.85rem 0.9rem;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  transition: all 0.15s ease;
  box-shadow: var(--shadow-sm);
}

.research-card-compact:hover {
  transform: translateY(-2px);
  border-color: var(--primary-border);
  box-shadow: var(--shadow-md);
}

.research-card-compact h5 {
  font-size: 0.86rem;
  font-weight: 700;
  color: var(--text-main);
  margin: 0 0 0.3rem;
  display: flex;
  align-items: center;
  gap: 0.4rem;
  line-height: 1.3;
}

.research-card-compact p {
  font-size: 0.78rem;
  color: var(--text-muted);
  line-height: 1.45;
  margin: 0;
}

.section-head {
  display: flex;
  align-items: center;
  gap: 0.6rem;
  margin: 1.75rem 0 0.75rem;
  padding-bottom: 0.45rem;
  border-bottom: 1px solid var(--border);
}

.section-head h3 {
  font-size: 1.2rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  color: var(--text-main);
  margin: 0;
}

.section-head i {
  color: var(--primary);
  font-size: 1.15rem;
}

.bg-feature-box {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: var(--radius-md);
  padding: 1.35rem 1.5rem;
  margin: 1rem 0 2rem;
  box-shadow: var(--shadow-sm);
}

.bg-feature-box ul {
  padding-left: 1.2rem;
  margin-bottom: 0;
}

.bg-feature-box li {
  margin-bottom: 0.65rem;
  font-size: 0.92rem;
  color: var(--text-muted);
  line-height: 1.6;
}

.bg-feature-box li:last-child {
  margin-bottom: 0;
}

.bg-feature-box strong {
  color: var(--text-main);
}

@media (max-width: 900px) {
  .research-single-line {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 650px) {
  .about-hero-container {
    flex-direction: column-reverse;
    align-items: flex-start;
    gap: 1.25rem;
  }
  .about-hero-photo-wrap {
    width: 120px;
    height: 120px;
  }
  .about-hero-name {
    font-size: 1.85rem;
  }
  .research-single-line {
    grid-template-columns: 1fr;
  }
}
</style>

<!-- Hero Section with Photo right in front of name -->
<div class="about-hero-container">
  <div class="about-hero-info">
    <h1 class="about-hero-name">Yousef Akbari</h1>
    <div class="about-hero-role">Prospective M.Sc. Candidate &bull; Computer Science / Software Engineering</div>
    <div class="about-hero-summary">
      Computer Engineering graduate (Artificial Intelligence major) and active Systems &amp; DevOps Engineer with 2+ years hands-on experience in container orchestration (Docker), enterprise virtualization (VMware ESXi), storage resilience (TrueNAS ZFS), and automated operational pipelines. Preparing for M.Sc. graduate research positions (Fall 2027).
    </div>
    <div class="about-contact-grid">
      <span class="about-contact-item"><i class="fa-solid fa-location-dot"></i> Mashhad, Iran</span>
      <span class="about-contact-item"><a href="mailto:usfakbari@gmail.com"><i class="fa-solid fa-envelope"></i> usfakbari@gmail.com</a></span>
      <span class="about-contact-item"><a href="https://github.com/USFAkbari" target="_blank" rel="noopener"><i class="fa-brands fa-github"></i> GitHub</a></span>
      <span class="about-contact-item"><a href="https://linkedin.com/in/yousefakbari" target="_blank" rel="noopener"><i class="fa-brands fa-linkedin"></i> LinkedIn</a></span>
    </div>
  </div>
  <div class="about-hero-photo-wrap">
    <img src="/assets/img/prof_pic.jpg" alt="Yousef Akbari" class="about-hero-photo">
  </div>
</div>

<!-- Quick Navigation Action Buttons -->
<div class="hero-actions">
  <a href="/cv/" class="hero-btn hero-btn-primary"><i class="fa-solid fa-address-card"></i> View Full Academic CV</a>
  <a href="/transcripts/" class="hero-btn hero-btn-outline"><i class="fa-solid fa-graduation-cap"></i> View Transcripts &amp; GPA</a>
  <a href="/assets/pdf/Yousef_Akbari_Academic_CV.pdf" target="_blank" class="hero-btn hero-btn-outline"><i class="fa-solid fa-file-pdf"></i> Download PDF</a>
  <a href="/projects/" class="hero-btn hero-btn-outline"><i class="fa-solid fa-diagram-project"></i> Featured Projects</a>
  <a href="mailto:usfakbari@gmail.com" class="hero-btn hero-btn-outline"><i class="fa-solid fa-paper-plane"></i> Contact Directly</a>
</div>

<!-- Research Interests (Single Line 4-Column Grid) -->
<div class="section-head">
  <i class="fa-solid fa-compass"></i>
  <h3>Research Interests</h3>
</div>

<div class="research-single-line">
  <div class="research-card-compact">
    <h5><i class="fa-solid fa-eye" style="color: var(--primary);"></i> Applied AI &amp; CV</h5>
    <p>Image processing, feature extraction, and pattern recognition on scientific datasets.</p>
  </div>
  <div class="research-card-compact">
    <h5><i class="fa-solid fa-microchip" style="color: var(--primary);"></i> MLOps</h5>
    <p>Bridging ML to production with container pipelines and automated quality gates.</p>
  </div>
  <div class="research-card-compact">
    <h5><i class="fa-solid fa-shield-halved" style="color: var(--primary);"></i> Reliability</h5>
    <p>Empirical evaluation of canary/blue-green deployments and system resilience.</p>
  </div>
  <div class="research-card-compact">
    <h5><i class="fa-solid fa-server" style="color: var(--primary);"></i> Cloud-Native</h5>
    <p>Distributed container architectures, cluster automation, and storage resilience.</p>
  </div>
</div>

<!-- Academic & Technical Highlights -->
<div class="section-head">
  <i class="fa-solid fa-graduation-cap"></i>
  <h3>Academic &amp; Technical Highlights</h3>
</div>

<div class="bg-feature-box">
  <ul>
    <li>
      <strong>Education:</strong> Bachelor of Engineering in Computer Engineering (Artificial Intelligence), <em>Azad University, North Tehran Branch</em> (2016–2021).
    </li>
    <li>
      <strong>Core Academic Coursework:</strong> Artificial Intelligence, Computer Vision, Image Processing, Data Structures &amp; Algorithms, Software Engineering, Database Systems, Computer Networks, Operating Systems, Discrete Mathematics, Probability &amp; Statistics.
    </li>
    <li>
      <strong>Systems Engineering in Production:</strong>
      <ul>
        <li><em>Khademan Emam Zaman (shamim313.com):</em> Administered multi-node VMware ESXi hosting ~10 production VMs serving <strong>100,000+ registered users</strong>, automated TrueNAS ZFS snapshots, and containerized 15+ production services.</li>
        <li><em>Part Software Group:</em> Managed infrastructure operations for <strong>200+ virtual machines</strong> across 4 lifecycle environments.</li>
      </ul>
    </li>
    <li>
      <strong>Language Proficiency:</strong> Persian (Native), English (Professional working proficiency, IELTS in active preparation).
    </li>
  </ul>
</div>
