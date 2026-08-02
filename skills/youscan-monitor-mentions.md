---
name: youscan-monitor-mentions
description: Retrieve recent brand/topic mentions from YouScan and summarize their sentiment.
api: YouScan API
base_url: https://api.youscan.io/api/external
auth: X-API-KEY header
operations:
  - listTopics
  - listMentions
  - getSentimentsStatistics
  - getWordsStatistics
generated: '2026-07-21'
method: generated
source: openapi/youscan-openapi.yaml
---

# Monitor mentions with YouScan

Pull the latest mentions for a monitoring topic and report the sentiment split.

## Steps

1. **Find the topic.** `GET /topics` (`listTopics`). Match on `name` to get the `topicId`.
   The key only sees topics its user can access.
2. **Retrieve mentions.** `GET /topics/{topicId}/mentions` (`listMentions`). Filter with
   date (`from`/`to`, `addedFrom`/`addedTo`), `sourceTypes`, `postTypes`, `tags`, and
   sentiment params. Page through results — do not exceed the rate limit.
3. **Get sentiment breakdown.** `GET /topics/{topicId}/statistics/sentiments`
   (`getSentimentsStatistics`) for the positive/neutral/negative distribution.
4. **(Optional) Top themes.** `GET /topics/{topicId}/statistics/words`
   (`getWordsStatistics`) for the most frequent terms.

## Rules

- Auth: send `X-API-KEY: <key>` on every request (never the `apiKey` query param in production).
- Rate limit: <=5 parallel requests and <=10 requests / 10 seconds, or you get `429`.
- Coverage caveat: Reddit and Quora are excluded; Twitter/X is restricted (author/text/URL removed).
- Errors: a JSON body with `errorCode` + `message`; `404 RESOURCE_NOT_FOUND` deliberately
  hides topic existence; `402` means your plan lacks API access.
