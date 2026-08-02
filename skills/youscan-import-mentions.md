---
name: youscan-import-mentions
description: Import external mentions into a YouScan topic and track the import job to completion.
api: YouScan API
base_url: https://api.youscan.io/api/external
auth: X-API-KEY header
operations:
  - listTopics
  - createImport
  - getImportStatus
  - getImportErrors
  - abortImport
generated: '2026-07-21'
method: generated
source: openapi/youscan-openapi.yaml
---

# Import mentions into a YouScan topic

Load external mentions into a topic and monitor the asynchronous import job.

## Steps

1. **Pick the target topic.** `GET /topics` (`listTopics`) to resolve the `topicId`.
   You need Edit-level access to import.
2. **Create the import.** `POST /topics/{topicId}/imports` (`createImport`) with the
   mention payload (optionally `tagIds` to tag on ingest — get IDs from `listTags`).
   Returns `201` with an `importId`. Oversized payloads return `413`.
3. **Poll status.** `GET /topics/{topicId}/imports/{importId}` (`getImportStatus`) until
   `status` is terminal; read `savedCount` / `failedCount`.
4. **Inspect failures.** `GET /topics/{topicId}/imports/{importId}/errors`
   (`getImportErrors`) for per-mention `permaLink` + `error`.
5. **(If needed) Abort.** `POST /topics/{topicId}/imports/{importId}/abort` (`abortImport`)
   while running; a finished import returns `IMPORT_NOT_ABORTABLE`.

## Rules

- Auth: `X-API-KEY` header on every call.
- Rate limit: <=5 parallel, <=10 / 10s.
- Errors use `{errorCode, message}`; `VALIDATION_ERROR` (400) carries a per-field `errors[]`.
- No idempotency key — do not blindly retry `createImport`; check status first to avoid duplicates.
