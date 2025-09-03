---
layout: page
title: "SWE 233 - Project"
permalink: /teaching/swe233-fall2025/project/
---

<style>
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
</style>

# SWE 233 Project: Intelligent User Interface Design

[← Back to Main Syllabus](/teaching/swe233-fall2025/)

<div class="floating-toc">
  <h4>Project Navigation</h4>
  <ul>
    <li><a href="#project-guidelines">Project Guidelines</a></li>
    <li><a href="#project-timeline">Project Timeline</a>
      <ul>
        <li><a href="#problem-identification">Problem Identification</a></li>
        <li><a href="#project-proposal">Project Proposal</a></li>
        <li><a href="#project-proposal-presentation">Project Proposal Presentation</a></li>
        <li><a href="#prototype-design">Prototype Design</a></li>
        <li><a href="#final-report">Final Report</a></li>
        <li><a href="#presentation">Presentation</a></li>
        <li><a href="#optional-prototype-implementation">[Optional] Prototype Implementation</a></li>
      </ul>
    </li>
  </ul>
</div>

## Project Guidelines

Throughout the course, you will work on a quarter-long project where you design and prototype an intelligent user interface. This project will give you hands-on experience with the concepts covered in class and result in a research paper draft ready for conference submission.

**Key Requirements:**

- **Open-ended and creative**: Projects are open-ended and you are welcome to be creative. I highly encourage you to choose an idea that is relevant to Software Engineering (this is SWE 233!) and the topics in the schedule might be a good starting point. If you are confident that you have enough background knowledge and expertise to work on a project in other topics, you can but please discuss with the instructor.

- **Intelligent component required**: Your project should have an "intelligent" component that leverages AI techniques to enhance the user interface or user experience.

- **User interface requirement**: Your project should have some user interface component that users can interact with.

