# cyclistic_bikeshare_case_study
Case study for the Coursera Google Data Analytics Capstone by Aidan Doyle

Introduction
 
I recently completed the Google Data Analytics Professional Certificate through Coursera. At the end of the course, I was tasked with completing a capstone case study. I elected to complete data analysis for the fictional bike-share company Cyclistic. The course outlined six steps that were crucial to completing a data analysis case study: ask, prepare, process, analyze, share, and act. 

Background

In this case study, I am a junior data analyst working on the marketing analyst team at Cyclistic, a fictional bike-share company based in Chicago. The company was launched in 2016 and possesses 5,824 bikes across 692 stations. These bikes can be unlocked from any station and do not need to be returned to the same station. Cyclistic has 3 types of passes available to its users, resulting in two types of riders. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers who purchase annual memberships are Cyclstic members. Financial analysts at Cyclistic have concluded that annual members are more profitable than casual members. 

Ask

Three questions will guide the future marketing program: 
1. How do annual members and casual riders use Cyclistic bikes differently? 
2. Why would casual riders buy Cyclistic annual memberships? 
3. How can Cyclistic use digital media to influence casual riders to become members? 
To reiterate, I am tasked with question 1 in this case study. 

Prepare

To complete this task, I will be using the previous 12 months of Cyclistic bike-share data made available [here](https://divvy-tripdata.s3.amazonaws.com/index.html). 

The data has been made available by Motivate International Inc. through this [license](https://divvybikes.com/data-license-agreement).   

Process

I compiled data from April 2025 to March 2026 and used SQL through Google’s BigQuery (since it was used throughout the Data Analysis course) to process and analyze the data through 4 steps: Data combining, data exploration, data cleaning, and data analysis. 


The director of marketing, my manager, believes that maximizing the number of annual members will lead to growth. Instead of appealing to new customers, she believes converting casual riders to annual members will be the most effective since they are already familiar with the company. To do this, the team needs to understand how annual members and casual riders differ, why casual members would buy a membership, and how digital media could be used in marketing tactics. So, that is where I, the data analyst, come in. I am tasked with the first part of that equation. 

Analyze

The analyze step of this case study consists of data combining, data exploration, data cleaning, and data analysis. The code that I created in SQL for these steps will be attached below. 

[Data Combining](https://github.com/putitinreverseterry/cyclistic_bikeshare_case_study/blob/main/Data_Combining)
[Data Exploration](https://github.com/putitinreverseterry/cyclistic_bikeshare_case_study/blob/main/Data_Exploration)
[Data Cleaning](https://github.com/putitinreverseterry/cyclistic_bikeshare_case_study/blob/main/Data_Cleaning)
[Data Analysis](https://github.com/putitinreverseterry/cyclistic_bikeshare_case_study/blob/main/Data_Analysis)

Data Combining

The data from the twelve months were combined into a single table that yielded 13 columns of data and 5,620,544 rows. 

Data Exploration

The data was queried to reveal null values, duplicates, rider types, rideable bike type, and any discrepancies in ride ID

Data Cleaning

The data was cleaned, creating a new table that removed duplicates, nulls, and created rows for day of the week, month, and ride length. Furthermore, rides that lasted less than a minute or longer than a day were excluded from the cleaned data. In the data cleaning step, 1,915,868 rows were removed, leaving 3,704,676 rows for analysis. 

Data Analysis

In this step, important statistics and trends were gathered through the data via SQL queries. Counts for rider type (member casual), average ride lengths for rider type, and counts for rider type depending on month and day of the week were gathered to identify meaningful trends. 

Share

<img width="684" height="385" alt="image" src="https://github.com/user-attachments/assets/10e892d1-f88d-4fb5-bbfb-9b488389d378" />

Significant takeaways: 
1. Of the 3,704,676 rows available for analysis, 2,386,702 are members, while 1,317,974 are casual riders. Approximately 36% of Cyclistic Bikeshare riders are casual riders.
2. The average ride for a casual rider is nearly 10 minutes longer than for members (22.41 for casual riders and 12.51 for members).
3. The average ride length for members during the typical work week (Monday to Friday) is around 12 minutes. The average ride length for casual riders increases on the weekend and has the shortest ride length in the middle of the week.
4. Member ride length does not have much difference depending on the time of year, while casual rider ride length tends to be significantly longer in the warmer months (May to August).
5. Members unlock bikes at a higher rate during the week, whereas casual riders unlock bikes at a higher rate on the weekend.
6. There is a dramatic increase in ride count for casual riders during the warmer months and a steep drop-off during the colder months. The count of members decreases in the colder months as well, but not as drastically. 

Act

It is presumed that a majority of members are residents of Chicago and use Cylistic consistently. Since many Cyclistic members unlock bikes at a higher rate during the week and for a consistent ride length, we can infer that these members use Cyclistic as a commute method. Our members are aware of the reliability that Cyclistic offers. Casual riders are intrigued by the flexibility and convenience. Most of the rides by casual riders occur during the weekends and warmer months. Casual riders are more likely to unlock bikes for recreational purposes such as casual exercise or tourism. 

Suggestions
1. Offer a designated weekend membership at a lower price that allows users to unlock bikes from Friday to Sunday or Saturday to Sunday. This would allow tourists or weekend users a reliable source of transportation without the hassle of having to pay for multiple unlocks during a weekend.
2. Offer a designated summer membership that runs from Memorial Day to Labor Day (or a similar period).
3. When casual riders make an account in the app and unlock a bike a specific number of times, offer a complimentary weekend membership. This would allow casual riders to create a sense of familiarity and trust with the brand. In return, they would be offered a reward that would double as a trial period for a membership.
4. Offer a membership that allows for a free number of bike rides before the payment is processed. Riders would need to sign up with a card on file and are allowed to cancel at any time.
5. Prioritize marketing within the app. Alert casual riders of the savings of purchasing a membership based on how often they ride. This highlights the opportunity cost of not purchasing a membership.




Resources
[Aaron Hodges' case study](https://github.com/hodges0501/Google_Data_Analytics_Cyclistic_Bike_Share_Study/blob/main/README.md) 
[Hui Min's case study](https://github.com/minbean/Google-Data-Analytics-Capstone-Project-Cyclistic-Case-Study/blob/main/README.md)
