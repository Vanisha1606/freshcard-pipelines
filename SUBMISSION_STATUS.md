# Submission status

Student: Vanisha Garg (23BCS254)

Repository: https://github.com/Vanisha1606/freshcard-pipelines

## Prepared

- GitHub Actions initial pass, intentional split failure, and fix pass verified in the connected repository: [run 1](https://github.com/Vanisha1606/freshcard-pipelines/actions/runs/43594287133), [run 2](https://github.com/Vanisha1606/freshcard-pipelines/actions/runs/43597144515), [run 3](https://github.com/Vanisha1606/freshcard-pipelines/actions/runs/43597230323).
- GitHub commit history screenshot included at `evidence/GitHub/github_commit_history.png`.
- Snowflake baseline results recorded: 6 silver rows, 2 quarantined rows, 4 deduplicated/gold orders, INR 7,785.00 revenue, 126 points, and 25% rejected share.
- Snowflake and RabbitMQ were run in the student's own environments; the report includes the available run screenshots.
- Instructor credentials and run outputs remain removed from the sanitized notebook.
- The report includes the SCD2, future-order quality check, topic routing, ACK/NACK explanations, and supplied Mage run evidence (CLI, depth results, evaluation metrics, and graph).

## Mage evidence

The Mage report section includes the successful run output, depth results, evaluation metrics, and pipeline graph. The project includes the 0.9 accuracy gate and `save_metrics` exporter.

The full report is `REPORT.md`; the PDF is in `report/23BCS254_Vanisha_Garg_Pipelines.pdf`.

Snowflake, RabbitMQ, and Mage evidence is grouped by topic under `evidence/`.