- **Feasible scope**: You should be able to build the prototype if you are given 3-4 additional weeks (you won't be required to build the system 100% during this course, but the scope should be realistic for implementation).

## Project Timeline

**Note**: All project deliverables should be submitted to Canvas by the specified deadlines.

**Important - Iterative Project Structure**: Each written deliverable builds upon previous submissions to create a complete conference paper by the end of the quarter (excluding results section).

- **Intermediate Deliverables**: You will be graded only on newly added content for each submission (Problem Identification → Project Proposal → Prototype Design).
- **Revisions Encouraged**: You are strongly encouraged to revise and improve previously submitted sections based on feedback and new insights.
- **Final Report**: The entire paper will be evaluated holistically, including all previous sections plus the new evaluation methodology section.

### Problem Identification
**Due: October 8, 1 AM PST**  

For the problem identification, you'll need to identify a problem that may be addressed or mitigated by intelligent support. You don't need to have a complete solution yet—focus on identifying a well-scoped problem.

**Requirements:**

- **Problem Definition**: Clearly describe the problem and its context, explaining why it is important to address.

- **Target Users**: Identify who would be the main users affected by this problem and who would benefit from a solution.

- **Intelligent Solutions**: Outline some potential intelligent solutions you envision that could address this problem.

**Deliverable**: Submit a short abstract (300 words) that covers all the requirements above.

### Project Proposal
**Due: October 27, 1 AM PST**  

Building on your problem identification, you will now develop a comprehensive project proposal that includes a thorough literature review and your proposed solution.

**Requirements:**

- **Literature Review**: Conduct a comprehensive literature review of previous works that aim to address similar problems. The literature review should include at least 10 references and should identify gaps in existing solutions, specifying what is missing or inadequate in current approaches.

- **Proposed Solution**: Develop a potential solution that involves an intelligent component such as a recommender system, LLM, AI-powered features, or other intelligent technologies. You must explain how your solution differs from and improves upon existing approaches identified in your literature review.

- **Academic Writing**: The report should be written in the style of introduction and related works sections of top-tier conference papers (e.g., ICSE, CHI). This means clear problem motivation, systematic literature review, and well-articulated contributions.

**Deliverable**: Submit a 4-6 page report (excluding references) that follows academic conference paper format.

**Examples:**
- Sections Introduction and Background and Related Work in Li, T.J.J. et al. [PUMICE: A Multi-Modal Agent that Learns Concepts and Conditionals from Natural Language and Demonstrations](https://toby.li/files/Li_Pumice_UIST19.pdf).

### Project Proposal Presentation
**Dates: October 20 & October 22**

Students will present their project proposals to the class for feedback and discussion before finalizing their prototype designs.

**Requirements:**

- **Presentation Length**: 8-10 minutes per presentation with 4-5 minutes for questions and feedback.

- **Content Coverage**: Your presentation should cover your problem identification, literature review findings, and proposed intelligent solution. Emphasize the gaps you identified in existing work and how your solution addresses them.

- **Literature Review**: Highlight key papers from your literature review and clearly articulate the research gap your project will address.

- **Feedback Integration**: Be prepared to receive and discuss feedback that will help refine your approach before the prototype design phase.

**Deliverable**: Students must submit presentation slides to Canvas by the deadline (1 AM PST), but are free to update slides for the live presentation. Live presentation with supporting slides. The order of presentations will be randomly decided. This presentation serves as preparation for your prototype design submission.

### Prototype Design
**Due: November 17, 1 AM PST**  

Now, let's design a solution that supports end-to-end scenarios. You don't need to build the system but should design the system and interface comprehensively.

**Requirements:**

- **System Design**: The deliverable should be written like the system description section in a CHI/UIST paper that describes the new system. Include a system architecture figure that shows the use case pipeline with a concrete example demonstrating how users would interact with your system. The caption should describe the system architecture graph and explain the flow of information through your system.

- **Interface Design**: Include a design of the user interface. You don't need to build a working system—this can be mockups, wireframes, or manually created interface images that clearly show how users would interact with your intelligent system.

- **Realistic Scope**: You should scope the design so that the prototype could realistically be built within a month if you were given dedicated time to implement it.

- **Technical Implementation Plan**: Include details about what programming languages, frameworks, and libraries you plan to use for implementation. Justify your technology choices based on your system requirements.

**Deliverable**: Submit a 4-6 page design document (excluding references) that includes system architecture diagrams, interface mockups, and technical implementation details.

**Examples:**
- Section 4 (and Figure 2) in Liu et al. ["What It Wants Me To Say": Bridging the Abstraction Gap Between End-User Programmers and Code-Generating Large Language Models](https://arxiv.org/pdf/2304.06597).

### Final Report
**Due: December 10, 1 AM PST**  

For your final report, you should develop a comprehensive research plan that demonstrates how you would evaluate your proposed solution.

**Requirements:**

- **Research Questions**: Formulate specific, testable research questions that address whether your solution can adequately solve the problem you identified at the beginning of the project.

- **Evaluation Plan**: Choose appropriate research methods to test your solution's effectiveness. Depending on your chosen method, you may need to consider:
  - Evaluation metrics (quantitative and/or qualitative)
  - Participant recruiting and filtering plans
  - Study design and procedures
  - Data collection and analysis methods

- **Realistic Scope**: The evaluation plan should be realistic for completion within one month when you have a working prototype. For example, do not propose to test with 10,000 developers—consider what is actually feasible given time and resource constraints.

- **Threats to Validity**: Include a thorough discussion of potential threats to validity and limitations of your proposed evaluation approach. Address internal, external, construct, and conclusion validity concerns.

**Deliverable**: Submit a 6-8 page research plan (excluding references) that includes research questions, detailed evaluation methodology, and validity considerations.

**Examples:**
- Any relevant paper we read during the quarter.

### Presentation
**Dates: December 1 & December 3**

Students will present their final projects to the class, showcasing their intelligent user interface solutions and research plans.

**Requirements:**

- **Presentation Length**: 10-12 minutes per presentation with 3-4 minutes for questions and discussion.

- **Content Coverage**: Your presentation should cover your problem identification, proposed solution, system design, and evaluation plan. Focus on demonstrating how your intelligent component addresses the identified problem.

- **Visual Materials**: Include slides that show your system architecture, interface mockups, and key findings from your literature review. Visual demonstrations or prototypes are encouraged if available.

- **Audience Engagement**: Prepare to answer questions about your design choices, technical implementation, and evaluation methodology.

**Deliverable**: Students must submit presentation slides to Canvas by the deadline (1 AM PST), but are free to update slides for the live presentation. Live presentation with supporting slides. The order of presentations will be randomly decided. No additional written submission required for the presentation component.

### [Optional] Prototype Implementation
**No specific deadline - ongoing throughout quarter**

For students who want to go beyond design and actually implement their intelligent user interface prototype, this optional component provides additional learning opportunities and extra credit.

**Requirements:**

- **Working Prototype**: Implement a functional version of your designed system that demonstrates the core intelligent features you proposed.

- **Technology Stack**: Use the programming languages, frameworks, and libraries you specified in your prototype design document.

- **Core Features**: Focus on implementing the most essential intelligent components rather than a fully polished system.

- **Documentation**: Provide setup instructions, usage examples, and a brief reflection on implementation challenges and learnings.

**Deliverable**: Submit working code (via GitHub repository or similar), demo video (3-5 minutes), and implementation documentation. This can be submitted anytime before the final presentation dates.

**Grading**: This optional component can contribute up to 10% additional credit to your final course grade.

---

[← Back to Main Syllabus](/teaching/swe233-fall2025/) | [View Schedule](/teaching/swe233-fall2025/schedule/)