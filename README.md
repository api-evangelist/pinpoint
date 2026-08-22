# Pinpoint (pinpoint)

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

Pinpoint is an applicant tracking system (ATS) and recruitment platform for in-house talent teams. Its REST API follows the JSON:API specification and is served per-tenant at https://{subdomain}.pinpointhq.com/api/v1, exposing jobs, applications, candidates, comments, files, and webhooks for building recruitment integrations. Not to be confused with AWS Pinpoint (customer engagement) or Pinpoint (signal/data intelligence).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/apis.yml)

## Tags

- ATS
- Recruitment
- Hiring
- HR Tech
- JSON:API

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Pinpoint Jobs API

List, fetch, create, update, and destroy job postings (requisitions), with JSON:API filtering by status, department, location, and division, plus pagination, sorting, and related includes for departments, locations, stages, and applications.

- **Human URL:** [https://developers.pinpointhq.com/reference/get-jobs](https://developers.pinpointhq.com/reference/get-jobs)
- **Base URL:** `https://{subdomain}.pinpointhq.com/api/v1`

#### Tags

- Jobs
- Requisitions
- Recruitment

#### Properties

- [Documentation](https://developers.pinpointhq.com/docs/introduction)
- [API Reference](https://developers.pinpointhq.com/reference/get-jobs)
- [OpenAPI](openapi/pinpoint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pinpoint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pinpoint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pinpoint Applications API

Manage candidate applications as they move through a job's hiring workflow — list, fetch, create, update, and destroy applications, with includes for jobs, candidates, stages, and offers via JSON:API relationships.

- **Human URL:** [https://developers.pinpointhq.com/reference/get-applications](https://developers.pinpointhq.com/reference/get-applications)
- **Base URL:** `https://{subdomain}.pinpointhq.com/api/v1`

#### Tags

- Applications
- Pipeline
- Stages

#### Properties

- [Documentation](https://developers.pinpointhq.com/docs/introduction)
- [API Reference](https://developers.pinpointhq.com/reference/get-applications)
- [OpenAPI](openapi/pinpoint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pinpoint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pinpoint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pinpoint Applicants API

Read and update candidate (applicant) records — name, contact details, LinkedIn profile, and custom attributes — and access uploaded documents through the candidates resource using JSON:API extra_fields for attachments.

- **Human URL:** [https://developers.pinpointhq.com/reference/get-candidates](https://developers.pinpointhq.com/reference/get-candidates)
- **Base URL:** `https://{subdomain}.pinpointhq.com/api/v1`

#### Tags

- Applicants
- Candidates
- Talent Pool

#### Properties

- [Documentation](https://developers.pinpointhq.com/docs/introduction)
- [API Reference](https://developers.pinpointhq.com/reference/get-candidates)
- [OpenAPI](openapi/pinpoint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pinpoint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pinpoint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pinpoint Job Stages API

Read the hiring workflow stages a job exposes and reference them when moving applications through the pipeline, accessed as JSON:API related resources of jobs and applications.

- **Human URL:** [https://developers.pinpointhq.com/docs/introduction](https://developers.pinpointhq.com/docs/introduction)
- **Base URL:** `https://{subdomain}.pinpointhq.com/api/v1`

#### Tags

- Job Stages
- Hiring Workflow
- Pipeline

#### Properties

- [Documentation](https://developers.pinpointhq.com/docs/introduction)
- [OpenAPI](openapi/pinpoint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pinpoint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pinpoint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pinpoint Comments and Files API

List, fetch, and create comments on applications, and upload or read files and documents — submitted as base64 payloads on create and read back as attachments via JSON:API extra_fields.

- **Human URL:** [https://developers.pinpointhq.com/reference/get-comments](https://developers.pinpointhq.com/reference/get-comments)
- **Base URL:** `https://{subdomain}.pinpointhq.com/api/v1`

#### Tags

- Comments
- Files
- Attachments

#### Properties

- [Documentation](https://developers.pinpointhq.com/docs/introduction)
- [API Reference](https://developers.pinpointhq.com/reference/get-comments)
- [OpenAPI](openapi/pinpoint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pinpoint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pinpoint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pinpoint Webhooks

Subscribe to account events — new application, application moved, applicant hired, job created/updated/deleted, offer accepted, interview scheduled, and more — delivered as JSON payloads signed with a base64 PINPOINT-HMAC-SHA256 header and retried with exponential backoff.

- **Human URL:** [https://developers.pinpointhq.com/docs/webhooks-overview](https://developers.pinpointhq.com/docs/webhooks-overview)
- **Base URL:** `https://{subdomain}.pinpointhq.com/api/v1`

#### Tags

- Webhooks
- Events
- HMAC

#### Properties

- [Documentation](https://developers.pinpointhq.com/docs/webhooks-overview)
- [Documentation](https://developers.pinpointhq.com/docs/verifying-webhooks)
- [OpenAPI](openapi/pinpoint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pinpoint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pinpoint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/pinpoint-hq)
- [Website](https://www.pinpointhq.com)
- [Documentation](https://developers.pinpointhq.com/docs/introduction)
- [Plans](plans/pinpoint-plans-pricing.yml)
- [Rate Limits](rate-limits/pinpoint-rate-limits.yml)
- [Fin Ops](finops/pinpoint-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
