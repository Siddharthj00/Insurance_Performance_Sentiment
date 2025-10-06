# Insurance_Performance_Sentiment

## Problem Statement

The insurance industry plays a vital role in financial security and risk management.
However, insurers face challenges in maintaining profitability and operational efficiency.
This project aims to analyze the performance of insurance companies based on key financial indicators.
It will focus on metrics such as premiums earned, claims paid, operating expenses, and profits.
The goal is to identify strengths and weaknesses in their financial health.
The analysis will help improve decision-making and business strategies.
By understanding performance trends, the project supports sustainable growth in the insurance sector.

Ultimately, it seeks to provide actionable insights for enhancing company success.

### Features
* Data Import and Transformation: Efficient data handling in Microsoft SQL Server.
* Visualizations: 
  * Slicers with Policy number, Claim number and Customer ID so that the user can choose or filter the data as needed.

  * Multi row card for Gender and Gender Count.

  * Ribbon Chart of claim status against claim staus to show the status of claim against the count of claim 

  * Cards with key performance indicators including Premium Amount, Coveragre Amount and Claim Amount.
  * Interactive report with drill-through capabilities for processed and diagnosed claims.



* Sentiment Analysis: Text analytics to compute sentiment scores from customer feedback.

### Data Source
* insurance dataset: Imported dataset into Microsoft SQL Server.


### Steps followed 

- Step 1 : Create a database named insurance_db and Load data into Microsoft SQL Server, dataset is a csv file.
- Step 2 : Import the insurance dataset into Power BI using the SQL server import wizard.
- Step 3 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 4 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 5 : It was observed that in none of the columns errors & empty values were present. 
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Multi row Card was created with column Gender, the card represents the gender and the count of gender.
- Step 8 : Visual filters (Slicers) were added for three named "Policy Number", "Claim Number", & "Customer ID".
- Step 9 : Three card visuals were added to the canvas, representing Premium Amount, Coverage Amount and claim Amount.
- Step 10 : A stacked bar chart was also added to the report 
- Step 11 : Report was created with following visualizations
   <p align="center">
    <img src="https://github.com/user-attachments/assets/2de3ef37-0c79-42b0-85dd-211c22e052a0" width="800"/>
  </p>
- Step 12 : A table was created in the report consisting all the vital columns with drill through so that the filters could be appied from the main page to this page
    <p align="center">
    <img src="https://github.com/user-attachments/assets/a8a76ceb-9961-4b0b-a38a-72a49f6e56c8" width="800"/>
  </p>
- Step 13 : Sentiment analysis was done on customer feedback using python script from text analytics section resulting the report page
   <p align="center">
    <img src="https://github.com/user-attachments/assets/4ca175ff-f586-401a-92d0-888b26f28583" width="800"/>
  </p>
# Insights
Multiple page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the Report:

### Total Number of Customers = 97

   Number of satisfied Customers = 69 (27.7%)

   Number of neutral customers = 18 (18%) 

   Number of unsatisfie customers = 10 (10%) 
   
           thus, higher number of customers are satisfied.
    
 ### Policy Type
 
  Number of Customers with Travel Policy = 415 (41%)

  Number of Customers with Health Policy = 182 (18%)

  Number of Customers with Auto Policy = 172 (17%)

  Number of Customers with Life Policy = 122 (12%)

  Number of Customers with Home Policy = 109 (10%)

           thus, higher number of customers using Travel policy

### Claims by Age Group

   Claim by Adult is 8.8M

   claim by Elder is 6.4M

   claim by Young Adult is 1.7M

         thus, the higher number of claims were by Adults

    
