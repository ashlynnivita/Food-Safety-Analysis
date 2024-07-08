# Database and Analytics Programming - Extraction, Transformation, Loading and Visualization

## Food Data Fusion: Integrating Food & Drug Administration, Food Inspection, Nutrients, and Foodborne Disease Outbreaks for Enhanced Food Safety Analysis

### Introduction
The aim of this project is to integrate multiple datasets related to food safety, including data from the Food and Drug Administration (FDA), food inspection records, nutrient data, and disease outbreak reports, to enhance food safety analysis. ETL operations are then performed on the data and visualizations are done on the resultant data.

### Dependencies
This project uses the following packages:
* json
* requests
* pymongo
* pandas
* psycopg2
* sqlalchemy
* matplotlib
* seaborn
* wordcloud

### Softwares/Tools Required
1. Jupyter Notebook
2. MongoDB Compass GUI
3. PostgreSQL and pgAdmin4 GUI
4. MongoDB Atlas 

### Note:
1. The config.ipynb contains all the properties such as the databaseName, ports, username, password, connection string, etc. Connections with postgreSQL(hosted on an AWS EC2 instance) and mongoDB can be establised by utilising these properties.
2. All cells in the Master.ipynb must be run sequentially to view the final output.

### Steps Followed in the Analysis
* The following datasets are used :
    1. Dataset 1: Fda data extracted via api from fda.gov and loaded into mongoDB
    2. Dataset 2: Food Inspection data in json format is loaded into mongoDB
    3. Dataset 3: Food Nutrients in csv format
    4. Dataset 4: Foodborne Disease Outbreak in csv format
* Pre-processing, cleansing and transformation is performed on all four datasets.
* The final structured dataframe is loaded into postgresSQL.
* Datasets 2,3 and 4 are merged, thereby creating a single csv which is further visualised for statistical findings.
* Individual datasets are also visualised to obtained certain insights.



### Data Flow Diagram
<img src="https://github.com/Subash2409/pheonix/blob/master/Data%20flow%20diagram.png" alt="Data Flow Diagram" width="600" height="400">

### Cloud Architecture
<img src="https://github.com/Subash2409/pheonix/blob/master/Cloud%20Architecture.png" alt="Cloud Architecture" width="600" height="400">
