# Project Description

## Power BI Project: Call Centre Trends Analysis
This Power BI project focuses on analyzing a detailed call center dataset, which includes features such as Call ID, Agent, Date, Time, Topic, Answered (Y/N), Resolved, Speed of Answer (seconds), Average Talk Duration, and Satisfaction Rating. The objective is to extract meaningful insights into call center performance, customer satisfaction, and emerging trends.

## Problem statemnet 
In this project Create a dashboard in Power BI for the call center manager that reflects all relevant Key Performance Indicators (KPIs) and metrics in the dataset.

Possible KPIs include (but not limited to):

- Overall customer satisfaction.
- Overall calls answered/abandoned.
- Calls by time.
- Average speed of answer.
- Agent’s performance quadrant -> average handle time (talk duration) vs calls answered.

## Datasource :
  Dataset used for this task was presented by [Pwc](https://www.pwc.in/) and call centre trends dataset:

  Dataset: Call Centre Trends

## Data Preparation:
   Completed the Data transformation in Power Query and the dataset loaded into Microsoft Power BI Desktop for modeling.

   Call Centre Trends dataset is give table named:

     - Call Center trends dataset which has 10 columns and 5000 rows of observation.

   Data Cleaning for the dataset was done in the power query editor as follows:

    - Removed Unnecessary columns.
    - Removed Unnecessary rows.
    - Each of the columns in the table were validated to have the correct data type.

## Data Modeling:

- The call centre table as show below

![Screenshot 2024-09-14 182052](https://github.com/user-attachments/assets/8b6bc3f1-5455-4c8d-94c4-7e49bc07515c)



## Data Analysis (DAX):

Measures used in all visualization are:

- count  of answered = CALCULATE(DISTINCTCOUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Answered (Y/N)]="y")).
- count  of resolved = CALCULATE(DISTINCTCOUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Resolved]="y")).
- Target Value Satisfaction = 4.5

  ## Data Visualization (Dashboard) :
  ###                                         call centre trend
  ![Screenshot 2024-09-14 193257](https://github.com/user-attachments/assets/39f3f26a-fe57-40a8-8452-b5cafd9716b7)

  ## Insights
  ### Overall customer satisfaction

      - Most of the satisfaction ratings from each call are 3 and 4.
      - The average satisfaction rating has decreased over the span of three months. January brought the highest satisfaction rating and march the lowest.
      - Admin support has the highest customer satisfaction compared to other topics

  ### Overall calls answered/abandoned

      - The overall call answer rate ranges between 80-81%, with January recording the highest percentage of calls answered.
      - The highest percentage of abandoned calls was recorded in February.

  ### Calls by time.
      - the month of January with the highest recorded number of calls.

  ### Average speed of answer
      - The average speed of answer in the month of march was higest

   ### Agent’s performance quadrant 

      -The average speed of answer by Joe is the highest.
      -The call resolution rate of Jim is the highest, even though the average speed of his answers is lower compared to those of Joe, Martha and Dan. The call answered by  
           him are also higher than the average number of calls answered.
      -Becky's speed of answer is the lowest among all, and her rate of calls resolved is higher. She is in the 5th position in the call resolution rate.
      -Martha has the highest speed of answered in the sec








  

  

