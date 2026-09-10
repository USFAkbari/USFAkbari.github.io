---
layout: page
title: Transcripts
permalink: /transcripts/
description: Academic transcripts, GPA conversions (WES, OMSAS, UBC/SFU), and coursework breakdown of Yousef Akbari (B.Sc. Computer Engineering - AI).
nav: true
nav_order: 4
---

<style>
.transcript-container {
    max-width: 900px;
    margin: 1rem auto 3rem;
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: var(--radius-lg);
    box-shadow: var(--shadow-md);
    padding: 2.25rem;
    line-height: 1.6;
    color: var(--text-main);
}

/* Header */
.transcript-header {
    border-bottom: 2px solid var(--border);
    padding-bottom: 1.5rem;
    margin-bottom: 2rem;
}

.header-top {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    flex-wrap: wrap;
    gap: 1rem;
}

.name-title h1 {
    font-size: 2rem;
    font-weight: 700;
    letter-spacing: -0.025em;
    color: var(--text-main);
    line-height: 1.2;
    margin-bottom: 0.35rem;
}

.target-role {
    font-size: 1.02rem;
    font-weight: 500;
    color: var(--primary);
    margin-bottom: 0.35rem;
}

.academic-subtext {
    font-size: 0.88rem;
    color: var(--text-muted);
}

.header-actions {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
}

.btn-action {
    display: inline-flex;
    align-items: center;
    gap: 0.4rem;
    font-size: 0.84rem;
    font-weight: 600;
    padding: 0.45rem 0.85rem;
    border-radius: var(--radius-sm);
    cursor: pointer;
    text-decoration: none !important;
    transition: all 0.15s ease;
    border: 1px solid var(--border);
    background: var(--surface);
    color: var(--text-main) !important;
}

.btn-action:hover {
    border-color: var(--primary);
    color: var(--primary) !important;
    background: var(--primary-light);
}

.btn-action-primary {
    background: var(--primary);
    color: #ffffff !important;
    border-color: var(--primary);
}

.btn-action-primary:hover {
    background: var(--primary-dark);
    color: #ffffff !important;
}

/* KPI Summary Cards */
.kpi-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1rem;
    margin-bottom: 2rem;
}

.kpi-card {
    background: var(--tag-bg);
    border: 1px solid var(--border);
    border-radius: var(--radius-md);
    padding: 1.1rem;
    position: relative;
    overflow: hidden;
    transition: transform 0.15s ease, border-color 0.15s ease;
}

.kpi-card:hover {
    transform: translateY(-2px);
    border-color: var(--primary-border);
}

.kpi-card.highlight {
    background: var(--primary-light);
    border-color: var(--primary-border);
}

.kpi-label {
    font-size: 0.78rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.04em;
    color: var(--text-muted);
    margin-bottom: 0.35rem;
}

.kpi-value {
    font-size: 1.6rem;
    font-weight: 800;
    color: var(--text-main);
    line-height: 1.15;
    font-family: var(--font-mono, monospace);
}

.kpi-card.highlight .kpi-value {
    color: var(--primary);
}

.kpi-sub {
    font-size: 0.8rem;
    color: var(--text-muted);
    margin-top: 0.35rem;
    display: flex;
    align-items: center;
    gap: 0.3rem;
}

.badge-surge {
    display: inline-flex;
    align-items: center;
    gap: 0.2rem;
    font-size: 0.74rem;
    font-weight: 700;
    color: #059669;
    background: rgba(16, 185, 129, 0.12);
    padding: 0.1rem 0.4rem;
    border-radius: 4px;
}

/* Section styling */
.t-section {
    margin-bottom: 2.25rem;
}

.t-section:last-child {
    margin-bottom: 0;
}

.section-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-bottom: 1.1rem;
    padding-bottom: 0.45rem;
    border-bottom: 1px solid var(--border);
}

.section-title-wrap {
    display: flex;
    align-items: center;
    gap: 0.55rem;
}

.section-icon {
    color: var(--primary);
    font-size: 1.1rem;
}

.section-title {
    font-size: 1.12rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.03em;
    color: var(--text-main);
    margin: 0;
}

/* Tables */
.table-responsive {
    width: 100%;
    overflow-x: auto;
    border: 1px solid var(--border);
    border-radius: var(--radius-md);
    background: var(--surface);
    margin-bottom: 1rem;
}

.transcript-table {
    width: 100%;
    border-collapse: collapse;
    font-size: 0.88rem;
    text-align: left;
}

