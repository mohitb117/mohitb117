<style>
  /* Resume Styling - Medium Format with Multi-column Layout */
  body {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    line-height: 1.25;
    color: #1f2937;
    max-width: 1100px;
    margin: 0 auto;
    padding: 12px 20px;
    background: #ffffff;
    font-size: 0.93em;
  }

  p {
    margin: 0.3em 0;
    line-height: 1.3;
  }

  /* Header Section with Photo */
  .header-container {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 8px;
    padding-bottom: 6px;
    border-bottom: 2px solid #e5e7eb;
  }

  .profile-photo {
    flex-shrink: 0;
  }

  .profile-photo img {
    width: 70px;
    height: 70px;
    border-radius: 4px;
    border: 1px solid #d1d5db;
    object-fit: cover;
    display: block;
  }

  .header-info {
    flex-grow: 1;
  }

  h1 {
    color: #1a1a1a;
    font-size: 1.4em;
    margin: 0;
    padding: 0;
    font-weight: 700;
    line-height: 1.2;
  }

  .contact-info {
    font-size: 0.85em;
    line-height: 1.3;
    margin-top: 2px;
  }

  .contact-item {
    display: inline;
    white-space: nowrap;
  }

  .contact-item:not(:last-child)::after {
    content: " | ";
    margin: 0 8px;
    color: #9ca3af;
  }

  .contact-info a {
    color: #2563eb;
    text-decoration: none;
  }

  .contact-info a:hover {
    text-decoration: underline;
  }

  .contact-text {
    color: #374151;
  }

  /* Section Styling */
  h2 {
    color: #2563eb !important;
    font-size: 1.3em;
    margin-top: 0.6em;
    margin-bottom: 0.3em;
    padding-bottom: 3px;
    border-bottom: 2px solid #2563eb;
    font-weight: 600;
  }

  h3 {
    color: #1a1a1a !important;
    font-size: 1em;
    margin-top: 0.5em;
    margin-bottom: 0.2em;
    font-weight: 600;
    line-height: 1.2;
  }

  /* Job Entry Styling */
  .job-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 8px;
    margin-bottom: 3px;
    margin-top: 0.4em;
  }

  .job-header-left {
    display: flex;
    align-items: center;
    gap: 12px;
  }

  .company-logo {
    width: 32px;
    height: 32px;
    flex-shrink: 0;
  }

  .company-logo img {
    width: 100%;
    height: 100%;
    object-fit: contain;
  }

  .job-title {
    color: #059669;
    font-weight: 700;
  }

  .company-name {
    color: #1f2937;
    font-weight: 700;
    font-size: 1.1em;
  }

  .date-range {
    color: #6b7280;
    font-style: italic;
    font-size: 0.95em;
    white-space: nowrap;
  }

  .job-separator {
    color: #d1d5db;
    margin: 0 8px;
  }

  /* Multi-column Skills Layout */
  .skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 10px;
    margin: 0.6em 0;
  }

  .skill-category {
    background: #f9fafb;
    padding: 10px;
    border-radius: 6px;
    border-left: 4px solid #2563eb;
  }

  .skill-category-title {
    color: #1f2937;
    font-weight: 700;
    display: block;
    margin-bottom: 4px;
    font-size: 0.95em;
  }

  .skill-category-content {
    color: #4b5563;
    line-height: 1.5;
  }

  /* Education Section */
  .education-entry {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 0.4em;
  }

  .education-logo {
    width: 28px;
    height: 28px;
    flex-shrink: 0;
  }

  .education-logo img {
    width: 100%;
    height: 100%;
    object-fit: contain;
  }

  /* List Styling */
  ul {
    margin-top: 0.1em;
    margin-bottom: 0.3em;
    padding-left: 18px;
  }

  li {
    margin-bottom: 0.1em;
    line-height: 1.3;
    color: #374151;
  }

  li::marker {
    color: #2563eb;
  }

  /* Table Styling */
  table {
    border-collapse: separate;
    border-spacing: 0 6px;
    width: 100%;
    margin: 0.4em 0;
  }

  th {
    display: none;
  }

  td {
    padding: 10px;
    text-align: left;
    background: linear-gradient(135deg, #ffffff 0%, #f8fafc 100%);
    border-radius: 8px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
    border-left: 4px solid #2563eb;
    transition: all 0.3s ease;
    color: #1f2937 !important;
  }

  td strong {
    color: #1a1a1a !important;
  }

  td a {
    color: #2563eb !important;
  }

  tr:first-child td {
    border-left-color: #f59e0b;
    background: linear-gradient(135deg, #fffbeb 0%, #fef3c7 100%);
  }

  tr:nth-child(2) td {
    border-left-color: #0ea5e9;
    background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
  }

  tr:nth-child(3) td {
    border-left-color: #8b5cf6;
    background: linear-gradient(135deg, #faf5ff 0%, #f3e8ff 100%);
  }

  tr:nth-child(4) td {
    border-left-color: #10b981;
    background: linear-gradient(135deg, #f0fdf4 0%, #dcfce7 100%);
  }

  tr:nth-child(5) td {
    border-left-color: #ec4899;
    background: linear-gradient(135deg, #fdf2f8 0%, #fce7f3 100%);
  }

  tr:hover td {
    transform: translateY(-4px);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.12);
  }

  /* Links and Highlights */
  .patent-link, .award-link {
    color: #2563eb;
    font-size: 0.9em;
  }

  strong {
    color: #1a1a1a !important;
    font-weight: 600;
  }

  p, span, div {
    color: #1f2937 !important;
  }

  /* Section Dividers */
  hr {
    border: none;
    border-top: 1px solid #e5e7eb;
    margin: 1em 0;
  }

  /* Project Section */
  .project-header {
    background: #f9fafb;
    padding: 10px 12px;
    border-radius: 6px;
    border-left: 4px solid #7c3aed;
    margin-bottom: 6px;
  }

  .project-title {
    color: #1f2937;
    font-weight: 700;
    font-size: 1.05em;
    margin-bottom: 3px;
  }

  .project-meta {
    color: #6b7280;
    font-size: 0.85em;
  }

  /* Patents Section */
  .patent-box {
    background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
    padding: 12px;
    border-radius: 6px;
    border-left: 4px solid #0ea5e9;
    margin: 0.6em 0;
  }

  .patent-title {
    color: #1f2937;
    font-weight: 700;
    font-size: 1em;
    margin-bottom: 4px;
  }

  /* Print Optimization */
  @media print {
    body {
      max-width: 100%;
      padding: 20px;
    }
    .header-container {
      page-break-after: avoid;
    }
    h2 {
      page-break-after: avoid;
    }
  }

  /* Responsive Design */
  @media (max-width: 768px) {
    .header-container {
      flex-direction: column;
      text-align: center;
    }

    h1 {
      font-size: 2.2em;
    }

    .contact-info {
      grid-template-columns: 1fr;
    }

    .skills-grid {
      grid-template-columns: 1fr;
    }

    .job-header {
      flex-direction: column;
      align-items: flex-start;
    }
  }
</style>

<div class="header-container">
  <div class="profile-photo">
    <img src="https://avatars.githubusercontent.com/u/3359983" alt="Mohit Bhalla">
  </div>
  <div class="header-info">
    <h1>Mohit Bhalla</h1>
    <div class="contact-info">
      <div class="contact-item">
        <span class="contact-text">Nashville, TN</span>
      </div>
      <div class="contact-item">
        <span class="contact-text">315-897-7702</span>
      </div>
      <div class="contact-item">
        <a href="mailto:mohitb117@gmail.com">mohitb117@gmail.com</a>
      </div>
      <div class="contact-item">
        <a href="https://github.com/mohitb117">GitHub</a>
      </div>
      <div class="contact-item">
        <a href="https://www.linkedin.com/in/mohitb117">LinkedIn</a>
      </div>
    </div>
  </div>
</div>

<h2>Professional Experience</h2>

<div class="job-header">
  <div class="job-header-left">
    <div class="company-logo">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/DoorDash_Logo.svg/2880px-DoorDash_Logo.svg.png" alt="DoorDash">
    </div>
    <span><span class="company-name">DoorDash - Grocery</span><span class="job-separator">|</span><span class="job-title">Sr. Software Engineer | New Verticals Mobile Tech Lead</span></span>
  </div>
  <span class="date-range">Nov '21 - Present (3+ years)</span>
</div>

<p>Mobile Technical Lead building Android and backend features while leading iOS engineers to architect scalable solutions. Built Order Confirmation UI, Dynamic Delivery Options framework, migrated 30+ post-checkout features to unified Consumer Android app with split shipment support. Led on-call operations, mentored engineers, and drove code craftsmanship initiatives across Mobile and Backend teams.</p>

<div class="job-header">
  <div class="job-header-left">
    <div class="company-logo">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/06/Amazon_2024.svg/2880px-Amazon_2024.svg.png" alt="Amazon">
    </div>
    <span><span class="company-name">Amazon</span><span class="job-separator">|</span><span class="job-title">Software Engineer → Sr. Software Engineer</span></span>
  </div>
  <span class="date-range">Dec '15 - Nov '21 (6 years)</span>
</div>

<p><strong>Amazon Care (Sr. SDE, Apr '18 - Nov '21)</strong> - Built Audio/Video conferencing capability using WebRTC with real-time quality monitoring (<a href="https://patents.google.com/patent/US11038933B1/">USPTO Patent US11038933B1</a>). Led Kotlin migration and Coroutines adoption across Android team. Modularized codebase for faster compilation. Built AWS backend infrastructure for high-volume customer metrics.</p>

<p><strong>AWS Silk Browser (SDE, Dec '15 - Apr '18)</strong> - Led development of leanback experience for Silk on FireTV including HomeMenu launcher and Optimal Navigational Cursor implementation. Implemented Intent Handling for FireTablets/FireTV. Optimized memory usage and performance.</p>

<div class="job-header">
  <div class="job-header-left">
    <div class="company-logo">
      <img src="https://upload.wikimedia.org/wikipedia/commons/e/e9/INRIX_logo.png" alt="INRIX">
    </div>
    <span><span class="company-name">INRIX Inc.</span><span class="job-separator">|</span><span class="job-title">Software Development Engineer</span></span>
  </div>
  <span class="date-range">Oct '14 - Dec '15</span>
</div>

<p>Android Mobile Development for real-time traffic information delivery platform serving business and consumer markets.</p>

<div class="job-header">
  <div class="job-header-left">
    <div class="company-logo">
      <img src="https://upload.wikimedia.org/wikipedia/commons/e/eb/PNNL_CENTER_FullColorSMALL.jpg" alt="PNNL">
    </div>
    <span><span class="company-name">Pacific Northwest National Laboratory</span> (US Dept. of Energy) <span class="job-separator">|</span> <span class="job-title">Software Engineering Intern</span></span>
  </div>
  <span class="date-range">Summer 2013 & 2014</span>
</div>

<p>Primary developer for Android bio surveillance application using Java EE Framework. Built real-time server-client architecture with push notifications and News Feed. <strong>Won 1st Place</strong> in Mobile App Development Competition among team of 4 interns.</p>

<hr>

<h2>Education</h2>

<div class="education-entry">
  <div class="education-logo">
    <img src="https://upload.wikimedia.org/wikipedia/commons/4/49/Syracuse_Orange_logo.svg" alt="Syracuse University">
  </div>
  <div>
    <strong>Master of Science in Computer Engineering</strong> | Syracuse University | May 2014 | GPA: 3.55/4.0
  </div>
</div>

<div class="education-entry">
  <div class="education-logo">
    <img src="https://upload.wikimedia.org/wikipedia/en/thumb/b/b8/GGSIU_logo.svg/2560px-GGSIU_logo.svg.png" alt="GGSIPU">
  </div>
  <div>
    <strong>Bachelor of Technology in Computer Science</strong> | Guru Gobind Singh Indraprastha University, New Delhi, India | Aug 2012 | GPA: 3.97/4.0
  </div>
</div>

<hr>

<h2>Technical Skills</h2>

<div class="skills-grid">
  <div class="skill-category">
    <span class="skill-category-title"> Mobile Full-Stack Development</span>
    <div class="skill-category-content">
      Android SDK • Kotlin • Java • Jetpack Compose • Kotlin Coroutines • WebRTC • Server-Driven UI • REST APIs • GraphQL • Backend Integration • Mobile App Architecture
    </div>
  </div>

  <div class="skill-category">
    <span class="skill-category-title"> Platform & Infrastructure</span>
    <div class="skill-category-content">
      AWS Backend Infrastructure • CI/CD Pipelines • Performance Optimization • Memory Management • Modularization • Testing (Unit, Integration, Screenshot)
    </div>
  </div>

  <div class="skill-category">
    <span class="skill-category-title"> Observability & Leadership</span>
    <div class="skill-category-content">
      Telemetry & Metrics • A/B Testing • Experimentation Platforms • On-Call & Incident Management • Code Reviews • Technical Mentorship
    </div>
  </div>
</div>

<hr>

<h2>Highlights & Recognition</h2>

<table>
<tr>
<td>
<strong>1st Place - Mobile App Development Competition (2014)</strong><br>
<strong>Food Feed Bio Surveillance App</strong> - PNNL / US Dept. of Energy<br>
Primary Software Developer in team of 4. Built full-stack Android app using Java EE with real-time data delivery via push notifications and News Feed for bio surveillance monitoring.<br>
<span class="award-link"><a href="https://www.youtube.com/watch?v=HVIy1bWt29Y">Video</a> | <a href="http://www.pnnl.gov/news/release.aspx?id=1015">Press Release</a> | <a href="https://www.newswise.com/articles/killer-apps-that-could-keep-you-healthy">Newswise</a></span>
</td>
</tr>
<tr>
<td>
<strong>US Patent 11038933B1 (2018-21)</strong><br>
<strong>WebRTC Quality Monitoring</strong> - Amazon Care Platform<br>
Real-time quality monitoring for WebRTC audio/video conferencing - Awarded for innovative work on Amazon Care's video conferencing platform.<br>
<span class="patent-link"><a href="https://patents.google.com/patent/US11038933B1/">View Patent →</a></span>
</td>
</tr>
<tr>
<td>
<strong>Merit Scholarship (2012-14)</strong><br>
<strong>Syracuse University Graduate Program</strong> - Computer Engineering<br>
50% Tuition Coverage for academic excellence in Master's program.
</td>
</tr>
<tr>
<td>
<strong>2nd Place - INNOVISION Linux Challenge (2011)</strong><br>
<strong>Netaji Subas Institute of Technology</strong> - Sponsored by IEEE India<br>
Annual tech fest competition demonstrating Linux system expertise.
</td>
</tr>
<tr>
<td>
<strong>2nd Place - Embedded Systems Design (2009)</strong><br>
<strong>Programming Competition</strong><br>
National level competition for embedded systems programming.
</td>
</tr>
</table>


