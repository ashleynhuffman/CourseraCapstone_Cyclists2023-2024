#Case Study: Cyclist \(A Google Data Analytics Professional Certificate Capstone Project\)#

*Hello and welcome! This is my capstone project for Google's Data Analytics Professional Certificate on Coursera. For this capstone I chose to work with data provided by the course on rental bike usage.*

##Scenario##

*You are a junior data analyst working on the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, your team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, your team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve your recommendations, so they must be backed up with compelling data insights and professional data visualizations.*

##Stakeholders##
**Company** Cyclistics
**Report to** Lily Moreno, Director of Marketing
**Audience** Cyclistic executive team

##ASK##
How do annual members and casual riders use Cyclistic bikes differently?
Provide a report with the following deliverables: 
    1. A clear statement of the business task 
    2. A description of all data sources used
    3. Documentation of any cleaning or manipulation of data
    4. A summary of your analysis
    5. Supporting visualizations and key findings
    6. Your top three recommendations based on your analysis

##Prepare##
The capstone assignment provided a link to the company's ride history, found [here](https://divvy-tripdata.s3.amazonaws.com/index.html) I downloaded the data from May 2023 to April 2024.

##Process##
I first opened each of the 12 speadsheets and created a column called ride_length. Then used a function to calculated the ride length by subtracting the started_at from the ended_at columns. I created a day_of_week column and populated the rows by using the WEEKDAY function. 
I then cleaned the data by removing duplicates and unnecessary columns. 
The remaining columns are as listed:
    +rideable_type
    +started_at
    +ended_at
    +member_casual
    +ride_length
    +day_of_week
After calculating the ride length, I noticed I was getting an error for some rows due to the started_at and ended_at data was transposed. To correct this, I sorted the ride_length column so it grouped all of the '\#\#\#' results. This enabled me to quickly correct the data by selecting the range and drag the cells to the desired column while holding shift.