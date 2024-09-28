---
title: "ISM Controls"
description: "OSCAL and the ACSC Information Security Manual"
lead: "ISM for automated security trace and validation."
draft: false
images: []
weight: 5
toc: true
---

## Enabling Automated Security Trace and Validation

The following links are the top level ISM controls sets as input to automated security control allocation and automation.

- [ISM in Security Group Context](https://ism.mentormind.com.au/context)
- [All the ISM Controls](https://ism.mentormind.com.au/control/index)
- [Essential Eight Controls](https://ism.mentormind.com.au/essential-eight)

## Overview
To obtain an Authority to Operate (ATO), systems must demonstrate reduced operational risks to an acceptable level. This is commonly achieved through the Australian Cyber Security Centre's ([ACSC](https://cyber.gov.au/)) Information Security Manual ([ISM](https://www.cyber.gov.au/resources-business-and-government/essential-cyber-security/ism)). However, the traditional approach—using Excel spreadsheets and Word documents—complicates reliable control allocation and testing, making it challenging to maintain a verifiable security posture over time.

To address this, the U.S. standards body NIST has developed the Open Security Controls Assessment Language ([OSCAL](https://pages.nist.gov/OSCAL/)), which enables automated control allocation and testing. The ACSC has adapted this by publishing the ISM with an OSCAL schema.

Despite this advancement, additional tools are necessary for practical application. MentorMind has developed ISM OSCAL parsers in [Rust](https://www.rust-lang.org), complemented by a REST API for easy access.

Thus, the following `curl` request:

```bash
https://raw.githubusercontent.com/stem-teacher/ism.github.io/refs/heads/main/content/control/ism-0047.md
```

returns the following result.

```markdown
### Control: ism-0047; Revision: 4; Updated: May-19; Applicability: ALL; Essential Eight: N/A
<p>Organisational-level security documentation is approved by the Chief Information Security Officer while system-specific security documentation is approved by the system’s authorising officer.</p>
```

Similarly, the following curl requests produce all the controls as a single document, as well as the different security control groups:
```bash
curl https://ism.mentormind.com.au/control
curl https://ism.mentormind.com.au/control/all
curl https://ism.mentormind.com.au/group
```

## Take me to the controls

[ISM in Group Context](https://ism.mentormind.com.au/context) [All ISM Controls](https://ism.mentormind.com.au/control/index) [Essential Eight Controls](/essential-eight)
