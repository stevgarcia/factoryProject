# Azure datafactory and databricks project
Welcome to the ##Azure data factory project##

This project demonstrates a comprehensive data warehousing and analytics solution, from bulding pipelines in datafactory, cleaning the data in databricks to generating reports in power BI. Designed as a complete Azure project that includes logic apps and monitoring.



<img width="1752" height="898" alt="arquitectura" src="https://github.com/user-attachments/assets/685840b7-478e-473b-998f-f050e425da4c" />

## 📖 Project Overview
This project involves:

1. **Data Architecture**: Designing a Modern Data solution Using data factory connected to Github and consuming files using pipelines.
2. **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse. (only in SQL)
3. **Data Modeling**: Developing fact and dimension tables optimized for analytical queries. (only in SQL)
4. **Analytics & Reporting**: Creating SQL-based reports and dashboards for actionable insights.

   
#### Objective
Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical reporting and informed decision-making.

#### Specifications
- **Data Sources**: Import data files from my local computer using a selfhostedIntegration runtime  and data factory pipelines
<img width="571" height="302" alt="image" src="https://github.com/user-attachments/assets/90d0adbb-5651-469b-b062-96ed81926b03" />

- the activities notify to logic apps in case of success or fail 

<img width="1098" height="435" alt="image" src="https://github.com/user-attachments/assets/e7ab77c9-5f4d-47c5-a6da-5d926e6e0607" />

- **Data layers**: an azure data lake Gen2 with 2 layers, a landing container "rawdata" and the transformed container

<img width="1034" height="323" alt="image" src="https://github.com/user-attachments/assets/124d8378-747a-473f-a1a6-3ca662b717bf" />

- **Integration**: deployment of an azure databricks connector to mount the lakeGen2 in order to make transformations with notebooks.

<img width="517" height="181" alt="image" src="https://github.com/user-attachments/assets/6b65de87-33ed-41f2-95a6-ac064c065aa6" />

- **serving layer**: a synapse serverless pool to get the transformed data .

  <img width="996" height="413" alt="image" src="https://github.com/user-attachments/assets/3f53e01f-2bdf-493e-b93a-4f34f98528d1" />

- **Presentation /report layer**: Connect power BI and synapse to create the final report

<img width="1208" height="508" alt="image" src="https://github.com/user-attachments/assets/7bd41cc0-2989-4e74-abd1-9b1979477ed1" />

