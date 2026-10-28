---
name: Bug Report
about: Create a report to help us improve
title: ''
labels: ''
assignees: ''

---

name: Bug report
description: Report a reproducible problem.
title: "[Bug]: "
labels:
  - bug
body:
  - type: markdown
    attributes:
      value: |
        Describe the problem clearly.
        Do not include credentials, private keys, or sensitive proxy details.

  - type: textarea
    id: description
    attributes:
      label: Description
      description: What happened?
      placeholder: Describe the issue.
    validations:
      required: true

  - type: textarea
    id: reproduction
    attributes:
      label: Steps to reproduce
      description: List the steps needed to reproduce the issue.
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: Expected behavior
      description: What should have happened?
    validations:
      required: true

  - type: textarea
    id: logs
    attributes:
      label: Relevant logs
      description: Remove secrets and personal information before posting.
      render: text
    validations:
      required: false

  - type: input
    id: environment
    attributes:
      label: Environment
      description: OS, Python version, or relevant workflow run.
    validations:
      required: false
