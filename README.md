# Formula1-Project

## Source of Dataset :
- http://ergast.com/mrd/

## ER Diagram of the Dataset :
![formula1_ergast_db_data_model](https://github.com/shekharj21/shekharj21/assets/54074505/992030b0-d5e0-447d-a388-fa5ee8adc640)

## Upload the data in Data Lake Gen 2:
![Screenshot (509)](https://github.com/shekharj21/shekharj21/assets/54074505/849e7cc2-341f-4b8e-88e2-b0a78f059458)

1. create Resource group and add storage account in it (Data Lake Gen2)
2. Add 4 folders inside container named as demo,presentation,processed and raw.
3. In the data File we have 6 files which are in CSV and JSON file format. Upload those file raw container.
4. Upload the 2 Folders too named as lap_times and qualifying.

## Data Ingestion Requirements :
1. Ingest all 8 files into data lake.
2. Ingested data must have the schema applied.
3. ingested data must have audit columns.
4. ingested data must be stored in columnar format ---- parquet.
5. Must be able to analyze the ingested data via SQL.
6. Ingestion logic must be able to handle incremental laod.


## Data transformation Requiremnts :
1. Join the key information required for reporting to create a new table.
2. Join the key information required for analysis to create a new table.
3. transformed data must have audit columns.
4. Must be able to analyze the transformed data via SQL.
5. Transformed data format ----- parquet.
6. Transformation logic must be Able to handle Incremental Load.
