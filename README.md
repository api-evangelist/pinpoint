# Pinpoint (pinpoint)

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
