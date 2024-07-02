# Generic Data Ingestion Project (Used Cricket Related Data)

This project demonstrates an end-to-end data engineering pipeline for ingesting, processing, and analyzing cricket match data using Snowflake Cloud Data Warehouse. The project includes loading nested JSON files, transforming data, creating dimensional models, and visualizing the data through dashboards.


## Project Overview

The objective of this project is to build a comprehensive data pipeline that can handle cricket match data, transform it into a structured format, and provide meaningful insights through data analysis and visualization.

## Architecture

The project uses a layered architecture within Snowflake:
- **Landing Layer**: Temporary storage for raw JSON files uploaded from the source.
- **Raw Layer**: Stores raw, unprocessed data in its original format.
- **Clean Layer**: Transforms and cleans data to make it more structured and analyzable.
- **Consumption Layer**: Stores final processed data ready for analysis and reporting.

## Schemas

### Landing Layer
- **Purpose**: Temporary storage for raw JSON files.
- **Example**: JSON files uploaded using Snow Site Web UI.

### Raw Layer
- **Purpose**: Stores raw, unprocessed data.
- **Example**: JSON files copied from the landing layer.

### Clean Layer
- **Purpose**: Transforms and cleans data.
- **Example**: Flattening nested JSON structures and extracting relevant fields.

### Consumption Layer
- **Purpose**: Stores final processed data.
- **Example**: Creating fact and dimension tables for analysis.
