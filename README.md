# Amazon Detective (amazon-detective)
Amazon Detective is a security investigation service that makes it easy to analyze, investigate, and quickly identify the root cause of potential security issues or suspicious activities. It automatically collects log data from your AWS resources and uses machine learning, statistical analysis, and graph theory to build interactive visualizations that help you conduct faster and more efficient security investigations.

**URL:** [Visit Amazon Detective](https://aws.amazon.com/detective/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - AWS, Forensics, Investigation, Security

## Timestamps

- **Created:** 2024-01-15
- **Modified:** 2026-04-19

## APIs

### Amazon Detective API
The Amazon Detective API provides programmatic access to manage security investigation workflows. It enables developers to create and manage behavior graphs, invite and manage member accounts, start and manage investigations, list indicators of compromise, manage data source packages, and configure AWS Organizations integration for multi-account security management.

**Human URL:** [https://aws.amazon.com/detective/](https://aws.amazon.com/detective/)

#### Tags:

 - AWS, Forensics, Investigation, Security

#### Properties

- [Documentation](https://docs.aws.amazon.com/detective/)
- [OpenAPI](openapi/amazon-detective-openapi.yml)
- [Pricing](https://aws.amazon.com/detective/pricing/)
- [GettingStarted](https://aws.amazon.com/detective/getting-started/)
- [FAQ](https://aws.amazon.com/detective/faqs/)
- [JSONSchema - Graph](json-schema/amazon-detective-graph-schema.json)
- [JSONSchema - Member Detail](json-schema/amazon-detective-member-detail-schema.json)
- [JSONSchema - Investigation Detail](json-schema/amazon-detective-investigation-detail-schema.json)
- [JSONSchema - Indicator](json-schema/amazon-detective-indicator-schema.json)
- [JSONSchema - Administrator](json-schema/amazon-detective-administrator-schema.json)
- [JSONStructure - Graph](json-structure/amazon-detective-graph-structure.json)
- [JSONStructure - Member Detail](json-structure/amazon-detective-member-detail-structure.json)
- [JSONStructure - Investigation Detail](json-structure/amazon-detective-investigation-detail-structure.json)
- [JSON-LD](json-ld/amazon-detective-context.jsonld)
- [Example - Graph](examples/amazon-detective-graph-example.json)
- [Example - Member Detail](examples/amazon-detective-member-detail-example.json)
- [Example - Investigation Detail](examples/amazon-detective-investigation-detail-example.json)

## Common Properties

- [Portal](https://aws.amazon.com/)
- [Website](https://aws.amazon.com/detective/)
- [Documentation](https://docs.aws.amazon.com/detective/)
- [TermsOfService](https://aws.amazon.com/service-terms/)
- [PrivacyPolicy](https://aws.amazon.com/privacy/)
- [Support](https://aws.amazon.com/premiumsupport/)
- [GitHubOrganization](https://github.com/aws)
- [Console](https://console.aws.amazon.com/detective/)
- [SignUp](https://signin.aws.amazon.com/signup?request_type=register)
- [Login](https://aws.amazon.com/console/)
- [StatusPage](https://health.aws.amazon.com/health/status)
- [Contact](https://aws.amazon.com/contact-us/)
- [Blog](https://aws.amazon.com/blogs/security/tag/amazon-detective/)
- [ReleaseNotes](https://docs.aws.amazon.com/detective/latest/userguide/release-notes.html)
- [SpectralRules](rules/amazon-detective-spectral-rules.yml)
- [Vocabulary](vocabulary/amazon-detective-vocabulary.yaml)
- [NaftikoCapability](capabilities/security-investigation.yaml)

## Features

| Name | Description |
|------|-------------|
| Behavior Graph Analysis | Automatically builds a behavior graph from log data using machine learning and graph theory to visualize security issues. |
| Security Investigations | Start and manage structured investigations on IAM users and roles with scoped time ranges and severity scoring. |
| Indicators of Compromise | Automatically identifies indicators including impossible travel, flagged IP addresses, new geolocations, new user agents, and TTP observations. |
| Multi-Account Support | Aggregate security data from multiple AWS accounts using an administrator account and member account model. |
| AWS Organizations Integration | Automatically enable new organization accounts as member accounts in the organization behavior graph. |
| Data Source Packages | Ingest security telemetry from CloudTrail, VPC Flow Logs, GuardDuty findings, EKS audit logs, and Active Directory audit logs. |
| Interactive Visualizations | Provides interactive graph visualizations in the AWS console to explore entity relationships and security events. |
| Investigation Severity Scoring | Assigns severity levels (Informational, Low, Medium, High, Critical) based on likelihood and impact of compromise indicators. |

## Use Cases

| Name | Description |
|------|-------------|
| Security Incident Investigation | Rapidly investigate security incidents by analyzing entity behavior, network activity, and API call patterns across your AWS environment. |
| Threat Hunting | Proactively search for suspicious activity and potential threats using behavior analysis and machine learning across your AWS accounts. |
| Root Cause Analysis | Identify the root cause of security issues by exploring the relationships between resources, users, and events in a behavior graph. |
| Compliance Forensics | Collect and preserve forensic evidence for compliance investigations using structured investigations with defined scope and time ranges. |
| Multi-Account Security Operations | Centrally manage security investigations across an AWS Organization from a single administrator account. |

## Integrations

| Name | Description |
|------|-------------|
| Amazon GuardDuty | Automatically ingests GuardDuty findings into the behavior graph for deeper investigation context. |
| AWS CloudTrail | Ingests CloudTrail API call logs to track user and service activity across your AWS environment. |
| Amazon VPC Flow Logs | Analyzes VPC flow logs to identify network communication patterns and anomalies. |
| Amazon EKS | Optionally ingests EKS audit logs to monitor Kubernetes API server activity. |
| AWS Organizations | Integrates with AWS Organizations to manage multi-account behavior graphs and auto-enable new accounts. |
| AWS Security Hub | Surfaces Detective investigation context within Security Hub for consolidated security findings. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Amazon Detective OpenAPI](openapi/amazon-detective-openapi.yml)

### JSON Schema

- [Graph Schema](json-schema/amazon-detective-graph-schema.json)
- [Member Detail Schema](json-schema/amazon-detective-member-detail-schema.json)
- [Investigation Detail Schema](json-schema/amazon-detective-investigation-detail-schema.json)
- [Indicator Schema](json-schema/amazon-detective-indicator-schema.json)
- [Administrator Schema](json-schema/amazon-detective-administrator-schema.json)
- [Account Schema](json-schema/amazon-detective-account-schema.json)
- [Start Investigation Request Schema](json-schema/amazon-detective-start-investigation-request-schema.json)
- [Get Investigation Response Schema](json-schema/amazon-detective-get-investigation-response-schema.json)
- [List Indicators Response Schema](json-schema/amazon-detective-list-indicators-response-schema.json)
- [Datasource Package Ingest Detail Schema](json-schema/amazon-detective-datasource-package-ingest-detail-schema.json)
- [Membership Datasources Schema](json-schema/amazon-detective-membership-datasources-schema.json)

### JSON Structure

- [Graph Structure](json-structure/amazon-detective-graph-structure.json)
- [Member Detail Structure](json-structure/amazon-detective-member-detail-structure.json)
- [Investigation Detail Structure](json-structure/amazon-detective-investigation-detail-structure.json)
- [Indicator Structure](json-structure/amazon-detective-indicator-structure.json)
- [Account Structure](json-structure/amazon-detective-account-structure.json)

### JSON-LD

- [Amazon Detective Context](json-ld/amazon-detective-context.jsonld)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Amazon Detective API](capabilities/shared/detective-api.yaml) — 27 operations for behavior graph management, member accounts, investigations, indicators, datasources, organizations, and tags

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Security Investigation](capabilities/security-investigation.yaml) | detective | 15 | SOC Analyst, Security Engineer |

## Vocabulary

- [Amazon Detective Vocabulary](vocabulary/amazon-detective-vocabulary.yaml) — Unified taxonomy mapping 8 resources, 10 actions, 1 workflow, and 2 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Amazon Detective Spectral Rules](rules/amazon-detective-spectral-rules.yml) — 40 rules across 10 categories enforcing Amazon Detective API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
