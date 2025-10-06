# Insurance_Performance_Sentiment
# Insurance Perfomance-Dashboard

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

Following inferences can be drawn from the dashboard;

### [1] Total Number of Customers = 129880

   Number of satisfied Customers (Male) = 28159 (21.68 %)

   Number of satisfied Customers (Female) = 28269 (21.76 %)

   Number of neutral/unsatisfied customers (Male) = 35822 (27.58 

   Number of neutral/unsatisfied customers (Female) = 37630 (28.97 %)


           thus, higher number of customers are neutral/unsatisfied.
           
### [2] Average Ratings

    a) Baggage Handling - 3.63/5
    b) Check-in Service - 3.31/5
    c) Cleanliness - 3.29/5
    d) Ease of online booking - 2.88/5
    e) Food & Drink - 3.21/5
    f) In-flight Entertainment - 3.36/5
    g) In-flight service - 3.64/5
    h) In-flight Wifi service - 2.81/5
    i) Leg room service - 3.37/5
    j) On-board service - 3.38/5
    k) Online boarding - 3.33/5
    l) Seat comfort - 3.44/5
    m) Departure & arrival convenience - 3.22/5
  
  while calculating average rating, null values have been ignored as they were not relevant for some customers. 
  
  These ratings will change if different visual filters will be applied.  
  
  ### [3] Average Delay 
  
      a) Average delay in arrival(minutes) - 15.09
      b) Average delay in departure(minutes) - 14.71
Average delay will change if different visual filters will be applied.

 ### [4] Some other insights
 
 ### Class
 
 1.1) 47.87 % customers travelled by Business class.
 
 1.2) 44.89 % customers travelled by Economy class.
 
 1.3) 7.25 % customers travelled by Economy plus class.
 
         thus, maximum customers travelled by Business class.
 
 ### Age Group
 
 2.1)  21.69 % customers belong to '0-25' age group.
 
 2.2)  52.44 % customers belong to '25-50' age group.
 
 2.3)  25.57 % customers belong to '50-75' age group.
 
 2.4)  0.31 % customers belong to '75-100' age group.
 
         thus, maximum customers belong to '25-50' age group.
         
### Customer Type

3.1) 18.31 % customers have customer type 'First time'.

3.2) 81.69 % customers have customer type 'returning'.
       
       thus, more customers have customer type 'returning'.

### Type of travel

4.1) 69.06 % customers have travel type 'Business'.

4.2) 30.94 % customers have travel type 'Personal'.

        thus, more customers have travel type 'Business'.
