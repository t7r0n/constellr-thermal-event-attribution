# Thermal Event Attribution Workbench

A local physical-world analytics prototype for attributing synthetic thermal anomalies to decision-grade event categories with evidence trails.

## Features

- Synthetic thermal tiles, weather context, anomaly bands, and intervention signals.
- Attribution logic for crop stress, irrigation failure, equipment risk, and heat events.
- Structured reports, CSV outputs, and an offline dashboard for review.

## Run Locally

```bash
uv sync
uv run app init-demo
uv run app ingest fixtures/
uv run app analyze
uv run app verify
uv run app dashboard
uv run app benchmark
uv run app export-demo-pack
uv run pytest -q
uv run ruff check .
```

## Outputs

- `outputs/dashboard.html`
- `outputs/decision_report.md`
- `outputs/evidence_graph.mmd`
- `outputs/risk_or_quality_report.csv`
- `outputs/benchmark.md`
- `outputs/demo_pack.md`

## Data Policy

This project runs fully locally on deterministic synthetic fixtures. It does not require external APIs, credentials, private datasets, network access, or production systems.
