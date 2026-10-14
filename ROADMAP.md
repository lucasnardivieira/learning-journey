# Data Engineering + AI Engineering Roadmap

12-month path (Oct 2026 → Oct 2027), ~6.5 h/week. This file is the source of truth for status.

**Weekly rhythm:** 2 × 1.5 h study · 1 × 3 h project · 30 min weekly review (`/weekly-review`).

Status legend: ⬜ not started · 🟨 in progress · ✅ done

---

## Phase 0 — Foundation & workflow (weeks 1–2) 🟨
- [ ] Install git, gh, Docker, uv, ruff, pre-commit, Obsidian
- [ ] `gh auth login`; push this repo to GitHub
- [ ] GitHub Project board + milestones (Phases 0–5)
- [ ] Global `~/.claude/CLAUDE.md` + skills (`weekly-review`, `new-portfolio-project`, `study-explain`)
- [ ] GitHub audit: report → decisions → cleanup
- [ ] Profile README + pinned repos
- [ ] First weekly review

## Phase 1 — Modern data engineering (months 1–3) ⬜
**Topics:** Docker · Terraform basics · orchestration (Dagster/Airflow) · dbt · dimensional modeling · data quality · Spark/PySpark · BigQuery
- [ ] DataTalks.Club DE Zoomcamp — Module 1: Docker, Postgres, Terraform, GCP
- [ ] Module 2: Workflow orchestration
- [ ] Module 3: Data warehouse (BigQuery)
- [ ] Module 4: Analytics engineering (dbt)
- [ ] Module 5: Batch processing (Spark)
- [ ] Module 6: Streaming (Kafka) — intro only, deepened in Phase 2
- [ ] Book: *Fundamentals of Data Engineering* (Reis & Housley)
- [ ] Book: *The Data Warehouse Toolkit* ch. 1–4 (Kimball)
- [ ] **Project 1 — `br-open-data-platform`**: BCB SGS + IBGE/SIDRA → GCS → BigQuery · dbt · Dagster · Terraform · tests · CI · dashboard

## Phase 2 — Lakehouse, streaming & AWS (months 4–5) ⬜
**Topics:** Iceberg/Delta · Kafka/Redpanda · Spark Structured Streaming · S3/Glue/Athena/Lambda/IAM · Terraform on AWS · cost
- [ ] **Cert: AWS Certified Data Engineer – Associate (DEA-C01)**
- [ ] **Project 2 — `realtime-lakehouse-aws`**: events → Redpanda → Spark Streaming → Iceberg on S3 → Athena · full Terraform · teardown

## Phase 3 — AI Engineering (months 6–8) ⬜
**Topics:** Claude API (tool use, structured outputs, caching, batch) · embeddings · RAG · evals · Claude Agent SDK · MCP
- [ ] Anthropic Academy: Building with the Claude API · Introduction to MCP · Claude Code in Action
- [ ] DataTalks.Club LLM Zoomcamp
- [ ] Book: *AI Engineering* (Chip Huyen)
- [ ] **Project 3 — `data-docs-rag`**: RAG over Project 1's dbt docs/catalog + eval set
- [ ] **Project 4 — `warehouse-mcp-agent`**: read-only BigQuery MCP server + text-to-SQL agent with guardrails & evals

## Phase 4 — LLMOps & AI in production (months 9–10) ⬜
**Topics:** LLM observability · evals in CI · guardrails · unstructured extraction at scale · Vertex AI / Bedrock
- [ ] **Project 5 — `unstructured-to-warehouse`**: public PDFs → Claude Batch API extraction → schema validation → warehouse
- [ ] (Optional) Cert: Google Cloud Professional Data Engineer

## Phase 5 — Capstone & personal brand (months 11–12) ⬜
- [ ] Capstone: data platform + AI layer end-to-end, with ADRs
- [ ] 3–4 technical posts (dev.to / LinkedIn)
- [ ] Résumé + LinkedIn update

---

## Log of planning parts
| Part | Scope | Status |
|---|---|---|
| 1 | Overview + foundation | 🟨 |
| 2 | Phase 1 week-by-week + Project 1 spec | ⬜ |
| 3 | Phase 2 + Project 2 + AWS cert prep | ⬜ |
| 4 | Phase 3 + Projects 3–4 | ⬜ |
| 5 | Phase 4 + Project 5 | ⬜ |
| 6 | Capstone + personal brand | ⬜ |
