# Amazon Detective

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Amazon Detective is a security investigation service that makes it easy to analyze, investigate, and quickly identify the root cause of potential security issues or suspicious activities. It automatically collects log data from your AWS resources and uses machine learning, statistical analysis, and graph theory to build interactive visualizations that help you conduct faster and more efficient security investigations.

**Areas:** AWS · Forensics · Investigations · Security

## Amazon Detective on APIs.io

Everything profiled for Amazon Detective is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/amazon-detective/](https://apis.io/providers/amazon-detective/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Amazon Detective Graph API](https://apis.io/apis/amazon-detective/amazon-detective-graph-api/) — Behavior graph management operations
- [Amazon Detective Investigations API](https://apis.io/apis/amazon-detective/amazon-detective-investigations-api/) — Security investigation operations
- [Amazon Detective Invitations API](https://apis.io/apis/amazon-detective/amazon-detective-invitations-api/) — Invitation management for member accounts
- [Amazon Detective Members API](https://apis.io/apis/amazon-detective/amazon-detective-members-api/) — Member account management operations
- [Amazon Detective Organizations API](https://apis.io/apis/amazon-detective/amazon-detective-organizations-api/) — AWS Organizations integration operations
- [Amazon Detective Tags API](https://apis.io/apis/amazon-detective/amazon-detective-tags-api/) — Resource tagging operations
- [Amazon Detective Data Sources API](https://apis.io/apis/amazon-detective/amazon-detective-data-sources-api/) — Data source package management operations

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (7)

Multi-step workflows that chain operations into a business task.

- [Amazon Detective Archive a Resolved Investigation](https://apis.io/arazzos/amazon-detective/amazon-detective-archive-resolved-investigation-workflow/)
- [Amazon Detective Enable a Data Source Package](https://apis.io/arazzos/amazon-detective/amazon-detective-enable-datasource-package-workflow/)
- [Amazon Detective Onboard a Behavior Graph with Member Accounts](https://apis.io/arazzos/amazon-detective/amazon-detective-graph-onboard-members-workflow/)
- [Amazon Detective Member Accepts a Behavior Graph Invitation](https://apis.io/arazzos/amazon-detective/amazon-detective-member-accept-invitation-workflow/)
- [Amazon Detective Run an Investigation and Collect Indicators](https://apis.io/arazzos/amazon-detective/amazon-detective-run-investigation-workflow/)
- [Amazon Detective Start Monitoring a Member Account](https://apis.io/arazzos/amazon-detective/amazon-detective-start-monitoring-member-workflow/)
- [Amazon Detective Tag a Behavior Graph](https://apis.io/arazzos/amazon-detective/amazon-detective-tag-behavior-graph-workflow/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Amazon Detective Agentic Access](https://apis.io/agentic-access/amazon-detective/amazon-detective-agentic-access/)

#### JSON Schema (54)

The data models the API reads and writes.

- [AcceptInvitationRequest](https://apis.io/schemas/amazon-detective/amazon-detective-accept-invitation-request/)
- [Account](https://apis.io/schemas/amazon-detective/amazon-detective-account/)
- [Administrator](https://apis.io/schemas/amazon-detective/amazon-detective-administrator/)
- [BatchGetGraphMemberDatasourcesRequest](https://apis.io/schemas/amazon-detective/amazon-detective-batch-get-graph-member-datasources-request/)
- [BatchGetGraphMemberDatasourcesResponse](https://apis.io/schemas/amazon-detective/amazon-detective-batch-get-graph-member-datasources-response/)
- [BatchGetMembershipDatasourcesRequest](https://apis.io/schemas/amazon-detective/amazon-detective-batch-get-membership-datasources-request/)
- [BatchGetMembershipDatasourcesResponse](https://apis.io/schemas/amazon-detective/amazon-detective-batch-get-membership-datasources-response/)
- [CreateGraphRequest](https://apis.io/schemas/amazon-detective/amazon-detective-create-graph-request/)
- [CreateGraphResponse](https://apis.io/schemas/amazon-detective/amazon-detective-create-graph-response/)
- [CreateMembersRequest](https://apis.io/schemas/amazon-detective/amazon-detective-create-members-request/)
- [CreateMembersResponse](https://apis.io/schemas/amazon-detective/amazon-detective-create-members-response/)
- [DatasourcePackageIngestDetail](https://apis.io/schemas/amazon-detective/amazon-detective-datasource-package-ingest-detail/)
- [DeleteGraphRequest](https://apis.io/schemas/amazon-detective/amazon-detective-delete-graph-request/)
- [DeleteMembersRequest](https://apis.io/schemas/amazon-detective/amazon-detective-delete-members-request/)
- [DeleteMembersResponse](https://apis.io/schemas/amazon-detective/amazon-detective-delete-members-response/)
- [DescribeOrganizationConfigurationRequest](https://apis.io/schemas/amazon-detective/amazon-detective-describe-organization-configuration-request/)
- [DescribeOrganizationConfigurationResponse](https://apis.io/schemas/amazon-detective/amazon-detective-describe-organization-configuration-response/)
- [DisassociateMembershipRequest](https://apis.io/schemas/amazon-detective/amazon-detective-disassociate-membership-request/)
- [EnableOrganizationAdminAccountRequest](https://apis.io/schemas/amazon-detective/amazon-detective-enable-organization-admin-account-request/)
- [GetInvestigationRequest](https://apis.io/schemas/amazon-detective/amazon-detective-get-investigation-request/)
- [GetInvestigationResponse](https://apis.io/schemas/amazon-detective/amazon-detective-get-investigation-response/)
- [GetMembersRequest](https://apis.io/schemas/amazon-detective/amazon-detective-get-members-request/)
- [GetMembersResponse](https://apis.io/schemas/amazon-detective/amazon-detective-get-members-response/)
- [Graph](https://apis.io/schemas/amazon-detective/amazon-detective-graph/)
- [Indicator](https://apis.io/schemas/amazon-detective/amazon-detective-indicator/)
- …and 29 more published on APIs.io

#### JSON Structure (54)

Data models expressed in JSON Structure.

- [Amazon Detective Accept Invitation Request Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-accept-invitation-request-structure/)
- [Amazon Detective Account Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-account-structure/)
- [Amazon Detective Administrator Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-administrator-structure/)
- [Amazon Detective Batch Get Graph Member Datasources Request Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-batch-get-graph-member-datasources-request-structure/)
- [Amazon Detective Batch Get Graph Member Datasources Response Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-batch-get-graph-member-datasources-response-structure/)
- [Amazon Detective Batch Get Membership Datasources Request Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-batch-get-membership-datasources-request-structure/)
- [Amazon Detective Batch Get Membership Datasources Response Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-batch-get-membership-datasources-response-structure/)
- [Amazon Detective Create Graph Request Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-create-graph-request-structure/)
- [Amazon Detective Create Graph Response Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-create-graph-response-structure/)
- [Amazon Detective Create Members Request Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-create-members-request-structure/)
- [Amazon Detective Create Members Response Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-create-members-response-structure/)
- [Amazon Detective Datasource Package Ingest Detail Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-datasource-package-ingest-detail-structure/)
- [Amazon Detective Delete Graph Request Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-delete-graph-request-structure/)
- [Amazon Detective Delete Members Request Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-delete-members-request-structure/)
- [Amazon Detective Delete Members Response Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-delete-members-response-structure/)
- [Amazon Detective Describe Organization Configuration Request Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-describe-organization-configuration-request-structure/)
- [Amazon Detective Describe Organization Configuration Response Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-describe-organization-configuration-response-structure/)
- [Amazon Detective Disassociate Membership Request Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-disassociate-membership-request-structure/)
- [Amazon Detective Enable Organization Admin Account Request Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-enable-organization-admin-account-request-structure/)
- [Amazon Detective Get Investigation Request Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-get-investigation-request-structure/)
- [Amazon Detective Get Investigation Response Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-get-investigation-response-structure/)
- [Amazon Detective Get Members Request Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-get-members-request-structure/)
- [Amazon Detective Get Members Response Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-get-members-response-structure/)
- [Amazon Detective Graph Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-graph-structure/)
- [Amazon Detective Indicator Structure](https://apis.io/json-structure/amazon-detective/amazon-detective-indicator-structure/)
- …and 29 more published on APIs.io

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Amazon Detective Context](https://apis.io/jsonld/amazon-detective/amazon-detective-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Amazon Detective Vocabulary](https://apis.io/vocabularies/amazon-detective/amazon-detective-vocabulary/)

#### Examples (54)

Example requests and responses.

- [Amazon Detective Accept Invitation Request Example](https://apis.io/examples/amazon-detective/amazon-detective-accept-invitation-request-example/)
- [Amazon Detective Account Example](https://apis.io/examples/amazon-detective/amazon-detective-account-example/)
- [Amazon Detective Administrator Example](https://apis.io/examples/amazon-detective/amazon-detective-administrator-example/)
- [Amazon Detective Batch Get Graph Member Datasources Request Example](https://apis.io/examples/amazon-detective/amazon-detective-batch-get-graph-member-datasources-request-example/)
- [Amazon Detective Batch Get Graph Member Datasources Response Example](https://apis.io/examples/amazon-detective/amazon-detective-batch-get-graph-member-datasources-response-example/)
- [Amazon Detective Batch Get Membership Datasources Request Example](https://apis.io/examples/amazon-detective/amazon-detective-batch-get-membership-datasources-request-example/)
- [Amazon Detective Batch Get Membership Datasources Response Example](https://apis.io/examples/amazon-detective/amazon-detective-batch-get-membership-datasources-response-example/)
- [Amazon Detective Create Graph Request Example](https://apis.io/examples/amazon-detective/amazon-detective-create-graph-request-example/)
- [Amazon Detective Create Graph Response Example](https://apis.io/examples/amazon-detective/amazon-detective-create-graph-response-example/)
- [Amazon Detective Create Members Request Example](https://apis.io/examples/amazon-detective/amazon-detective-create-members-request-example/)
- [Amazon Detective Create Members Response Example](https://apis.io/examples/amazon-detective/amazon-detective-create-members-response-example/)
- [Amazon Detective Datasource Package Ingest Detail Example](https://apis.io/examples/amazon-detective/amazon-detective-datasource-package-ingest-detail-example/)
- [Amazon Detective Delete Graph Request Example](https://apis.io/examples/amazon-detective/amazon-detective-delete-graph-request-example/)
- [Amazon Detective Delete Members Request Example](https://apis.io/examples/amazon-detective/amazon-detective-delete-members-request-example/)
- [Amazon Detective Delete Members Response Example](https://apis.io/examples/amazon-detective/amazon-detective-delete-members-response-example/)
- [Amazon Detective Describe Organization Configuration Request Example](https://apis.io/examples/amazon-detective/amazon-detective-describe-organization-configuration-request-example/)
- [Amazon Detective Describe Organization Configuration Response Example](https://apis.io/examples/amazon-detective/amazon-detective-describe-organization-configuration-response-example/)
- [Amazon Detective Disassociate Membership Request Example](https://apis.io/examples/amazon-detective/amazon-detective-disassociate-membership-request-example/)
- [Amazon Detective Enable Organization Admin Account Request Example](https://apis.io/examples/amazon-detective/amazon-detective-enable-organization-admin-account-request-example/)
- [Amazon Detective Get Investigation Request Example](https://apis.io/examples/amazon-detective/amazon-detective-get-investigation-request-example/)
- [Amazon Detective Get Investigation Response Example](https://apis.io/examples/amazon-detective/amazon-detective-get-investigation-response-example/)
- [Amazon Detective Get Members Request Example](https://apis.io/examples/amazon-detective/amazon-detective-get-members-request-example/)
- [Amazon Detective Get Members Response Example](https://apis.io/examples/amazon-detective/amazon-detective-get-members-response-example/)
- [Amazon Detective Graph Example](https://apis.io/examples/amazon-detective/amazon-detective-graph-example/)
- [Amazon Detective Indicator Example](https://apis.io/examples/amazon-detective/amazon-detective-indicator-example/)
- …and 29 more published on APIs.io

#### Collections (9)

Postman and Open Collection request collections.

- [Amazon Detective](https://apis.io/collections/amazon-detective/open-amazon-detective/)
- [Amazon Detective Datasources API](https://apis.io/collections/amazon-detective/open-amazon-detective-datasources-api/)
- [Amazon Detective Datasources Graph API](https://apis.io/collections/amazon-detective/open-amazon-detective-graph-api/)
- [Amazon Detective Datasources Investigations API](https://apis.io/collections/amazon-detective/open-amazon-detective-investigations-api/)
- [Amazon Detective Datasources Invitations API](https://apis.io/collections/amazon-detective/open-amazon-detective-invitations-api/)
- [Amazon Detective Datasources Members API](https://apis.io/collections/amazon-detective/open-amazon-detective-members-api/)
- [Amazon Detective Datasources Organizations API](https://apis.io/collections/amazon-detective/open-amazon-detective-organizations-api/)
- [Amazon Detective Datasources Tags API](https://apis.io/collections/amazon-detective/open-amazon-detective-tags-api/)
- [Amazon Detective](https://apis.io/collections/amazon-detective/postman-amazon-detective/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Amazon Detective — jsonschema rules](https://apis.io/rules/amazon-detective/amazon-detective-jsonschema-spectral-rules/)
- [Amazon Detective API Rules](https://apis.io/rules/amazon-detective/amazon-detective-spectral-rules/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Amazon Detective Authentication](https://apis.io/security/amazon-detective/amazon-detective-authentication/)
- [Amazon Detective Domain Security](https://apis.io/security/amazon-detective/amazon-detective-domain-security/)
- [Amazon Detective Trust Center](https://apis.io/security/amazon-detective/amazon-detective-trust-center/)
- [Amazon Detective Vulnerability Disclosure](https://apis.io/security/amazon-detective/amazon-detective-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Amazon Detective Plans Pricing](https://apis.io/plans/amazon-detective/amazon-detective-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Amazon Detective Rate Limits](https://apis.io/rate-limits/amazon-detective/amazon-detective-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Amazon Detective Finops](https://apis.io/finops/amazon-detective/amazon-detective-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://aws.amazon.com/detective/)
- [Documentation](https://docs.aws.amazon.com/detective/)
- [Support](https://aws.amazon.com/premiumsupport/)
- [Blog](https://aws.amazon.com/blogs/security/tag/amazon-detective/)
- [Terms of service](https://aws.amazon.com/service-terms/)
- [Privacy policy](https://aws.amazon.com/privacy/)
- [GitHub](https://github.com/aws)
- [Status](https://health.aws.amazon.com/health/status)

## API Evangelist rating

**Kin Score 49.8** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 69.6 |
| Contract quality | 31.7 |
| Contract governance | 27.3 |
| Operational transparency | 52.6 |
| Developer ergonomics | 58.3 |
| Access clarity | 53.9 |

**Agent readiness 30.2** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 35.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/amazon-detective/](https://apis.io/providers/amazon-detective/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Amazon Detective: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/amazon-detective/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
