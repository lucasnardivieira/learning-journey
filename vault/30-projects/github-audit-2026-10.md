---
type: decision
project: github-portfolio
date: 2026-10-14
status: proposed
---
# GitHub audit — 2026-10

Account: `lucasnardivieira` · 21 repos (20 public, 1 private) · currently pinned: spell_checker, projeto-AtmoAlert, projeto-priorize-me, pipeline-api.

**Main problem:** the profile tells a "full-stack / React" story while the target is **Data Engineering + AI Engineering**. Only one repo (`desafio_franq`) shows modern DE skills; the rest is academic work, bootcamp clones and one-off scripts, often with no README, committed `.pyc`/`.log` files or large datasets.

## 🚨 Security
| Repo | Issue | Action |
|---|---|---|
| (one old repo) | A committed cloud credential | Revoke the credential, then delete the repo. Lesson: never commit keys — use `.env` + secret managers + `detect-private-key` pre-commit hook. |
| airflow-docker | `.env` committed (only `AIRFLOW_UID` + credential *path* — no secret) | Remove from repo, add `.env.example` |

## Classification
| Repo | Proposal | Why |
|---|---|---|
| **desafio_franq** | ⭐ **Keep & improve** → rename `cnpj-dbt-pipeline`, README in English, CI, Mermaid diagram, pin | dbt + DuckDB + Prefect + SCD2 snapshots + tests: best DE showcase |
| myMovie | Keep & improve (later) | "Dream project"; remove 42 MB CSV from git (download script), real README |
| industrial-visao-computacional | Keep (archive) | Decent AI/CV notebook with README |
| segment_anything_way | Keep (archive) | CV experiment with README |
| gazenet_gaze_estimation | Keep (archive) | CV notebook with README |
| airflow-docker | Archive after cleanup (or make private) | Committed logs/.pyc; superseded by Project 1 |
| pipeline-api | Archive | 14-byte README; superseded by Project 1 |
| ETL_project | Make private | One script; superseded |
| scraper-ofertas | Make private | Empty README, `.pyc` committed |
| analise_dados_CEAPS | Make private | No README |
| spell_checker | Make private | Old NLTK experiment |
| Trabalho-compiladores | Make private | Academic |
| trabalho-poo | Make private | Academic, no README |
| projeto-AtmoAlert | Make private | Single `.ino` file, no README |
| fruitsDB | Make private | 525 PNG dataset, no code |
| react-project | Make private | Off-target (frontend) |
| projeto-priorize-me | Make private | Off-target (full-stack) |
| aws-bootcamp-cruddur-2023 | Make private | Bootcamp clone, 1 commit |
| teste_kindra_LucasN | Leave private | Technical test; build artifacts — harmless while private |
| lucasnardivieira (profile) | **Rewrite** | Reposition as Data + AI Engineer |

"Make private" keeps the code for you while removing noise from the public profile. "Archive" keeps it public but read-only.

## Target pinned set (evolves as projects ship)
1. learning-journey → 2. cnpj-dbt-pipeline → 3. br-open-data-platform (Project 1) → 4. myMovie (after cleanup) → 5–6. Projects 2–4 as they ship.

## Decisions
_(filled after review)_
