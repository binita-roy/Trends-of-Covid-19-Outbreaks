# 🦠 Trends of Covid-19 Outbreaks

## 📌 Overview
This project focuses on analyzing the **Trends of Covid-19 Outbreaks** by building an end-to-end **ETL pipeline** using **Azure Data Factory (ADF)** and **Power BI** for visualization. The pipeline extracts Covid-19 datasets from an HTTP source, transforms them to handle inconsistencies, and loads the data into an **Azure SQL Database**. Finally, interactive dashboards in **Power BI** provide insights into the pandemic trends across multiple countries.

## 🔄 Project Workflow
1. **Extract**: Data is retrieved from an HTTP API using **Azure Data Factory (ADF)**.
2. **Transform**: Data Flow in ADF is used to:
   - Handle missing values.
   - Remove inconsistencies.
   - Define appropriate data types.
3. **Load**: The cleaned data is stored in an **Azure SQL Database**.
4. **Orchestration**: The entire pipeline is automated with **scheduled triggers** in ADF.
5. **Visualization**: Power BI is connected to the Azure SQL Database to create insightful dashboards.

## 📂 Data Sources
The project extracts the following datasets:
- **cases_deaths**: Contains daily Covid-19 cases and deaths per country.
- **hospital_admissions**: Captures hospital and ICU occupancy due to Covid-19.
- **testing**: Provides Covid-19 testing data per country.

## 🛠️ Technologies Used
- **Azure Data Factory (ADF)**: For ETL pipeline automation.
- **Azure SQL Database**: For storing transformed data.
- **Power BI**: For data visualization and dashboard creation.
- **SQL**: For querying and managing the database.
- **HTTP Connector**: For data extraction.

## 🔧 Data Pipeline Architecture
The ETL pipeline consists of:
- **Ingestion Pipeline**: Extracts data from API sources.
- **Transformation Pipeline**: Cleans and processes the data.
- **Load Pipeline**: Loads the transformed data into the database.

### 📊 ETL Pipeline Diagram
![ETL Pipeline](./ETL%20Pipeline_Covid19.PNG)

## 🗄️ Database Schema
The Azure SQL Database consists of three main tables:
1. **covid_reporting_cases_and_deaths**
2. **covid_reporting_hospital_admissions**
3. **covid_reporting_testing**

### 🏛️ Database Schema Diagram
![Database Schema](./Database_Covid%2019.PNG)

## 📈 Power BI Dashboards
The project includes interactive Power BI dashboards:

1. **📊 Covid-19 Outbreak Trends**
   ![Dashboard - Trends](./Dashboard_Trends_Covid%2019.PNG)

2. **🌍 Covid-19 Cases by Country**
   ![Dashboard - Country Trends](./Dashboard_Country%20Trends_Covid%2019.PNG)

3. **🧪 Covid-19 Testing Trends**
   ![Dashboard - Testing Trends](./Dashboard_Testing_Covid%2019.PNG)

## 🚀 How to Use the Project
### ✅ Prerequisites
- Azure account with **Azure Data Factory** and **Azure SQL Database**.
- Power BI installed for visualization.

### 📌 Steps to Run the Project
1. **Set up the Database**
   - Execute the SQL script [`SQL Database_Covid 19.sql`](./SQL%20Database_Covid%2019.sql) to create tables in Azure SQL Database.

2. **Configure Azure Data Factory**
   - Import and set up the ADF pipelines for data ingestion, transformation, and loading.
   - Schedule the pipeline execution using triggers.

3. **Connect Power BI to Azure SQL Database**
   - Load the processed data into Power BI.
   - Use provided dashboard templates to visualize trends.

## 📊 Key Insights from the Project
- **Testing vs Confirmed Cases**: The number of tests performed correlates with the rise in confirmed cases.
- **Hospital Occupancy Trends**: The ICU and hospital occupancy rates reflect the severity of outbreaks.
- **Country-wise Covid-19 Trends**: Trends in cases, deaths, and hospitalizations across different countries.

## 🎯 Skills Demonstrated
- **ETL Pipeline Development** using Azure Data Factory.
- **Data Transformation & Cleaning** with Data Flows.
- **SQL Database Design & Querying**.
- **Data Visualization** with Power BI.
- **Pipeline Orchestration** using Scheduled Triggers in ADF.

## 🚀 Future Improvements
- Automate the data pipeline to fetch real-time Covid-19 data.
- Expand the analysis to include vaccination trends.
- Optimize Power BI dashboards for more interactive insights.

## 👤 Author
- **Binita Roy**
- **Contact**: [LinkedIn](https://www.linkedin.com/in/binita-roy/) | [Email](mailto:binitaroy1312@gmail.com)

