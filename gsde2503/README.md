# GSD2503 Structure

#### Problem folder (Stores the provided use case information)
- requirements → Contains the detailed explanation of the use case.

#### Solution folder (Stores the solution for the use case, organized into two main tasks)

1. ER_Diagram folder (Documents related to the first task)
    - ERD&analysis → Includes the Scala function to infer table schemas and queries to identify table relationships.
    - ER_Diagram Doc → Contains table definitions with an ERD explanation at the bottom.
    - ER Diagram.png → Visual representation of the ERD, depicting relationships among tables. Refer to the ER_Diagram Document for details.
    - Technologies Used: Scala, Spark, SQL, Databricks, Mural.
2. ELT Pipeline (Documents related to the second task)
    - 2a.bronze_load_checks have Functions and code for 
        - Raw data ingestion.
        - Primary key validation (uniqueness & non-null check).
        - Foreign key validation against one fact and hierarchy table.
        - Technologies Used: PySpark, SQL, Databricks.
    - 2b. silver_staging_tables have functions and code for
        - Defining table schemas with primary key constraints.
        - Table creation with constraints.
        - Data loading.
        - Technologies Used: PySpark, SQL, Databricks.
    - 2cd.gold_refined have queries for
        - Creating a refined table representing weekly sales data.
        - Implementing incremental logic for daily data ingestion using the upsert strategy.
        - Technologies Used: SQL, Databricks.
