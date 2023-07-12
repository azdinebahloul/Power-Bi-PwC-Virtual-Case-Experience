# Power Bi-PwC-Virtual-Case-Experince
## Introduction
Welcome to the PwC Switzerland Power BI Virtual Case Internship! This internship project focuses on leveraging the power of Microsoft Power BI for data analysis and visualization. Our goal is to create a comprehensive dashboard that provides valuable insights and facilitates informed decision-making.

Throughout this internship, we will explore various aspects of data analysis using Power BI. From connecting and transforming data to designing interactive visualizations, we will learn how to effectively present complex information in a meaningful way.

Join me on this exciting journey as we dive into the world of data analytics, harness the capabilities of Power BI, and unlock the potential of data-driven insights. Get ready to make an impact and enhance your skills in the realm of business intelligence and visualization."

## Data Preparation
Before diving into data analysis using Power BI, it is essential to perform data preparation tasks. Initially, the data provided by PwC had a specific format :

![Image1](https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20181850.png)

During the data preparation phase, we will clean and transform the data using Power Query as necessary. For example, we will extract call duration without its associated date and introduce a new category for answered calls. Additionally, we will create a conditional column based on customer ratings to assign a descriptive text to each rating. These steps are essential in ensuring that our data is in a suitable format for analysis in Power BI.

## Call Center Analysis 
The goal is to design a visually appealing and user-friendly dashboard that effectively communicates the relevant information to Claire. Unleashing my creativity and thinking outside the box has allowed me to develop compelling visualizations that showcase the data in an impactful way.

![Image2](https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Screen%20Shot%202021-06-15%20at%205.23.06%20PM.png)

As we embark on this journey, we will prioritize the following KPIs (but not limited to) to guide our dashboard design:

1. Overall customer satisfaction: Analyzing customer feedback and ratings to gauge the satisfaction level of Claire's clients.
2. Overall calls answered/abandoned: Tracking the number of calls handled by the customer service team and identifying any abandoned calls.
3. Calls by time: Visualizing call volumes based on different time segments, such as hourly, daily, or monthly breakdowns.
4. Average speed of answer: Calculating the average time it takes for a call to be answered by the customer service team.
5. Agent's performance quadrant: Comparing the average handle time (talk duration) and the number of calls answered to assess the performance of individual agents.

Remember, these KPIs are just a starting point. We can explore additional metrics and dimensions that could provide valuable insights for Claire's business.

Let's tap into the power of Power BI and create a dynamic dashboard that showcases the KPIs and metrics, enabling Claire to make informed decisions and drive her business forward. Get ready to dive in and unleash your creativity!

> :bulb: The following steps outline the key points for creating the chart in Task 1, focusing on essential aspects rather than general design elements like fonts, colors, backgrounds, and legends. Please note that these step-by-step instructions are provided as an example specific to Task 1, which involves creating a dashboard.

### Creation of Essential Measures for KPI Analysis
After cleaning and preparing our data using Power Query, we decided to start by creating all the metrics we felt were relevant for our analysis.

For example, leveraging our new column "CallsDuration," we created a measure to calculate the average call duration by utilizing the following DAX formula:

![Image3](https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20184804.png)

