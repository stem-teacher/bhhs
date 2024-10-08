---
title: "Lesson Plan: Introduction to System Requirements Specification (SRS)"
draft: false
images: []
weight: 5
toc: true
---
## Overview
**Name:** Philip Haynes **Date:** 28/09/2024
**School:** Broken Hill High School

**Unit of Work:** Programming Fundamentals
**Lesson Topic:** System Requirements Specification (SRS) **Lesson Length:** 60 mins

**Lesson Begins / End:** 9:05:10:05 **Class Size:** 20

## Syllabus Outcomes
1. **SE-11-01**: Describes methods used to plan, develop and engineer software solutions
Introduce Students to the use of SRS in the context of a formal software engineering.

1. **SE-11-02**: explains how structural elements are used to develop programming code
Demonstrate how requirements tracde to implementation.

1. **SE-11-03**: Describes how current hardware, software and emerging technologies influence the  development of software engineering solutions
Demonstrate a contemporary software engineering environment.

1. **SE-11-04**: applies safe and secure practices to collect, use and store data
Continued demonstration to students to the use of [github](https://github.com/stem-teacher/brokenhill-h.github.io)

1. **SE-11-06**: applies tools and resources to design, develop, manage and evaluate software
Introduce students to key software technologies to complete software engineering.

1. **SE-11-07**: Implements safe and secure programming solutions
Introduce students to the [ISM Security Controls](https://ism.mentormind.com.au/control/index)

## Lesson Outcomes
- Define what an SRS is and explain its importance in software engineering.
- Identify and describe different types of software requirements.
- Introduce students to the characteristics of a good SRS.
- Explain how requirements fit into the software engineering lifecycle.
- Demonstrate how to write, document, and manage requirements using GitHub and Hugo.
- Introduce tooling

## Assessment (Diagnostic/Formative/Summative)
This is an inital subject with a lot of material for students to understand.
The goal is to ensure students can access and explore the information, then complete the initial task of creating and submitting a requirement.
1. Formative assessment - ensure students can access material and make progress.
1. Summative: Successfully created a requirement to review.

## The Key/Foundational Ideas Addressed in This Lesson Are
1. SRS in the context of a formal software engineering process.

## General Capabilities
The class consists of main stream Y11 students. Bright and enthusasistic, but otherwise new to software engineering.

## Equipment/Resources
- [Presentation pack](/workbooks/training/srs/bhhs-srs.pptx)
- Students have access to a computer and are logged into GitHub.
- Prepared [software engineering site](https://brokenhill-h.polemos.ai/)
- [**GitHub**](https://github.com/stem-teacher/brokenhill-h.github.io): A version control platform where students will store their SRS documents.
- **Templates:** Refer to the [SRS template](/process/specification/req-template/) provided on the engineering site for structured requirement specification template.

## Context of the Lesson/Students' Prior Learning:
The students have been introduced to git and github, but otherwise new to the subject.

## Lesson Plan

### Stages/Timing

### 0-5 Minutes: Introduction

- **Objective:** Introduce the concept of System Requirements Specification (SRS).
- **Activities:**
  - Welcome students and briefly introduce the day's topic.
  - Pose an opening question: _“What do you think is the first step in building software?”_
  - Explain that creating a **System Requirements Specification (SRS)** is one of the first and most critical steps.

### 5-15 Minutes: What is an SRS?

- **Objective:** Define what an SRS is and discuss its context in software engineering.
- **Content:**
  - Present the definition of an SRS:
    - _“A Software Requirements Specification (SRS) forms a contractual basis between a customer and the software engineering team, detailing what the system should do.”_
  - Show a **Context Diagram** from SWEBOK to illustrate the role of SRS in software development.
  - Discuss the **context** of using an SRS in different scenarios, from large organizations building software for clients to individuals instructing an AI.
- **Questions:**
  - _“Why do you think having a clear set of requirements is important when building software?”_

### 15-25 Minutes: Understanding Software Requirements

- **Objective:** Explain what software requirements are and introduce various types.
- **Content:**
  - Define a software requirement and differentiate between:
    - **Functional Requirements:** What the system should do.
    - **Non-Functional Requirements:** How the system performs.
    - **Security Requirements:** How the system protects data and interactions.
  - **Examples:**
    - Functional: _"The system must allow students to register for events online."_
    - Non-Functional: _"The system should load event details within 2 seconds."_
    - Security: _"User passwords must be encrypted using AES-256 encryption."_
- **Activity:**
  - Ask students to write down one simple functional requirement for a school event management system.

### 25-35 Minutes: Gathering Requirements & Standards

- **Objective:** Discuss where requirements come from and introduce software standards.
- **Content:**
  - Explain **Requirements Sources**:
    - Stakeholders (e.g., users, clients).
    - Business needs and goals.
    - Regulations and standards.
  - Introduce the concept of **Standards** in software engineering.
    - Describe what standards are and their role in ensuring software quality.
    - Introduce **ACSC ISM (Australian Cyber Security Centre's Information Security Manual)** as a key security standard.
- **Activity:**
  - Display the class [Software Engineering site](https://brokenhill-h.polemos.ai/) and showcase a section on software standards.

### 35-45 Minutes: Characteristics of a Good SRS

- **Objective:** Highlight the key characteristics of a well-defined SRS.
- **Content:**
  - Discuss the **8 characteristics of a good SRS**:
    - **Correct:** Accurately describes the intended functionality.
    - **Unambiguous:** Clear and interpreted in only one way.
    - **Complete:** Covers all necessary aspects.
    - **Consistent:** No conflicting requirements.
    - **Ranked:** Prioritized by importance or stability.
    - **Verifiable:** Can be tested or inspected.
    - **Modifiable:** Easy to update and maintain.
    - **Traceable:** Each requirement can be tracked throughout the project.
  - Emphasize the use of **"shall"** statements for mandatory requirements.
- **Activity:**
  - Have students refine the functional requirement they wrote earlier to make it unambiguous and verifiable.


### 45-50 Minutes: Traceability & What to Avoid in SRS

- **Objective:** Explain traceability and what not to include in an SRS.
- **Content:**
  - Define **Traceability**: The ability to track a requirement through its implementation and testing.
  - Introduce traceability elements: ID, Type, Description, Importance.
  - **What to Avoid:**
    - Do not include design details.
    - Avoid vague language.
    - Keep project management aspects separate.
- **Questions:**
  - _“Why is it important to track each requirement?”_
- **Activity:**
  - Show a sample SRS statement on the Software Engineering site that includes traceability elements.


### 50-60 Minutes: How Requirements Fit into the Software Engineering Lifecycle

- **Objective:** Place SRS in the context of the overall software engineering process.
- **Content:**
  - Explain how SRS fits into different phases:
    - **Planning:** Defines scope and project goals.
    - **Construction:** Guides developers on what to build.
    - **Testing:** Used to verify that the final product meets the requirements.
- **Wrap-Up:**
  - Summarize the importance of a well-defined SRS.
  - Emphasise that good requirements form the backbone of successful software projects.

---

### Homework / Follow-Up Activity

- **Activity:** Ask students to create three requirements (one functional, one non-functional, one security) for a simple system they choose. They should:
  - Write them using the SRS template in Markdown.
  - Save them in their GitHub repository.
  - Commit the link with the teacher for feedback.


## Reflection

1. What assumptions did I make when I planned this lesson?


1. Were these assumptions correct/incorrect?

1. What impact did these assumptions have on the effectiveness of the lesson?

1. How could I do things differently next time?

## Evaluation

| Evaluation                                                      | Strongly Agree | Agree | Neutral | Disagree |
| --------------------------------------------------------------- | -------------- | ----- | ------- | -------- |
| Pre-planning Proved Effective                                   | [ ]            | [ ]   | [ ]      | [ ]      |
| Teaching & Learning Strategies Were Effectively Implemented     | [ ]            | [ ]   | [ ]      | [ ]      |
| I Was Able to Generate a Sense of Purpose:                      | [ ]            | [ ]   | [ ]      | [ ]      |
| A High Level of Student Participation Was Achieved:             | [ ]            | [ ]   | [ ]      | [ ]      |
| My Questioning Was Clear, Concise and Logically Sequenced:      | [ ]            | [ ]   | [ ]      | [ ]      |
| Pupils Were Interested and Self Disciplined:                    | [ ]            | [ ]   | [ ]      | [ ]      |
| The Resources Used Were Appropriately Graded:                   | [ ]            | [ ]   | [ ]      | [ ]      |
| Instructions Were Clear and Easily Understood by Students:      | [ ]            | [ ]   | [ ]      | [ ]      |
| I Recognised and Catered for Individual Differences:            | [ ]            | [ ]   | [ ]      | [ ]      |
| I Established and Maintained an Effective Learning Environment: | [ ]            | [ ]   | [ ]      | [ ]      |

### What Were the Most Effective Elements of the Lesson?


### What Were the Least Effective Elements of the Lesson?

### If I Was to Repeat the Lesson, What Would I Change? What Could I Improve?
