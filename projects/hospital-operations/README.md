# Hospital operations dashboard

A multi-page view of hospital visits, costs, service mix, and patient experience, paired with a SQL Server example for preparing operational data for analysis.

![Hospital operations dashboard](../../assets/previews/hospital-operations.png)

## Questions explored

- How do visit volume and billing move over time?
- How do service type, department, diagnosis, and procedure relate to costs?
- What do satisfaction, insurance coverage, and payment status look like across visits?

## Tools

Power BI · SQL Server (T-SQL) · Excel · Data modelling

## SQL example

[`sql/01_hospital_operations.sql`](sql/01_hospital_operations.sql) defines a safe staging structure, parses dates and currency fields, and provides reusable visit-level and monthly cost summaries. It contains no patient records.

## Recommendations

- Review departments and procedures with high billed cost relative to visit volume, then validate case mix and coding with operational owners.
- Compare monthly service demand with costs and patient satisfaction to identify areas for a closer capacity or workflow review.
- Monitor volume, cost, and satisfaction together after any operational change; these synthetic records are not a basis for clinical decisions.

## Privacy

Only an aggregate dashboard preview is published. The source CSVs and interactive report are excluded because source data can contain identifiable or sensitive information.
