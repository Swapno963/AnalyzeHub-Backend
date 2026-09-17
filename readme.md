# AnalyzeHub API

Django REST API for a data dashboard: import records, then serve summary, correlation, and ranking endpoints for charts.

**Status:** personal / lab. Pair with [AnalyzeHub-Frontend](https://github.com/Swapno963/AnalyzeHub-Frontend).

---

## What it does

- REST endpoints for dashboard data
- Management commands to import and clean records
- Summary stats (counts, averages, min/max) and grouped counts (sector, topic, region, country)
- Top records by intensity, impact, relevance, likelihood

---

## What I built

- Django + DRF serializers and views
- Import/cleanup management commands
- CORS-enabled API for the React client

---

## Stack

Python, Django, Django REST Framework, PostgreSQL (via `dj-database-url` / psycopg).

---

## Run

```bash
git clone https://github.com/Swapno963/AnalyzeHub-Backend.git
cd AnalyzeHub-Backend
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```
