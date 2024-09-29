---
title: "System Requirement Template"
draft: false
images: []
weight: 2
toc: true
---

The following markdown is an example

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
rationale: "Explanation of why this requirement is necessary."
dependencies: [List of related requirement IDs]
acceptance_criteria:
  - "Condition 1 that must be met."
  - "Condition 2 that must be met."
verification_method: "Testing/Inspection/Analysis"
references:
  - "Relevant documents, links, or sources."

# Traceability fields
implementation_ref: "/implementation/IMPL-REQ-001"
test_ref: "/tests/TEST-REQ-001"
status_progress:
  planned: "2024-09-28"
  implemented: "2024-10-05"
   tested: "2024-10-10"
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
