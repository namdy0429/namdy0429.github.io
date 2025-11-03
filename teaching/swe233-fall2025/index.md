---
layout: page
title: "SWE 233: Intelligent User Interfaces"
permalink: /teaching/swe233-fall2025/
---

<!-- Custom Styles -->
<style>
/* Floating Table of Contents */
.floating-toc {
  position: fixed;
  top: 100px;
  left: 20px;
  width: 250px;
  max-height: 70vh;
  overflow-y: auto;
  background: none;
  border: none;
  padding: 15px;
  font-size: 0.85rem;
  z-index: 1000;
}

.floating-toc h4 {
  margin: 0 0 10px 0;
  font-size: 0.9rem;
  color: #333;
  border-bottom: 1px solid #ddd;
  padding-bottom: 5px;
  display: none;
}

.floating-toc ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.floating-toc li {
  margin: 3px 0;
}

.floating-toc a {
  text-decoration: none;
  color: #0083b3;
  display: block;
  padding: 2px 0;
  border-left: 2px solid transparent;
  padding-left: 8px;
}

.floating-toc a:hover {
  color: #255799;
  text-decoration: underline;
}

.floating-toc ul ul {
  margin-left: 15px;
  margin-top: 5px;
}

.floating-toc ul ul li {
  margin: 2px 0;
}

.floating-toc ul ul a {
  font-size: 0.8rem;
  color: #666;
  padding-left: 5px;
}

.floating-toc ul ul a:hover {
  color: #0083b3;
}

/* Responsive TOC */
@media (max-width: 1200px) {
  .floating-toc {
    position: static;
    width: 100%;
    max-height: none;
    margin: 20px 0;
    background: none;
    border-left: 3px solid #0083b3;
    padding-left: 20px;
  }

  .floating-toc h4 {
    cursor: pointer;
    display: block;
  }

  .floating-toc h4:after {
    content: " ▼";
    float: right;
    transition: transform 0.2s;
  }

  .floating-toc.collapsed h4:after {
    transform: rotate(-90deg);
  }

  .floating-toc.collapsed ul {
    display: none;
  }
}

@media (max-width: 768px) {
  .floating-toc {
    margin: 15px 0;
    border-left: 3px solid #0083b3;
    padding-left: 20px;
  }
}

/* Schedule Table Styling */
.schedule-table {
  width: 100%;
  border-collapse: collapse;
  margin: 20px 0;
  font-size: 0.9rem;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  border-radius: 8px;
  overflow: hidden;
}

.schedule-table th {
  background-color: #f8f9fa;
  color: #333;
  font-weight: 500;
  padding: 12px;
  text-align: left;
  border-bottom: 2px solid #e0e0e0;
  font-size: 0.85rem;
  text-transform: uppercase;
  letter-spacing: 0.5px;
}

.schedule-table td {
  padding: 12px;
  border-bottom: 1px solid #e0e0e0;
  vertical-align: top;
}

.schedule-table tbody tr:hover {
  background-color: #f8f9fa;
  transition: background-color 0.2s ease;
}

.schedule-table tbody tr:nth-child(even) {
  background-color: #fafafa;
}

.schedule-table tbody tr:nth-child(even):hover {
  background-color: #f0f0f0;
}

.schedule-table td:first-child {
  font-weight: 500;
  width: 25%;
  color: #333;
}

.schedule-table td:nth-child(2) {
  font-weight: 500;
  width: 75%;
  color: #2c3e50;
}

/* Mobile Schedule Table */
@media (max-width: 768px) {
  .schedule-table {
    font-size: 0.8rem;
  }

  .schedule-table th,
  .schedule-table td {
    padding: 8px 6px;
  }

  .schedule-table td:first-child {
    width: 30%;
  }

  .schedule-table td:nth-child(2) {
    width: 70%;
  }
}

/* Placeholder Slides Styling */
.slides-placeholder {
  color: #999;
  font-style: italic;
  font-size: 0.9em;
}
</style>