.transcript-table th {
    background: var(--tag-bg);
    color: var(--text-main);
    font-weight: 700;
    padding: 0.65rem 0.85rem;
    border-bottom: 1px solid var(--border);
    white-space: nowrap;
}

.transcript-table td {
    padding: 0.6rem 0.85rem;
    border-bottom: 1px solid var(--border);
    color: var(--text-muted);
}

.transcript-table tr:last-child td {
    border-bottom: none;
}

.transcript-table tr:hover td {
    background: var(--tag-bg);
}

.course-title-cell {
    font-weight: 600;
    color: var(--text-main);
}

.grade-pill {
    font-family: var(--font-mono, monospace);
    font-weight: 700;
    font-size: 0.82rem;
    padding: 0.15rem 0.45rem;
    border-radius: 4px;
    display: inline-block;
}

.grade-excellent {
    background: rgba(16, 185, 129, 0.15);
    color: #059669;
    border: 1px solid rgba(16, 185, 129, 0.3);
}

.grade-verygood {
    background: rgba(2, 132, 199, 0.15);
    color: var(--primary);
    border: 1px solid rgba(2, 132, 199, 0.3);
}

.grade-good {
    background: rgba(245, 158, 11, 0.15);
    color: #d97706;
    border: 1px solid rgba(245, 158, 11, 0.3);
}

.grade-pass {
    background: rgba(100, 116, 139, 0.15);
    color: var(--text-muted);
    border: 1px solid var(--border);
}

/* Download Cards Grid */
.download-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1.15rem;
    margin-top: 1rem;
}

.download-card {
    background: var(--tag-bg);
    border: 1px solid var(--border);
    border-radius: var(--radius-md);
    padding: 1.25rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    transition: border-color 0.2s ease, box-shadow 0.2s ease;
}

.download-card:hover {
    border-color: var(--primary-border);
    box-shadow: var(--shadow-sm);
}

.download-card-header {
    display: flex;
    align-items: flex-start;
    gap: 0.75rem;
    margin-bottom: 0.85rem;
}

.download-card-icon {
    font-size: 1.5rem;
    color: var(--primary);
    flex-shrink: 0;
    margin-top: 0.15rem;
}

.download-card-title {
    font-size: 0.98rem;
    font-weight: 700;
    color: var(--text-main);
    margin: 0 0 0.2rem;
}

.download-card-desc {
    font-size: 0.82rem;
    color: var(--text-muted);
    margin: 0;
    line-height: 1.45;
}

.download-btn-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
    margin-top: 1.1rem;
    padding-top: 0.85rem;
    border-top: 1px solid var(--border);
}

.btn-dl {
    display: inline-flex;
    align-items: center;
    gap: 0.3rem;
    font-size: 0.76rem;
    font-weight: 600;
    padding: 0.35rem 0.65rem;
    border-radius: 4px;
    border: 1px solid var(--border);
    background: var(--surface);
    color: var(--text-main) !important;
    text-decoration: none !important;
    transition: all 0.15s ease;
}

.btn-dl:hover {
    border-color: var(--primary);
    color: var(--primary) !important;
    background: var(--primary-light);
}

.btn-dl-pdf {
    background: var(--primary);
    color: #ffffff !important;
    border-color: var(--primary);
}

.btn-dl-pdf:hover {
    background: var(--primary-dark);
    color: #ffffff !important;
}

/* Filter / Search Bar */
.filter-bar {
    display: flex;
    flex-wrap: wrap;
    gap: 0.6rem;
    margin-bottom: 1rem;
    align-items: center;
    justify-content: space-between;
}

.filter-buttons {
    display: flex;
    flex-wrap: wrap;
    gap: 0.35rem;
}

.filter-btn {
    font-size: 0.78rem;
    font-weight: 600;
    padding: 0.3rem 0.65rem;
    border-radius: 4px;
    border: 1px solid var(--border);
    background: var(--surface);
    color: var(--text-muted);
    cursor: pointer;
    transition: all 0.15s ease;
}

.filter-btn.active, .filter-btn:hover {
    background: var(--primary-light);
    border-color: var(--primary-border);
    color: var(--primary);
}

.filter-btn.active {
    font-weight: 700;
}

.search-input {
    font-size: 0.82rem;
    padding: 0.35rem 0.65rem;
    border-radius: var(--radius-sm);
    border: 1px solid var(--border);
    background: var(--surface);
    color: var(--text-main);
    outline: none;
    min-width: 180px;
}

