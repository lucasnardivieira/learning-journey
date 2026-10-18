# Data Engineering + AI Engineering Roadmap

12-month path (Oct 2026 → Oct 2027), ~6.5 h/week. This file is the source of truth for status.

**Weekly rhythm:** 2 × 1.5 h study · 1 × 3 h project · 30 min weekly review (`/weekly-review`).

Status legend: ⬜ not started · 🟨 in progress · ✅ done

**Timeline & weekly tasks:** [GitHub Project — Roadmap view](https://github.com/users/lucasnardivieira/projects/1). Hierarchy: Phase epic → checkpoint (M*n*.*x*) → session-sized issues, each with `Start` / `Target` / `Kind`. Later phases get their checkpoints planned near the end of the previous phase.

---

## Phase 0 — Foundation & workflow (weeks 1–2) ✅
- [x] Install git, gh, Docker, uv, ruff, pre-commit, Obsidian
- [x] `gh auth login`; push this repo to GitHub
- [x] GitHub Project board + milestones (Phases 0–5) — https://github.com/users/lucasnardivieira/projects/1
- [x] Global `~/.claude/CLAUDE.md` + skills (`weekly-review`, `new-portfolio-project`, `study-explain`)
- [x] GitHub audit: report → decisions → cleanup (see `vault/30-projects/github-audit-2026-10.md`)
- [x] Profile README + pinned repos
- [x] First weekly review

## Phase 1 — Modern data engineering (2026-10-19 → 2027-01-31) 🟨
**Topics:** Docker · Terraform basics · orchestration (Kestra in the course, Dagster in the project) · ingestion (dlt) · BigQuery · dbt · dimensional modeling · data quality · Spark/PySpark · streaming intro

| Checkpoint | Dates | Done when |
|---|---|---|
| **M1.1 Cloud foundations** | 10-19 → 11-08 | Zoomcamp M1 homework · GCP account with budget alert · Project 1 repo with green CI · Terraform `apply`/`destroy` tested |
| **M1.2 Orchestrated ingestion** | 11-09 → 11-29 | Zoomcamp M2 + dlt workshop · BCB + IBGE/SIDRA in GCS · Dagster schedule, idempotent, tested |
| **M1.3 Warehouse modeled** | 11-30 → 12-20 | Zoomcamp M3–M4 · Kimball ch. 1–4 · BigQuery raw + dbt marts with `dbt build` green |
| 🎄 Buffer | 12-21 → 01-03 | Catch-up or rest |
| **M1.4 Batch, streaming & ship** | 01-04 → 01-31 | Zoomcamp M5 (skim), M6, M7 · Project 1 shipped (quality, CI, dashboard, README, costs, teardown) · Phase 1 retro |

- [ ] DataTalks.Club DE Zoomcamp — Module 1: Docker, Postgres, Terraform, GCP
- [ ] Module 2: Workflow orchestration (Kestra)
- [ ] Workshop: Data ingestion (dlt)
- [ ] Module 3: Data warehouse (BigQuery)
- [ ] Module 4: Analytics engineering (dbt)
- [ ] Module 5: Data platforms (Bruin) — skim only
- [ ] Module 6: Batch processing (Spark)
- [ ] Module 7: Streaming (Kafka) — intro only, deepened in Phase 2
- [ ] Book: *Fundamentals of Data Engineering* (Reis & Housley) — extra reading, ~30 min/week
- [ ] Book: *The Data Warehouse Toolkit* ch. 1–4 (Kimball) — alongside Module 4
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
| 1 | Overview + foundation | ✅ |
| 2 | Phase 1 checkpoints + weekly tasks (Project 1 spec → issue #25) | ✅ |
| 3 | Phase 2 + Project 2 + AWS cert prep | ⬜ |
| 4 | Phase 3 + Projects 3–4 | ⬜ |
| 5 | Phase 4 + Project 5 | ⬜ |
| 6 | Capstone + personal brand | ⬜ |