<!-- Table of Contents -->
<div class="floating-toc">
  <h4>Table of Contents</h4>
  <ul>
    <li><a href="#overview">Overview</a>
      <ul>
        <li><a href="#course-information">Course Information</a></li>
        <li><a href="#course-description">Course Description</a></li>
        <li><a href="#learning-goals">Learning Goals</a></li>
        <li><a href="#grading">Grading</a></li>
      </ul>
    </li>
    <li><a href="#schedule">Schedule</a></li>
    <li><a href="#project">Project</a></li>
    <li><a href="#presentations-and-discussions">Paper Reading</a></li>
    <li><a href="#logistics">Logistics</a>
      <ul>
        <li><a href="#time-management">Time Management</a></li>
        <li><a href="#attendance">Attendance</a></li>
        <li><a href="#late-work-and-absence-policy">Late Work Policy</a></li>
        <li><a href="#policy-on-the-use-of-generative-ai-tools">AI Tools Policy</a></li>
        <li><a href="#feedback-for-the-course">Feedback</a></li>
        <li><a href="#accommodations">Accommodations</a></li>
        <li><a href="#a-note-for-self-care">Self Care</a></li>
      </ul>
    </li>
  </ul>
</div>

<!-- TOC JavaScript -->
<script>
document.addEventListener('DOMContentLoaded', function() {
  const toc = document.querySelector('.floating-toc');
  const tocHeader = toc.querySelector('h4');

  function handleTocCollapse() {
    if (window.innerWidth <= 1200) {
      tocHeader.addEventListener('click', function() {
        toc.classList.toggle('collapsed');
      });
      if (window.innerWidth <= 768) {
        toc.classList.add('collapsed');
      }
    }
  }

  handleTocCollapse();
  window.addEventListener('resize', handleTocCollapse);
});
</script>

# SWE 233: Intelligent User Interfaces
**Fall 2025 • University of California, Irvine**

# Overview

## Course Information

**Instructor:** Daye Nam<br>
**Email:** daye.nam@uci.edu<br>
**Lecture:** 9:30 AM-10:50 AM PST, MW @ PCB 1200<br>
**Office Hours:** Monday 4:00 PM - 5:00 PM @ ISEB 2430<br>
**Course Credits:** 4 units

## Course Description

This course examines the design, implementation, and evaluation of intelligent user interfaces; interactive systems that use AI techniques to enhance usability, adapt to context, and support user goals. We will focus on applications in software engineering, including intelligent developer tools, AI-assisted programming environments, and data science workflows.

The course begins with fundamentals of user interface design and human-computer interaction, then explores user modeling, conversational interfaces, and agentic tools for various software engineering-related tasks and processes. We will discuss trade-offs among different approaches, design for diverse users, and study how to evaluate them.

You will critically analyze research papers from HCI, software engineering, and AI conferences (e.g., CHI, UIST, IUI, ICSE, FSE) and apply these insights in a quarter-long project. Through the project, you will design and prototype an intelligent interface, conduct a literature review, develop a study design, and present your work. The final deliverable will be a research paper draft (in the style of a conference submission) and an evaluation plan, ready to complete with results after the course.

## Learning Goals

By the end of this course, you will be able to:

- **Identify and analyze** real-world problems that can be addressed through intelligent user interfaces
- **Design end-to-end intelligent systems** with AI components, system architectures, and interface mockups
- **Evaluate solutions** through appropriate research methods, metrics, and validity considerations
- **Conduct research** including literature reviews and academic writing following conference standards
- **Understand human-AI collaboration** and design interfaces that balance automation with user control

<details>
<summary><strong>Topics Covered</strong></summary>
<ul>
<li>Foundations of Human-Computer Interaction and UI Design Principles</li>
<li>User Modeling and Personalization Techniques</li>
<li>Adaptive and Context-Aware Interfaces</li>
<li>Conversational AI and Natural Language Interfaces</li>
<li>Agentic Interfaces and Multi-Step Task Delegation</li>
<li>Multi-Modal Interfaces (Voice, Gesture, AR/VR)</li>
<li>Programming by Demonstration and Example-Based Systems</li>
<li>Research Methods for HCI (Surveys, Interviews, Qualitative Analysis)</li>
<li>Evaluation Methods for Intelligent UI (A/B Testing, Longitudinal Studies, Wizard of Oz)</li>
<li>IDEs and AI-Powered Programming Tools</li>
<li>Debugging and Search Interfaces</li>
<li>Data Science Workflows and Computational Notebooks</li>
<li>Trust, Transparency, and User Control in Intelligent Systems</li>
<li>Ethics and Inclusive Design in Intelligent Systems</li>
</ul>
</details>