.search-input:focus {
    border-color: var(--primary);
}

/* PDF Modal / Viewer */
.pdf-preview-box {
    display: none;
    margin-top: 1.25rem;
    border: 1px solid var(--border);
    border-radius: var(--radius-md);
    overflow: hidden;
    background: var(--surface);
}

.pdf-preview-box.active {
    display: block;
}

.pdf-preview-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.65rem 1rem;
    background: var(--tag-bg);
    border-bottom: 1px solid var(--border);
}

.pdf-preview-title {
    font-size: 0.88rem;
    font-weight: 700;
    color: var(--text-main);
}

.pdf-frame {
    width: 100%;
    height: 520px;
    border: none;
}

/* Notes & Legend */
.notes-card {
    background: var(--tag-bg);
    border-left: 3px solid var(--primary);
    padding: 1rem 1.25rem;
    border-radius: 0 var(--radius-sm) var(--radius-sm) 0;
    font-size: 0.84rem;
    color: var(--text-muted);
    line-height: 1.55;
}

.notes-card strong {
    color: var(--text-main);
}

@media (max-width: 640px) {
    .transcript-container {
        padding: 1.25rem 1rem;
    }
    .name-title h1 {
        font-size: 1.6rem;
    }
    .kpi-grid {
        grid-template-columns: 1fr 1fr;
    }
    .pdf-frame {
        height: 380px;
    }
}
</style>

