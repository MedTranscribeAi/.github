---
layout: default
title: MedTranscribeAi – Release Notes
nav_order: 13
---

# MedTranscribeAi – Release Notes

## Latest Update (commit 5b19588, 2025‑08‑16)

### Highlights

-   **Dynamic log retention per stage** to meet SOC2 requirements, configurable through `logRetentionDays` mappings and applied via `logRetentionInDays` in the appointments service
-   **Expanded serverless microservices** covering core domains:

    -   Authentication API
    -   Appointments API
    -   Contacts API
    -   Organizations API
    -   Payment API
    -   Records API
    -   Transcription API with EKS integration
    -   Users API with custom domain support

-   **CI/CD automation** via CloudFormation templates for CodePipeline/CodeBuild in the devOps directory
-   **Comprehensive documentation** detailing system architecture, contribution guidelines, and authorization strategy
-   **Legal and compliance resources** outlining security practices for handling PHI and HIPAA/SOC2 adherence

### Testing

⚠️ No automated tests were executed; repository was examined via static analysis only.

### Notes

None.
