# Job Board Queries (with Clearance Exclusions)

## LinkedIn
- ("internal tools" OR "integration engineer" OR "workflow automation" OR "analytics engineer" OR "data engineer") AND (APIs OR ETL OR "data pipelines") NOT ("security clearance" OR "eligible for clearance" OR "national security" OR SCADA OR PLC)

## Indeed
- ("internal tools" OR "integration engineer" OR "analytics engineer" OR "data engineer") (API OR ETL OR "data pipeline") -"security clearance" -"eligible for clearance" -"national security" -SCADA -PLC

## Built In
- "internal tools" OR "integration engineer" OR "analytics engineer" OR "data engineer" + (APIs OR ETL OR "data pipeline") -"security clearance" -"national security" -SCADA -PLC

## Wellfound
- "internal tools" OR "integration engineer" OR "analytics engineer" OR "data engineer" AND (APIs OR ETL OR "data pipeline") -"security clearance" -"eligible for clearance" -"national security" -SCADA -PLC

## Optional Variants
- "business systems engineer" AND (integrations OR automation) -"security clearance"
- "data platform" AND (ETL OR ELT) -"eligible for clearance"
- "internal tools" AND remote AND (APIs OR ETL) -"security clearance"
