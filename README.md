# FreshCart Pipelines

Course project for **From Git to Gold** (Vanisha Garg, 23BCS254). Public repository: https://github.com/Vanisha1606/freshcard-pipelines

The repo contains a sanitized FreshCart notebook based on the instructor's supplied course material, an Iris Mage-style pipeline, RabbitMQ stream scripts, and report answers with grouped evidence. The notebook prompts for your own Snowflake login; course credentials and instructor run outputs were removed.

## Local setup

```bash
python3.12 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
pytest -q
```

Never commit `.env`, Snowflake credentials, broker URLs, or generated CSV/PKL outputs. Keep account secrets in Colab Secrets or local environment variables.

## Contents

- `tests/test_prepare_data.py`, `.github/workflows/ci.yml`: required 120/30 Iris split check and GitHub Actions pytest workflow (Python 3.12).
- `iris_project/`: importable Iris blocks with Mage decorator fallbacks, metadata, evaluation branch, and `save_metrics`.
- `stream/`: RabbitMQ dispatcher/driver and run instructions.
- `elt/freshcart_elt.ipynb`: supplied course flow with instructor credentials and outputs removed; includes the B3 currency rule and B5 quality check.
- `REPORT.md` and `report/23BCS254_Vanisha_Garg_Pipelines.pdf`: assignment answers and evidence appendix.
- `evidence/`: GitHub, Snowflake, RabbitMQ, and Mage screenshots grouped by topic.

## GitHub Actions

The workflow runs pytest on pushes and pull requests. Passing and intentional failing run links are recorded in `REPORT.md` after they are confirmed on this repository.

## Snowflake

Open `elt/freshcart_elt.ipynb` in Colab, enter your own credentials when prompted, and run the cells in order. Use screenshots and results from your own account in the submission.

## RabbitMQ

Set `RABBITMQ_URL` locally if using a hosted broker; leave it blank for localhost. Run three drivers in separate terminals and the dispatcher in another for the required two-minute observation. See `stream/README.md`.