## Grading

**Total: 100%**

- **80% Research Project and Assignments** ([view details](project/))
  - **5%** [Problem Identification](project/#problem-identification)
  - **25%** [Project Proposal](project/#project-proposal)
    - Report: 15%
    - [Presentation](project/#project-proposal-presentation): 10%
  - **15%** [Prototype Design](project/#prototype-design)
  - **35%** [Final Report](project/#final-report)
    - Report: 15%
    - [Presentation](project/#presentation): 10%
    - Holistic: 10%
- **10%** [Paper Presentation](#presentations-and-discussions)
- **10%** [In-Class Participation](#attendance)
- **[Optional] 10%** Prototype Implementation

**Submission Timing:** All assignments are due at 1 AM PST. I highly recommend submitting by midnight. Deadlines are set so you can complete work before the next class session.

# Schedule

<table class="schedule-table">
<thead>
<tr>
<th>Date</th>
<th>Topic</th>
</tr>
</thead>
<tbody>

<!-- Week 1 -->
<tr>
<td>Sep 29<br><small><em>In class: Intro survey</em></small></td>
<td>Introduction to Intelligent User Interfaces<br><a href="slides/Introduction.pdf">[slides]</a></td>
</tr>

<tr>
<td>Oct 1<br><small><em>Due: <a href="https://docs.google.com/forms/d/e/1FAIpQLScOuXUIm79mPFrKAyzuYRaEQzyBBwgv2fU7IH6yrLZkiknlWw/viewform?usp=header">Presentation Bidding</a></em></small></td>
<td>A Quick Tour of Human Computer Interaction / User Interface<br><a href="slides/HCI.pdf">[slides]</a></td>
</tr>

<!-- Week 2 -->
<tr>
<td>Oct 6</td>
<td>Overview of Research Methods<br><a href="slides/Methods.pdf">[slides]</a></td>
</tr>

<tr>
<td>Oct 8<br><small><em>Due: <a href="project/#problem-identification">Problem Identification</a></em></small></td>
<td>Designing Evaluation<br><a href="slides/Methods2.pdf">[slides]</a><br>
<small><em>
</em></small></td>
</tr>

<!-- Week 3 -->
<tr>
<td>Oct 13</td>
<td>Integrated Development Environment (IDE)<br>
<small><em>
• <a href="https://ieeexplore.ieee.org/document/6062113">Code bubbles: rethinking the user interface paradigm of integrated development environments</a><br>
• <a href="https://arxiv.org/pdf/2205.06537">Productivity Assessment of Neural Code Completion</a>
</em></small></td>
</tr>

<tr>
<td>Oct 15</td>
<td>Conversational UI I<br>
<small><em>
• <a href="https://dl.acm.org/doi/10.1145/3586030">Grounded Copilot: How Programmers Interact with Code-Generating Models</a><br>
• <a href="https://dl.acm.org/doi/10.1145/3544548.3581388">Why Jonny Can't Prompt: How Non-AI Experts Try (and Fail) to Design LLM Prompts</a><br>
</em></small></td>
</tr>

<!-- Week 4 -->
<tr>
<td>Oct 20</td>
<td>Conversational UI II<br>
<small><em>
• <a href="https://dl.acm.org/doi/10.1145/3180155.3180238">Context-aware conversational developer assistants</a><br>
• <a href="https://dl.acm.org/doi/full/10.1145/3706598.3714002">Need Help? Designing Proactive AI Assistants for Programming</a><br>
</em></small></td>
</tr>


<tr>
<td>Oct 22</td>
<td>Agents<br>
<small><em>
• <a href="https://arxiv.org/pdf/2507.22358?">Magentic-UI: Towards Human-in-the-loop Agentic Systems</a><br>
• <a href="https://dl.acm.org/doi/pdf/10.1145/3586183.3606763">Generative Agents: Interactive Simulacra of Human Behavior</a><br>
</em></small></td>
</tr>

<!-- Week 5 -->
<tr>
<td>Oct 27<br><small><em>Due: <a href="project/#project-proposal-presentation">Presentation slides</a></em></small></td>
<td>Project Proposal & Feedback 1</td>
</tr>


<tr>
<td>Oct 29</td>
<td>Project Proposal & Feedback 2</td>
</tr>


<!-- Week 6 -->
<tr>
<td>Nov 3<br><small><em>Due: <a href="project/#project-proposal">Project Proposal</a></em></small></td>
<td>User Modeling & Personalization<br>
<small><em>
• <a href="https://dl.acm.org/doi/pdf/10.1145/3746059.3747722">Creating General User Models from Computer Use</a><br>
• <a href="https://dl.acm.org/doi/pdf/10.1145/581339.581402">Supporting Reuse by Delivering Task-Relevant and Personalized Information</a><br>
</em></small></td>
</tr>

<tr>
<td>Nov 5</td>
<td>End Users I<br>
<small><em>
• <a href="https://dl.acm.org/doi/10.1145/3654777.3676368">SQLucid: Grounding Natural Language Database Queries with Interactive Explanations</a><br>
• <a href="https://dl.acm.org/doi/10.1145/3472749.3474773">Situated Live Programming for Human-Robot Collaboration</a>
</em></small></td>
</tr>

<!-- Week 7 -->
<tr>
<td>Nov 10</td>
<td>End Users II<br>
<small><em>
• <a href="https://dl.acm.org/doi/pdf/10.1145/3654777.3676391">ProgramAlly: Creating Custom Visual Access Programs via Multi-Modal End-User Programming</a><br>
• <a href="https://dl.acm.org/doi/10.1145/3379337.3415869">Small-Step Live Programming by Example</a>
</em></small></td>
</tr>

<tr>
<td>Nov 12</td>
<td>UI<br>
<small><em>
• <a href="https://dl.acm.org/doi/abs/10.1145/3397481.3450671">Auto-Icon: An Automated Code Generation Tool for Icon Designs Assisting in UI Development</a><br>
• <a href="https://dl.acm.org/doi/pdf/10.1145/1622176.1622213">Sikuli: Using GUI Screenshots for Search and Automation</a>
</em></small></td>
</tr>

<!-- Week 8 -->
<tr>
<td>Nov 17<br><small><em>Due: <a href="project/#prototype-design">Prototype Design</a></em></small></td>
<td>Collaboration<br>
<small><em>
• <a href="https://dl.acm.org/doi/abs/10.1145/2076354.2076393">Code space: touch + air gesture hybrid interactions for supporting developer meetings</a><br>
• <a href="https://dl.acm.org/doi/10.1145/1753326.1753478">What would other programmers do: suggesting solutions to error messages</a>
</em></small></td>
</tr>

<tr>
<td>Nov 19</td>
<td>Debugging & Testing<br>
<small><em>
• <a href="https://dl.acm.org/doi/10.1145/1368088.1368130">Debugging reinvented: asking and answering why and why not questions about program behavior</a><br>
• <a href="https://dl.acm.org/doi/pdf/10.1145/3611643.3616327">NaNofuzz: A Usable Tool for Automatic Test Generation</a>
</em></small></td>
</tr>

<!-- Week 9 -->
<tr>
<td>Nov 24</td>
<td>Wrap-up & Course Review<br><span class="slides-placeholder">[slides]</span></td>
</tr>

<tr>
<td>Nov 26</td>
<td>Thanksgiving - No Class</td>
</tr>

<!-- Week 10 -->
<tr>
<td>Dec 1<br><small><em>Due: <a href="project/#presentation">Presentation slides</a></em></small></td>
<td>Final presentation</td>
</tr>

<tr>
<td>Dec 3</td>
<td>Final presentation</td>
</tr>

<!-- Finals Week -->
<tr>
<td>Dec 10<br><small><em>Due: <a href="project/#final-report">Final Report</a><br>Due: <a href="project/#optional-prototype-implementation">[Optional] Prototype Implementation</a></em></small></td>
<td>No final exam (substituted by final presentation) - Final assignments due</td>
</tr>

</tbody>
</table>

*Schedule and content are subject to change.*

# Project

Throughout the course, you will work on a quarter-long project where you design and prototype an intelligent user interface. This project will give you hands-on experience with the concepts covered in class and result in a research paper draft ready for conference submission.

**Key milestones include:**
- **Problem Identification** (Oct 8) - Identify and scope a problem for intelligent UI solution
- **Project Proposal** (Nov 3) - Literature review and proposed solution
- **Proposal Presentation** (Oct 27 & 29) - Present proposal for feedback
- **Prototype Design** (Nov 17) - System architecture and interface design
- **Final Report** (Dec 10) - Complete evaluation methodology
- **Final Presentation** (Dec 1 & 3) - Showcase complete project

**[→ View Complete Project Requirements](project/)**

# Presentations and Discussions

For the second half of the course, we will read and discuss systems with intelligent user interfaces within the software engineering domain.

- **Paper Presentations**: Each student will present at least two papers over the quarter. Each presentation should be 10-15 minutes. As presenters, you will:
  - Summarize main research questions, proposed methods, and key contributions
  - Focus on the used methodologies; if not covered in the previous classes, please delve deeper into the details
  - Prepare 3 discussion questions

- **Slide Upload Deadline**: Slides must be uploaded by 1 am on the day you're presenting the paper
  - e.g., if you're presenting a paper on Oct 8, you should finalize your slides by October 8, 1 am
  - Upload your slides to the #presentation-slides channel on Slack

- **Reading Requirement**: You are expected to read every paper presented during the course before the class.

- **Paper Selection**: You will bid for a paper you want to present in the beginning of the quarter. You are encouraged to bid for papers that are close to your project topic.

# Logistics

## Time Management

This is a 4-unit course, which is expected to be approximately 12 hours of work per week when averaged over the whole quarter. In general, 3 hours per week will be spent in class, and 9 hours will be spent on readings and projects.

## Attendance

You are expected to attend classes in person. Classes will not be recorded or available through Zoom, except when noted.

Each class will have in-class activities and submissions that count toward your final grade. We do not take formal attendance, but your participation grade reflects your presence. Your lowest 2 participation scores will be dropped, giving you 2 no-questions-asked missed classes without grade impact.

Beyond the 2 drops, exceptions are only made for extraordinary circumstances and may involve your academic advisor. Contact me immediately to find solutions together.

## Late Work and Absence Policy

Late submission for assignments or projects will be penalized with a 10% or one letter grade deduction for every 24 hours they are late. For late submissions, the instructor cannot guarantee timely feedback.

Requests for extensions can be made only in extraordinary circumstances (e.g., family or medical emergency) and may involve your academic advisor.

## Policy on the Use of Generative AI Tools

You are encouraged to use generative AI-powered developer tools, such as Cursor, for building prototype tools.

For writing, you may use generative AI tools such as ChatGPT or Gemini, but you are responsible for what you submit. You are liable for factually inaccurate answers or citing the wrong references. This is a research-focused graduate-level course, and the submitted report will be graded according to the standard of academic research papers.

## Feedback for the Course

Please feel free to give the instructor feedback on which topics to cover, how much time you spend for the course, or anything else. There will be midterm and final course evaluations to help improve the course, but any form of feedback is welcome at any time.

## Accommodations

If you wish to request an accommodation due to a documented disability, please contact [https://dsc.uci.edu/](https://dsc.uci.edu/).

## A Note for Self Care

Please take care of yourself.

If you or anyone you know experience any academic stress, mental health concerns, or difficult life events, we strongly encourage you to seek support.

- UCIPD (Non-Emergency Line): (949) 824-5223
- UCI Counseling Center: (949) 824-6457
- Center for Student Wellness & Health Promotion: (949) 824-9355
- Student Health Center: (949) 824-5301

---