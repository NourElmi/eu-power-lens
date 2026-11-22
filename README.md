
# EU Power Lens

Forecasting European day-ahead electricity prices and demand from
public ENTSO-E data, from raw API to tested pipeline, forecasts and
an AI assistant.

> 🚧 Work in progress (started Nov 2026). Roadmap below.

## Why

Electricity prices in Europe are volatile (negative prices, spikes).
Traders, suppliers and grid operators need clean data and reliable
forecasts. This project builds that end to end on real, messy data.

## Stack

Python 3.12 · uv · pandas · PostgreSQL (Docker) · SQLAlchemy ·
pytest · ruff · ENTSO-E Transparency Platform API

## Roadmap

- [X] Project setup (uv, Docker, Postgres)
- [ ] Ingest day-ahead prices, load and generation
- [ ] Data model and data-quality checks
- [ ] Forecasting with backtesting
- [ ] Orchestration and cloud deployment (Azure)
- [ ] AI assistant over the data, with evaluations

## Run it locally

1. Get a free ENTSO-E API token (https://transparency.entsoe.eu).
2. `cp .env.example .env` and set `ENTSOE_TOKEN`.
3. `uv sync`
4. `docker compose up -d`   (from week 1)

## Data

Source: ENTSO-E Transparency Platform. Data is not stored in this repo.
