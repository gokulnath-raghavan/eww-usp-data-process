# EDW USP Data Process

This repository contains the service code for the Enterprise Data Warehouse (EDW) Universal Service Platform (USP) data processing pipeline.

## Repository Structure

### Glue
- `frameworks/`: Common framework utilities and shared code
- `jobs/`: AWS Glue ETL jobs
  - `pkg_variable_initialization/`: Variable initialization packages
  - `source_dw/`: Source to Data Warehouse transformations
  - `source_raw/`: Source to Raw data processing
  - `raw_normalized/`: Raw to Normalized data transformations
  - `normalized_stg/`: Normalized to Staging transformations
  - `stg_intermediate/`: Staging to Intermediate transformations
  - `intermediate_dw/`: Intermediate to Data Warehouse transformations
  - `stored_procedure_trigger/`: Stored procedure trigger jobs
  - `source_stage_cronjob/`: Source to Stage scheduled jobs
- `configs/`: Configuration files
  - `module-configs/`: Module-specific configurations
    - `APPS/`: Applications module configs
    - `INV/`: Inventory module configs
    - `ONT/`: Order and Trading module configs
- `tests/`: Test suites and test data

### Lambda
- `user_login/`: User authentication and authorization
  - `file_validation/`: File validation functions
  - `business_logic/`: Business logic implementation
  - `success_failure_lambda/`: Success/failure handling functions
- `common/`: Shared Lambda utilities

### Step Functions
- `apps_stg/`: Applications staging workflows
- `apps_order_views_stg/`: Application order views staging workflows
- `inv_stg/`: Inventory staging workflows

### Scripts
- `dms/`: Database Migration Service scripts
- `redshift/`: Redshift database scripts
  - `ddl/`: Data Definition Language scripts
  - `dml/`: Data Manipulation Language scripts
  - `views/`: Database views
- `maintenance/`: Maintenance scripts

### BI Analytics
- `power_bi/`: Power BI reports and dashboards

### CI/CD
- `bitbucket-pipelines/`: Bitbucket Pipelines configurations
- `scripts/`: CI/CD automation scripts

### Documentation
- `docs/`: Project documentation

## Getting Started

[Add setup instructions, prerequisites, and usage guidelines]

## Contributing

[Add contribution guidelines]

## License

[Add license information] 