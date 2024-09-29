---
title: "SRS Process Overview"
description: "Overview of Specification Process"
draft: false
images: []
weight: 2
toc: true
---
## Skill Pre-requisite

[GitHub Skills](https://skills.github.com)

Given the structure of your project, the goal is to create a well-organized **Requirements Workbook** within the `/workbooks/specification` directory in the GitHub repository. We will also add a **Training Workbook** for student guidance.

### 1. Setting Up the Requirements Workbook
Login to the courses github repo.
Then either clone the https://github.com/stem-teacher/brokenhill-h.github.io.git or simply create a new branch (e.g. srs-update).

Access the workbook is simplest using associated codespaces onn the branch.

#### Directory Structure for Requirements
The full path for the requirements would be under:
```
/content/workbooks/specification/functional
/content/workbooks/specification/non-functional
/content/workbooks/specification/security
/content/workbooks/specification/system
```

### 2. Requirements Template
Create a Markdown file named `REQ-TEMPLATE.md` inside each of the specification directories (e.g., `/workbooks/specification/functional/REQ-TEMPLATE.md`). This template will provide a standard format for writing requirements.

#### **`REQ-TEMPLATE.md`**
```markdown
---
id: "REQ-XXX"
title: "Requirement Title"
description: "Detailed description of the requirement."
type: "Functional/Non-Functional/Security/System"
priority: "High/Medium/Low"
status: "Planned/In Progress/Implemented/Tested"
author: "Your Name"
creation_date: "YYYY-MM-DD"
last_updated: "YYYY-MM-DD"
rationale: "Explanation of why this requirement is necessary."
dependencies: [List of related requirement IDs]
acceptance_criteria:
  - "Condition 1 that must be met."
  - "Condition 2 that must be met."
verification_method: "Testing/Inspection/Analysis"
references:
  - "Relevant documents, links, or sources."
---

# Requirement Title
Provide a detailed description of the requirement here...

## Rationale
Explanation of why this requirement is necessary.

## Acceptance Criteria
- List the specific conditions that must be fulfilled for this requirement to be considered complete.

## Dependencies
- List other related requirement IDs.
```

- **Instructions:** Whenever a new requirement is created, copy this template, rename it (e.g., `REQ-001.md`), and fill in the details.

### 3. Requirements Example

Here’s an example of a functional requirement using the template, to be placed in `./workbooks/specification/functional/REQ-001.md`:

#### **`REQ-001.md`**
```markdown
---
id: "REQ-001"
title: "User Authentication"
description: "The system must allow users to authenticate using a username and password."
type: "Functional"
priority: "High"
status: "Planned"
author: "John Doe"
creation_date: "2024-09-28"
last_updated: "2024-09-28"
rationale: "To ensure only authorized users can access the system, enhancing security."
dependencies: []
acceptance_criteria:
  - "Users can log in with valid credentials."
  - "Invalid login attempts are logged and rejected."
verification_method: "Testing"
references:
  - "School Event Management System Overview"
  - "https://example.com/authentication-guidelines"
---

# User Authentication
The system must allow users to authenticate using a username and password.

## Rationale
To ensure only authorized users can access the system, enhancing security.

## Acceptance Criteria
- Users can log in with valid credentials.
- Invalid login attempts are logged and rejected.

## Dependencies
None.
```

### 4. Requirements Workbook Index

Create or edit a `README.md` file inside the `./workbooks/specification/` directory to serve as an index for all requirements:

#### **`/workbooks/specification/README.md`**
```markdown
# Requirements Workbook

This workbook contains all the system requirements for the School Event Management System (SEMS). The requirements are categorized into functional, non-functional, security, and system requirements.

## List of Requirements

### Functional Requirements
- [REQ-001: User Authentication](functional/REQ-001.md)

### Non-Functional Requirements
- [REQ-TEMPLATE: Non-Functional Requirement Template](non-functional/REQ-TEMPLATE.md)

### Security Requirements
- [REQ-TEMPLATE: Security Requirement Template](security/REQ-TEMPLATE.md)

### System Requirements
- [REQ-TEMPLATE: System Requirement Template](system/REQ-TEMPLATE.md)
```

### 5. Creating the Training Workbook

To support students, add a **Training Workbook** in the root `/workbooks` directory. This will provide guidance on how to use the templates and create new requirements.

#### Directory Path
```
./workbooks/training
```

#### **`/workbooks/training/README.md`**
```markdown
# Training Workbook

Welcome to the Training Workbook for the Software Engineering Course. This workbook provides guidelines and instructions for creating software requirement specifications (SRS) and using the version control system (Git) to manage these specifications.

## How to Create a New Requirement

1. Navigate to the relevant category in the `./workbooks/specification/` directory (functional, non-functional, security, or system).
2. Copy the template file (`REQ-TEMPLATE.md`) and rename it (e.g., `REQ-002.md`).
3. Fill in the required fields in the front matter and the main body of the document.

### Example Workflow

1. Copy the [`req-template.md`](/process/specification/req-template):
   ```bash
   cp ./workbooks/specification/functional/REQ-TEMPLATE.md ./workbooks/specification/functional/REQ-002.md
   ```

2. Open the newly created `REQ-002.md` file in your text editor and complete the fields.

3. Save the file, add it to Git, commit, and push to the repository:
   ```bash
   git add ./workbooks/specification/functional/REQ-002.md
   git commit -m "Add new functional requirement: REQ-002"
   git push origin main
   ```

## Additional Resources

- [Git Basics](https://git-scm.com/docs/gittutorial) - Learn how to use Git for version control.
- [Markdown Guide](https://www.markdownguide.org/) - Learn Markdown syntax for creating structured documents.
```

### Summary

- **Templates**: Create `REQ-TEMPLATE.md` in each subdirectory under `./workbooks/specification` for different requirement types (functional, non-functional, security, system).
- **Examples**: Create example requirement files using the templates, such as `REQ-001.md`.
- **Index**: Use a `README.md` file in `./workbooks/specification` to link all requirements.
- **Training Workbook**: Place a `README.md` file in `./workbooks/training` to guide students through the process of creating requirements.

This structure will help your team and students systematically create, manage, and track software requirements, all within the organized workbook system on the GitHub-hosted Hugo site.
