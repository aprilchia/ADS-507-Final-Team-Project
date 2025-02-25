# ADS-507-Final-Team-Project

# College Sports Financial Data Pipeline

## Respository Contents Overview
* [Jupyter Notebook](https://raw.githubusercontent.com/aprilchia/ADS-507-Final-Team-Project/refs/heads/main/ADS_507_Final_Project.ipynb) - to run the pipeline
* Raw CSV Files (sourced from Equity in Athletics Data Analysis [website](https://ope.ed.gov/athletics/#/)):
  * [Coaching_Staff.csv](https://raw.githubusercontent.com/aprilchia/ADS-507-Final-Team-Project/refs/heads/main/Coaching_Staff.csv): Annual head coach salary and head coach count for each sport.
  * [Expenses.csv](https://raw.githubusercontent.com/aprilchia/ADS-507-Final-Team-Project/refs/heads/main/Expenses.csv): Amount spent on each sport per year, including coaches payroll, operating expenses, and recruiting expenses.
  * [Revenue.csv](https://raw.githubusercontent.com/aprilchia/ADS-507-Final-Team-Project/refs/heads/main/Revenue.csv): Revenue of each sport and total revenue including expenses.
  * [Tableau Workbook](https://github.com/aprilchia/ADS-507-Final-Team-Project/blob/main/Tableau.twbx): Graph created from the net profit output table.

## Pipeline Deployment
### Prerequisites
* Python 3.x+ installed
* MySQL Server
* Required Python libraries (listed in first code block of script)
* Visual Studio Code (VSCode) with MySQL Tools

### Steps
1. Download the [Jupyter Notebook](https://raw.githubusercontent.com/aprilchia/ADS-507-Final-Team-Project/refs/heads/main/ADS_507_Final_Project.ipynb) file and the three raw CSV files.
2. Open VSCode and connect to your local MySQL server.
3. Run the downloaded file in VSCode (which uses "localhost" for the server address and "3306" for the port).
4. Enter your personal MySQL username and password in code block #5 and #21.
5. Allow the pipeline to run to completion.
6. The output net_profit table can be viewed in the database.
7. The [Tableau Workbook](https://github.com/aprilchia/ADS-507-Final-Team-Project/blob/main/Tableau.twbx) can be downloaded to generate a graph to visualize net profit.

## Pipeline Monitoring
* Logging: INFO messages are incorporated to show successful steps. ERROR messages highlight issues and stops the execution of the pipeline to help diagnose the issue.
* Monitoring: Run the query "curl http://localhost:8000" in terminal to view real-time monitoring metrics.
