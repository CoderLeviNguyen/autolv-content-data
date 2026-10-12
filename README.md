# AutoLV Content Data

Public portable publishing jobs for AutoLV Social and third-party consumers.

- `jobs/<profile_id>/<job_id>-r<revision>.json`: approved captions, verified HTTPS image/video URLs, destination aliases and schedule-only instructions.
- `manifests/<profile_id>.json`: approved job references.
- `receipts/<consumer_id>/<job_id>.json`: optional delivery receipts.
- `schemas/job-v1.example.json`: illustrative draft only; not authorized for publishing.

Specification: https://github.com/CoderLeviNguyen/skills/blob/master/social/autolv-shared-workflow/GITHUB_JOB_DELIVERY.md

SECURITY: Do not store credentials, private channel IDs or sensitive content in this public repository. GitHub jobs are not independent publishing authorization; workers must check trusted backend approval, LIVE queue and deduplicate before scheduling.

No real jobs are approved or queued at initialization.
