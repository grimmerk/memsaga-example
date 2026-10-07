---
type: Translation
title: architecture (zh-TW)
description: Traditional Chinese translation of webapp docs/architecture.md
sources:
  - resource: ~/git/webapp/docs/architecture.md
    last_modified: 2026-10-05T09:00:00+01:00
    commit: 385e48f
generated:
  by: claude-code
  at: 2026-10-07T15:20:00+01:00
status: stable
---
# 架構

webapp 是一個 Node.js 伺服器，前端用 React。

- `server/` 處理 session 與 OAuth callback。
- `web/` 是 React 應用程式，透過 `/api` 和伺服器溝通。
- 背景工作在 `worker/` 執行，和伺服器共用同一個資料庫。
