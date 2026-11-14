# Assignment evidence

Screenshots supplied with the project are grouped by topic under `evidence/` and referenced in `REPORT.md`.

## GitHub Actions

- [Initial 80/20 split passed](https://github.com/Vanisha1606/freshcard-pipelines/actions/runs/43594287133).
- [Intentional 70/30 split failed](https://github.com/Vanisha1606/freshcard-pipelines/actions/runs/43597144515); pytest reported 105 training rows instead of 120.
- [Fix restored 80/20 and passed](https://github.com/Vanisha1606/freshcard-pipelines/actions/runs/43597230323).

The supplied GitHub history screenshot was removed because it showed a different account and unrelated commit history. No GitHub run screenshot is included; use the linked Actions pages as the verified records.

## Snowflake

`evidence/Snowflake/` contains the supplied baseline summary, bronze raw rows, silver clean rows, and quarantine/dedup results. The login screenshot was excluded because it displayed account details.

## RabbitMQ

`evidence/RabbitMQ/` contains the supplied dispatcher, broker, node status, queue, and activity screenshots.

## Mage

`evidence/Mage/` contains the supplied pipeline graph, successful test run, depth results, and evaluation metrics.

The assignment brief was not present in the project folder. The Snowflake, RabbitMQ, and Mage evidence reflects the supplied screenshots and is not a new run from this session.