<div class="transcript-container">

    <!-- Header -->
    <header class="transcript-header">
        <div class="header-top">
            <div class="name-title">
                <h1>Academic Transcripts & GPA Breakdown</h1>
                <div class="target-role">B.Sc. in Computer Engineering &bull; Artificial Intelligence Specialization</div>
                <div class="academic-subtext">
                    <strong>Institution:</strong> Islamic Azad University, North Tehran Branch (IAUNTB) &bull;
                    <strong>Status:</strong> 144 Completed Credits &bull; Unofficial Academic Evaluation
                </div>
            </div>
            <div class="header-actions">
                <a class="btn-action btn-action-primary" href="{{ '/assets/pdf/Yousef_Akbari_Last_2_Years_Transcript.pdf' | relative_url }}" target="_blank">
                    <i class="fa-solid fa-file-pdf"></i> Last 2 Years PDF
                </a>
                <button class="btn-action" onclick="togglePdfViewer('last2')">
                    <i class="fa-solid fa-eye"></i> Preview
                </button>
                <button class="btn-action" onclick="window.print()">
                    <i class="fa-solid fa-print"></i> Print
                </button>
            </div>
        </div>
    </header>

    <!-- Executive KPI Summary Cards -->
    <div class="kpi-grid">
        <div class="kpi-card highlight">
            <div class="kpi-label">Last 2 Years GPA (20-pt)</div>
            <div class="kpi-value">16.54<span style="font-size:0.95rem; font-weight:500; color:var(--text-muted);">/20</span></div>
            <div class="kpi-sub">
                <span class="badge-surge"><i class="fa-solid fa-arrow-trend-up"></i> 82.72%</span> First Class Equiv.
            </div>
        </div>

        <div class="kpi-card">
            <div class="kpi-label">WES Canada Scale</div>
            <div class="kpi-value">3.36<span style="font-size:0.95rem; font-weight:500; color:var(--text-muted);">/4.0</span></div>
            <div class="kpi-sub">
                <span class="badge-surge"><i class="fa-solid fa-arrow-trend-up"></i> +0.62</span> vs Cumulative (2.74)
            </div>
        </div>

        <div class="kpi-card">
            <div class="kpi-label">OMSAS Ontario Scale</div>
            <div class="kpi-value">3.61<span style="font-size:0.95rem; font-weight:500; color:var(--text-muted);">/4.0</span></div>
            <div class="kpi-sub">
                <span class="badge-surge"><i class="fa-solid fa-arrow-trend-up"></i> +0.39</span> vs Cumulative (3.22)
            </div>
        </div>

        <div class="kpi-card">
            <div class="kpi-label">Western Canada (UBC/SFU)</div>
            <div class="kpi-value">3.83<span style="font-size:0.95rem; font-weight:500; color:var(--text-muted);">/4.33</span></div>
            <div class="kpi-sub">
                <span class="badge-surge"><i class="fa-solid fa-arrow-trend-up"></i> +0.48</span> vs Cumulative (3.35)
            </div>
        </div>
    </div>

    <!-- Multi-Scale Conversion Matrix -->
    <section class="t-section">
        <div class="section-header">
            <div class="section-title-wrap">
                <span class="section-icon"><i class="fa-solid fa-scale-balanced"></i></span>
                <h2 class="section-title">Comparative GPA Conversion Matrix</h2>
            </div>
            <span style="font-size: 0.8rem; color: var(--text-muted);">Admissions Evaluation Baseline</span>
        </div>

        <div class="table-responsive">
            <table class="transcript-table">
                <thead>
                    <tr>
                        <th>Grading Standard / Evaluation Scale</th>
                        <th>Cumulative (144 Credits)</th>
                        <th>Last 2 Years / Senior ~60 Credits (59 Cr)</th>
                        <th>Academic Standing</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td class="course-title-cell">Weighted Average (Iranian 20-Point Scale)</td>
                        <td>14.61 / 20.00</td>
                        <td><strong style="color:var(--primary);">16.54 / 20.00</strong></td>
                        <td><span class="grade-pill grade-excellent">Distinction</span></td>
                    </tr>
                    <tr>
                        <td class="course-title-cell">Equivalent Percentage</td>
                        <td>73.03%</td>
                        <td><strong style="color:var(--primary);">82.72%</strong></td>
                        <td><span class="grade-pill grade-excellent">First Class</span></td>
                    </tr>
                    <tr>
                        <td class="course-title-cell">WES Canada Standard (4.00 Scale)</td>
                        <td>2.74 / 4.00</td>
                        <td><strong style="color:var(--primary);">3.36 / 4.00</strong></td>
                        <td><span class="grade-pill grade-verygood">Very Good / B+</span></td>
                    </tr>
                    <tr>
                        <td class="course-title-cell">OMSAS / Ontario Scale (4.00 with Sub-grades)</td>
                        <td>3.22 / 4.00</td>
                        <td><strong style="color:var(--primary);">3.61 / 4.00</strong></td>
                        <td><span class="grade-pill grade-excellent">A / Excellent</span></td>
                    </tr>
                    <tr>
                        <td class="course-title-cell">Western Canada Scale (4.33 Scale - UBC / SFU)</td>
                        <td>3.35 / 4.33</td>
                        <td><strong style="color:var(--primary);">3.83 / 4.33</strong></td>
                        <td><span class="grade-pill grade-excellent">A / Excellent</span></td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>

    <!-- Semester-by-Semester Progression -->
    <section class="t-section">
        <div class="section-header">
            <div class="section-title-wrap">
                <span class="section-icon"><i class="fa-solid fa-chart-line"></i></span>
                <h2 class="section-title">Last 2 Years Semester Progression</h2>
            </div>
            <span style="font-size: 0.8rem; color: var(--text-muted);">Senior Specialization & Upward Trajectory</span>
        </div>

        <div class="table-responsive">
            <table class="transcript-table">
                <thead>
                    <tr>
                        <th>Semester / Academic Term</th>
                        <th>Credits</th>
                        <th>Iranian Avg (0–20)</th>
                        <th>Percentage</th>
                        <th>Std Canadian (4.0)</th>
                        <th>WES Canada (4.0)</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td class="course-title-cell">First Semester 1399-1400 (Fall 2020)</td>
                        <td>16</td>
                        <td>12.97</td>
                        <td>64.84%</td>
                        <td>2.41</td>
                        <td>2.00</td>
                    </tr>
                    <tr>
                        <td class="course-title-cell">First Semester 1400-1401 (Fall 2021)</td>
                        <td>17</td>
                        <td>14.85</td>
                        <td>74.26%</td>
                        <td>2.99</td>
                        <td>2.94</td>
                    </tr>
                    <tr>
                        <td class="course-title-cell">Second Semester 1400-1401 (Spring 2022)</td>
                        <td>21</td>
                        <td><strong style="color: #059669;">18.74</strong></td>
                        <td><strong>93.69%</strong></td>
                        <td><strong style="color: #059669;">3.96</strong></td>
                        <td><strong style="color: #059669;">4.00</strong></td>
                    </tr>
                    <tr>
                        <td class="course-title-cell">Summer Semester 1400-1401 (Summer 2022)</td>
                        <td>7</td>
                        <td><strong style="color: #059669;">16.87</strong></td>
                        <td><strong>84.36%</strong></td>
                        <td><strong style="color: #059669;">3.57</strong></td>
                        <td><strong style="color: #059669;">3.57</strong></td>
                    </tr>
                    <tr>
                        <td class="course-title-cell">First Semester 1401-1402 (Fall 2022)</td>
                        <td>4</td>
                        <td><strong style="color: #059669;">17.75</strong></td>
                        <td><strong>88.75%</strong></td>
                        <td><strong style="color: #059669;">4.00</strong></td>
                        <td><strong style="color: #059669;">4.00</strong></td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>

    <!-- Detailed Coursework Breakdown Table -->
    <section class="t-section">
        <div class="section-header">
            <div class="section-title-wrap">
                <span class="section-icon"><i class="fa-solid fa-graduation-cap"></i></span>
                <h2 class="section-title">Coursework Details (Last 2 Years / 29 Courses)</h2>
            </div>
            <span style="font-size: 0.8rem; color: var(--text-muted);">65 Completed Credits</span>
        </div>

        <!-- Filter & Search Controls -->
        <div class="filter-bar">
            <div class="filter-buttons">
                <button class="filter-btn active" onclick="filterCourses('all', this)">All Semesters (29)</button>
                <button class="filter-btn" onclick="filterCourses('ai', this)">AI & Core CS (8)</button>
                <button class="filter-btn" onclick="filterCourses('1400-spring', this)">Spring 2022 (9)</button>
                <button class="filter-btn" onclick="filterCourses('1400-fall', this)">Fall 2021 (7)</button>
                <button class="filter-btn" onclick="filterCourses('1399-fall', this)">Fall 2020 (6)</button>
            </div>
            <input type="text" id="courseSearch" class="search-input" placeholder="Search course name..." onkeyup="searchCourses()">
        </div>

        <div class="table-responsive">
            <table class="transcript-table" id="courseTable">
                <thead>
                    <tr>
                        <th>Semester</th>
                        <th>Course Title</th>
                        <th>Type</th>
                        <th>Credits</th>
                        <th>Iranian Score (/20)</th>
                        <th>Letter & Equiv.</th>
                    </tr>
                </thead>
                <tbody>
                    <!-- Fall 2020 -->
                    <tr data-sem="1399-fall" data-cat="cs">
                        <td>Fall 1399-1400</td>
                        <td class="course-title-cell">Software Engineering 2</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>12.00</td>
                        <td><span class="grade-pill grade-pass">C (2.0)</span></td>
                    </tr>
                    <tr data-sem="1399-fall" data-cat="cs">
                        <td>Fall 1399-1400</td>
                        <td class="course-title-cell">Signals and Systems</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>10.00</td>
                        <td><span class="grade-pill grade-pass">D (1.0)</span></td>
                    </tr>
                    <tr data-sem="1399-fall" data-cat="cs">
                        <td>Fall 1399-1400</td>
                        <td class="course-title-cell">Object-Oriented Systems Design</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>13.50</td>
                        <td><span class="grade-pill grade-pass">C+ (2.3)</span></td>
                    </tr>
                    <tr data-sem="1399-fall" data-cat="cs">
                        <td>Fall 1399-1400</td>
                        <td class="course-title-cell">Microprocessors and Assembly Language</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>11.00</td>
                        <td><span class="grade-pill grade-pass">D+ (1.3)</span></td>
                    </tr>
                    <tr data-sem="1399-fall" data-cat="gen">
                        <td>Fall 1399-1400</td>
                        <td class="course-title-cell">Analytical History of Early Islam</td>
                        <td>Theoretical</td>
                        <td>2.0</td>
                        <td>18.50</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>
                    <tr data-sem="1399-fall" data-cat="gen">
                        <td>Fall 1399-1400</td>
                        <td class="course-title-cell">Thematic Interpretation of Nahj al-Balagha</td>
                        <td>Theoretical</td>
                        <td>2.0</td>
                        <td>15.50</td>
                        <td><span class="grade-pill grade-good">B+ (3.3)</span></td>
                    </tr>

                    <!-- Fall 2021 -->
                    <tr data-sem="1400-fall" data-cat="cs">
                        <td>Fall 1400-1401</td>
                        <td class="course-title-cell">Differential Equations</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>17.00</td>
                        <td><span class="grade-pill grade-verygood">A (3.9)</span></td>
                    </tr>
                    <tr data-sem="1400-fall" data-cat="cs">
                        <td>Fall 1400-1401</td>
                        <td class="course-title-cell">Programming Languages Design</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>12.00</td>
                        <td><span class="grade-pill grade-pass">C (2.0)</span></td>
                    </tr>
                    <tr data-sem="1400-fall" data-cat="ai">
                        <td>Fall 1400-1401</td>
                        <td class="course-title-cell">Fundamentals of Computational Intelligence (AI)</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>17.00</td>
                        <td><span class="grade-pill grade-verygood">A (3.9)</span></td>
                    </tr>
                    <tr data-sem="1400-fall" data-cat="gen">
                        <td>Fall 1400-1401</td>
                        <td class="course-title-cell">Familiarity with the Holy Quran</td>
                        <td>Theoretical</td>
                        <td>1.0</td>
                        <td>20.00</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>
                    <tr data-sem="1400-fall" data-cat="cs">
                        <td>Fall 1400-1401</td>
                        <td class="course-title-cell">Operating Systems</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>10.00</td>
                        <td><span class="grade-pill grade-pass">D (1.0)</span></td>
                    </tr>
                    <tr data-sem="1400-fall" data-cat="cs">
                        <td>Fall 1400-1401</td>
                        <td class="course-title-cell">Digital Systems Computer-Aided Design (CAD)</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>18.00</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>
                    <tr data-sem="1400-fall" data-cat="cs">
                        <td>Fall 1400-1401</td>
                        <td class="course-title-cell">Physics Laboratory 2</td>
                        <td>Practical</td>
                        <td>1.0</td>
                        <td>10.50</td>
                        <td><span class="grade-pill grade-pass">D+ (1.3)</span></td>
                    </tr>

                    <!-- Spring 2022 -->
                    <tr data-sem="1400-spring" data-cat="gen">
                        <td>Spring 1400-1401</td>
                        <td class="course-title-cell">Thoughts of the Imams of the Islamic Revolution</td>
                        <td>Theoretical</td>
                        <td>1.0</td>
                        <td>18.00</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>
                    <tr data-sem="1400-spring" data-cat="ai cs">
                        <td>Spring 1400-1401</td>
                        <td class="course-title-cell">Computer Networks</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>19.00</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>
                    <tr data-sem="1400-spring" data-cat="ai cs">
                        <td>Spring 1400-1401</td>
                        <td class="course-title-cell">Internet Engineering</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>19.75</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>
                    <tr data-sem="1400-spring" data-cat="ai">
                        <td>Spring 1400-1401</td>
                        <td class="course-title-cell">Fundamentals of Speech and Language Processing (NLP)</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>19.50</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>
                    <tr data-sem="1400-spring" data-cat="ai">
                        <td>Spring 1400-1401</td>
                        <td class="course-title-cell">Robotics Principles</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>16.75</td>
                        <td><span class="grade-pill grade-verygood">A- (3.7)</span></td>
                    </tr>
                    <tr data-sem="1400-spring" data-cat="ai">
                        <td>Spring 1400-1401</td>
                        <td class="course-title-cell">Fundamentals of Computer Vision</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>17.75</td>
                        <td><span class="grade-pill grade-verygood">A (3.9)</span></td>
                    </tr>
                    <tr data-sem="1400-spring" data-cat="ai cs">
                        <td>Spring 1400-1401</td>
                        <td class="course-title-cell">Software Project (Senior Thesis / Capstone)</td>
                        <td>Practical</td>
                        <td>3.0</td>
                        <td>20.00</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>
                    <tr data-sem="1400-spring" data-cat="gen">
                        <td>Spring 1400-1401</td>
                        <td class="course-title-cell">Physical Education</td>
                        <td>Theo/Prac</td>
                        <td>1.0</td>
                        <td>19.00</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>
                    <tr data-sem="1400-spring" data-cat="cs">
                        <td>Spring 1400-1401</td>
                        <td class="course-title-cell">Microprocessor Laboratory 1</td>
                        <td>Practical</td>
                        <td>1.0</td>
                        <td>18.25</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>

                    <!-- Summer 2022 -->
                    <tr data-sem="1400-summer" data-cat="cs">
                        <td>Summer 1400-1401</td>
                        <td class="course-title-cell">Engineering Mathematics</td>
                        <td>Theoretical</td>
                        <td>3.0</td>
                        <td>14.70</td>
                        <td><span class="grade-pill grade-good">B (3.0)</span></td>
                    </tr>
                    <tr data-sem="1400-summer" data-cat="cs">
                        <td>Summer 1400-1401</td>
                        <td class="course-title-cell">Logic Circuits and Computer Architecture Lab</td>
                        <td>Practical</td>
                        <td>1.0</td>
                        <td>20.00</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>
                    <tr data-sem="1400-summer" data-cat="gen">
                        <td>Summer 1400-1401</td>
                        <td class="course-title-cell">Sports 1</td>
                        <td>Practical</td>
                        <td>1.0</td>
                        <td>17.00</td>
                        <td><span class="grade-pill grade-verygood">A (3.9)</span></td>
                    </tr>
                    <tr data-sem="1400-summer" data-cat="cs">
                        <td>Summer 1400-1401</td>
                        <td class="course-title-cell">Internship (Industry Practicum)</td>
                        <td>Practical</td>
                        <td>1.0</td>
                        <td>20.00</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>
                    <tr data-sem="1400-summer" data-cat="cs">
                        <td>Summer 1400-1401</td>
                        <td class="course-title-cell">Computer Workshop</td>
                        <td>Practical</td>
                        <td>1.0</td>
                        <td>17.00</td>
                        <td><span class="grade-pill grade-verygood">A (3.9)</span></td>
                    </tr>

                    <!-- Fall 2022 -->
                    <tr data-sem="1401-fall" data-cat="gen">
                        <td>Fall 1401-1402</td>
                        <td class="course-title-cell">History of Islamic and Iranian Culture & Civilization</td>
                        <td>Theoretical</td>
                        <td>2.0</td>
                        <td>18.00</td>
                        <td><span class="grade-pill grade-excellent">A+ (4.0)</span></td>
                    </tr>
                    <tr data-sem="1401-fall" data-cat="gen">
                        <td>Fall 1401-1402</td>
                        <td class="course-title-cell">Familiarity with Sacred Defense</td>
                        <td>Theoretical</td>
                        <td>2.0</td>
                        <td>17.50</td>
                        <td><span class="grade-pill grade-verygood">A (3.9)</span></td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>

    <!-- Download Center & Document Hub -->
    <section class="t-section">
        <div class="section-header">
            <div class="section-title-wrap">
                <span class="section-icon"><i class="fa-solid fa-folder-open"></i></span>
                <h2 class="section-title">Official Download Center & Datasets</h2>
            </div>
            <span style="font-size: 0.8rem; color: var(--text-muted);">PDF, CSV & Excel Formats</span>
        </div>

        <div class="download-grid">
            <!-- Card 1: Last 2 Years -->
            <div class="download-card">
                <div>
                    <div class="download-card-header">
                        <i class="fa-solid fa-file-lines download-card-icon"></i>
                        <div>
                            <h3 class="download-card-title">Last 2 Years Unofficial Transcript</h3>
                            <p class="download-card-desc">
                                Senior curriculum breakdown (59-65 credits) covering specialized AI, systems, and engineering courses with GPA calculations.
                            </p>
                        </div>
                    </div>
                </div>
                <div class="download-btn-row">
                    <a class="btn-dl btn-dl-pdf" href="{{ '/assets/pdf/Yousef_Akbari_Last_2_Years_Transcript.pdf' | relative_url }}" target="_blank">
                        <i class="fa-solid fa-file-pdf"></i> PDF
                    </a>
                    <a class="btn-dl" href="{{ '/assets/Transcripts/last_2_years_transcript.csv' | relative_url }}" download>
                        <i class="fa-solid fa-file-csv"></i> CSV
                    </a>
                    <a class="btn-dl" href="{{ '/assets/Transcripts/last_2_years_transcript.xlsx' | relative_url }}" download>
                        <i class="fa-solid fa-file-excel"></i> Excel
                    </a>
                    <button class="btn-dl" onclick="togglePdfViewer('last2')">
                        <i class="fa-solid fa-eye"></i> Preview
                    </button>
                </div>
            </div>

            <!-- Card 2: Full Transcript -->
            <div class="download-card">
                <div>
                    <div class="download-card-header">
                        <i class="fa-solid fa-graduation-cap download-card-icon"></i>
                        <div>
                            <h3 class="download-card-title">Full Unofficial Transcript</h3>
                            <p class="download-card-desc">
                                Complete 144-credit academic record spanning all undergraduate coursework, semester averages, and multi-scale conversion data.
                            </p>
                        </div>
                    </div>
                </div>
                <div class="download-btn-row">
                    <a class="btn-dl btn-dl-pdf" href="{{ '/assets/pdf/Yousef_Akbari_Full_Unofficial_Transcript.pdf' | relative_url }}" target="_blank">
                        <i class="fa-solid fa-file-pdf"></i> PDF
                    </a>
                    <a class="btn-dl" href="{{ '/assets/Transcripts/full_transcript.csv' | relative_url }}" download>
                        <i class="fa-solid fa-file-csv"></i> CSV
                    </a>
                    <a class="btn-dl" href="{{ '/assets/Transcripts/full_transcript.xlsx' | relative_url }}" download>
                        <i class="fa-solid fa-file-excel"></i> Excel
                    </a>
                    <button class="btn-dl" onclick="togglePdfViewer('full')">
                        <i class="fa-solid fa-eye"></i> Preview
                    </button>
                </div>
            </div>
        </div>

        <!-- Inline PDF Preview Container -->
        <div id="pdfViewerContainer" class="pdf-preview-box">
            <div class="pdf-preview-header">
                <span id="pdfViewerTitle" class="pdf-preview-title">Document Preview</span>
                <button class="btn-dl" onclick="closePdfViewer()">
                    <i class="fa-solid fa-xmark"></i> Close Preview
                </button>
            </div>
            <iframe id="pdfFrame" class="pdf-frame" src=""></iframe>
        </div>
    </section>

    <!-- Notes & Scale Context for Graduate Committees -->
    <section class="t-section">
        <div class="notes-card">
            <strong>Notes on Grading System & Conversions for Graduate Admissions:</strong>
            <ul style="margin: 0.4rem 0 0; padding-left: 1.2rem; font-size: 0.82rem;">
                <li>The Iranian university grading system utilizes a 0–20 scale where 10.00 is the minimum passing grade for undergraduate courses, and scores above 16.00 indicate superior distinction.</li>
                <li><strong>Senior Year Performance Surge:</strong> Demonstrated substantial upward academic momentum in upper-division coursework, attaining a weighted GPA of <strong>16.54 / 20.00 (82.72%)</strong> in the last 2 years, with top scores in Computer Vision (17.75), Speech & NLP (19.50), Computer Networks (19.00), Internet Engineering (19.75), and Capstone Software Project (20.00).</li>
                <li>GPA conversions follow standard WES Canada (World Education Services) and OMSAS (Ontario Medical & Graduate School Applications) conversion frameworks.</li>
            </ul>
        </div>
    </section>

