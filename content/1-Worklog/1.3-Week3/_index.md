---
title: "Week 3 Worklog"
date: 2026-06-15
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 objectives

* Build and test the InsightShare application locally.
* Decouple storage and AI modules to simplify future integration.
* Test core workflows before deploying to AWS.

### Tasks during the week (15/06 - 19/06/2026)

| Day | Task | Start | End | Reference |
| --- | --- | --- | --- | --- |
| Mon | Initialize FastAPI project, design upload and file listing endpoints (`POST /files`, `GET /files`). | 15/06/2026 | 15/06/2026 | [FastAPI](https://fastapi.tiangolo.com/) |
| Tue | Implement upload and file listing APIs, storing data locally temporarily and returning file metadata. | 16/06/2026 | 16/06/2026 |  |
| Wed | Build basic web frontend (HTML/JS) featuring file upload form, file list, and progress bar. | 17/06/2026 | 17/06/2026 |  |
| Thu | Abstract Storage and AI layers using Python Abstract Base Classes, using mock data for AI services. | 18/06/2026 | 18/06/2026 |  |
| Fri | Refactor codebase into a 3-tier architecture (API - Service - Storage) and write unit tests with `pytest`. | 19/06/2026 | 19/06/2026 |  |

### Results achieved

1. Completed a working local application supporting file upload and listing via web UI.
2. Clearly decoupled storage and AI layers, ready for AWS service integration.
3. Standardized codebase architecture into layers with unit tests for core functionality.
