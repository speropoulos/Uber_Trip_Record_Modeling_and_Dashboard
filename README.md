## Uber Trip Record Modeling and Dashboard

[original dataset](https://github.com/speropoulos/Uber_Trip_Record_Modeling_and_Dashboard/tree/main/uber_dataset)

### Data modeling of the Uber dataset:

![uber_data_modeling_fact_dim_tables](https://github.com/speropoulos/Uber_Trip_Record_Modeling_and_Dashboard/blob/main/uber_data_modeling_fact_dim_tables.png?raw=true)

Here we are properly modeling the fact table after looking at the original dataset.

### Diagram showing the different technologies used:
![uber_data_pipeline_project_diagram](https://github.com/speropoulos/Uber_Trip_Record_Modeling_and_Dashboard/blob/main/uber_data_pipeline_project_diagram.png?raw=true)

### Cleaning the Uber dataset
[jupyter notebook](https://github.com/speropoulos/Uber_Trip_Record_Modeling_and_Dashboard/blob/main/uber_data_pipeline_project.ipynb) that does data cleaning on the uber dataset before being loaded onto MAGE.

### Mage ETL pipeline
![uber_data_pipeline_project_MAGE_code](https://i.gyazo.com/01b4202ba42380b941223467da60eeab.png)

With this modern data pipeline tool, its very easy to extract, transform, and load your datasets into tools like Google BigQuery. This is what we are doing if you look at the code. 

### BigQuery
Here is our fact table and dims we loaded in via MAGE.
![bq_fact_table_and_dim](https://i.gyazo.com/c74f623c446becc366114af84e291276.png)

Then we are going to create or replace our table on a schedule using MAGE, here is the query.

![bq_create_tbl_analytics](https://i.gyazo.com/fc718d4c6663098d9f123e5e2abf71b0.png)

Once we have this setup, we go to Looker Studio and build a dashboard to visualize the data findings.

![uber_dashboard_ss](https://i.gyazo.com/b2d8e05eb5ab876c4da933e8d944e8da.png)

You can view it in its entirety [here](https://lookerstudio.google.com/reporting/9842ab43-0b34-4e6d-95dc-77d31e812fe8)