</div>

<script>
function filterCourses(category, btn) {
    const buttons = document.querySelectorAll('.filter-btn');
    buttons.forEach(b => b.classList.remove('active'));
    if (btn) btn.classList.add('active');

    const rows = document.querySelectorAll('#courseTable tbody tr');
    rows.forEach(row => {
        if (category === 'all') {
            row.style.display = '';
        } else if (category === 'ai') {
            if (row.dataset.cat && row.dataset.cat.includes('ai')) {
                row.style.display = '';
            } else {
                row.style.display = 'none';
            }
        } else {
            if (row.dataset.sem === category) {
                row.style.display = '';
            } else {
                row.style.display = 'none';
            }
        }
    });
}

function searchCourses() {
    const input = document.getElementById('courseSearch');
    const filter = input.value.toLowerCase();
    const rows = document.querySelectorAll('#courseTable tbody tr');

    rows.forEach(row => {
        const title = row.querySelector('.course-title-cell').innerText.toLowerCase();
        if (title.indexOf(filter) > -1) {
            row.style.display = '';
        } else {
            row.style.display = 'none';
        }
    });
}

function togglePdfViewer(type) {
    const box = document.getElementById('pdfViewerContainer');
    const frame = document.getElementById('pdfFrame');
    const title = document.getElementById('pdfViewerTitle');
    
    let url = '';
    if (type === 'last2') {
        url = "{{ '/assets/pdf/Yousef_Akbari_Last_2_Years_Transcript.pdf' | relative_url }}";
        title.innerText = 'Document Preview: Last 2 Years Unofficial Transcript (PDF)';
    } else {
        url = "{{ '/assets/pdf/Yousef_Akbari_Full_Unofficial_Transcript.pdf' | relative_url }}";
        title.innerText = 'Document Preview: Full Unofficial Academic Transcript (PDF)';
    }

    frame.src = url;
    box.classList.add('active');
    box.scrollIntoView({ behavior: 'smooth', block: 'start' });
}

function closePdfViewer() {
    const box = document.getElementById('pdfViewerContainer');
    const frame = document.getElementById('pdfFrame');
    frame.src = '';
    box.classList.remove('active');
}
</script>
