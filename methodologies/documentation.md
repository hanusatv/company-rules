---
methodology_id: documentation
title: Documentation
priority: high
tags: [standards, documentation, confluence, atlassian]
---

# Documentation Standard

## 1. When Documentation is Required

Documentation **MUST** be created when:

- A feature changes or extends standard Business Central functionality.
- A feature introduces new business logic.
- A feature modifies system behavior.
- A feature affects integrations or external systems.

Documentation is **NOT REQUIRED** when:

- Only captions are changed.
- A simple field is added and its purpose is obvious.
- Minor UI adjustments are made without logic changes.
- Changes are purely cosmetic and self-explanatory.

If in doubt → **Create documentation.**

---

## 2. Where Documentation is Stored

- All documentation is created in **Atlassian Confluence**.
- Each customer has their own dedicated wiki space.
- Documentation must be created in the correct customer space.

---

## 3. Jira Linking Requirement

Each documentation page **MUST**:

- Contain a hyperlink to the corresponding Atlassian Jira ticket.
- Use the full Jira URL (not just the ticket ID).

---

## 4. Complex Features

If a feature is complex, extended documentation must be created.

A feature is considered complex if it:

- Contains multiple workflows.
- Includes new business processes.
- Requires explanation of technical logic.
- Involves integrations.
- Requires diagrams or process explanations.

In such cases:

- Create a **subpage** in Confluence.
- The main page must link to the subpage.

---

# Confluence Documentation Template

## Main Page Template

**Title:** Description of the Task  
**Jira:** Hyperlink to the Atlassian Jira Ticket  
**Specification:** Hyperlink to specification document (optional)  
**System Documentation:** Hyperlink to detailed subpage (optional)

---

## Subpage Template (for Complex Features)

The subpage should include:

- Purpose
- Functional description
- Technical description
- Data model changes (if any)
- Integration details (if any)
- Edge cases / limitations
- Diagrams (if relevant)
- Change impact

---

# Naming Convention

Main page title format:

`DOK: [Feature Name]`

Example:

`DOK: Sales Discount Approval Workflow`
