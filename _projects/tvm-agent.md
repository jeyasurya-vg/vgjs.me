---
layout: page
title: TVM AI Agent
description: >
  Production LangGraph-based autonomous agent automating enterprise
  threat and vulnerability management workflows.
img: assets/img/projects/tvm-agent.png
importance: 1
category: tools
github: jeyasuryavg/tvm-ai-agent
---

A production-grade autonomous agent built on LangGraph that automates the bulk of daily
TVM analyst tasks. Integrates Ivanti Neurons RBVM across four platform URLs, Securin RBVM,
Jira, ServiceNow, Slack, and Microsoft Teams via API.

**Key design decisions:**
- Dual-layer data extraction from Securin's platform
- EASM findings without CVE IDs handled via Securin weakness IDs
- Per-source API rate limiting to avoid throttling
- Dual-mode LLM backend switchable via environment variable
- Qwen3-30B-A3B as the recommended local model for 4GB VRAM constraints

**Stack:** Python, LangGraph, LangChain, FastAPI, SQLite, Docker
