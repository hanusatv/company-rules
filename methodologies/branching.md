---
methodology_id: git-branching
title: Branching
priority: high
tags: [naming, standards, conventions, git]
---

# Git Branching Standard

## 1. Base Branch

Feature branches MUST:

- Be created from the latest version of the `master` branch.
- Be created only after pulling the newest changes from remote.

Required workflow:

1. Checkout `master`
2. Pull latest changes from origin
3. Create new branch from updated `master`

---

## 2. Branch Naming Convention

Branch names MUST:

- Match the Jira ticket ID exactly.
- Be written in lowercase.
- Not contain spaces.
- Not contain additional text.

### Format

If Jira ticket ID is:

`TICKET-123`

Then the branch name MUST be:

`ticket-123`

---
- Use ticket ID as branch name.
- Do not add prefixes or descriptions.
