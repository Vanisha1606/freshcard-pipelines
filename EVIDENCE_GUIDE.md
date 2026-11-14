# Assignment evidence

Screenshots supplied with the project are grouped by topic under `evidence/` and referenced in `REPORT.md`.

## GitHub Actions

- [Initial 80/20 split passed](https://github.com/Vanisha1606/freshcard-pipelines/actions/runs/43594287133).
- [Intentional 70/30 split failed](https://github.com/Vanisha1606/freshcard-pipelines/actions/runs/43597144515); pytest reported 105 training rows instead of 120.
- [Fix restored 80/20 and passed](https://github.com/Vanisha1606/freshcard-pipelines/actions/runs/43597230323).

The repository commit history and CI checks are shown in [`evidence/GitHub/github_commit_history.png`](evidence/GitHub/github_commit_history.png). The linked Actions pages provide the detailed run records.

## Snowflake

`evidence/Snowflake/` contains the supplied baseline summary, bronze raw rows, silver clean rows, and quarantine/dedup results.

## RabbitMQ

`evidence/RabbitMQ/` contains the supplied dispatcher, broker, node status, queue, and activity screenshots.

## Mage

`evidence/Mage/` contains the supplied pipeline graph, successful test run, depth results, and evaluation metrics.

The Snowflake, RabbitMQ, and Mage sections in `REPORT.md` reference the supplied screenshots.
