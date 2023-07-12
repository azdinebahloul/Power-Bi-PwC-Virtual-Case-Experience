# Power Bi-PwC-Virtual-Case-Experince
## Introduction
Welcome to the PwC Switzerland Power BI Virtual Case Internship! This internship project focuses on leveraging the power of Microsoft Power BI for data analysis and visualization. Our goal is to create a comprehensive dashboard that provides valuable insights and facilitates informed decision-making.

Throughout this internship, we will explore various aspects of data analysis using Power BI. From connecting and transforming data to designing interactive visualizations, we will learn how to effectively present complex information in a meaningful way.

Join me on this exciting journey as we dive into the world of data analytics, harness the capabilities of Power BI, and unlock the potential of data-driven insights. Get ready to make an impact and enhance your skills in the realm of business intelligence and visualization."

## Data Preparation
Before diving into data analysis using Power BI, it is essential to perform data preparation tasks. Initially, the data provided by PwC had a specific format :

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/raw/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20181850.png" alt="Image1" width="50%">
</p>


During the data preparation phase, we will clean and transform the data using Power Query as necessary. For example, we will extract call duration without its associated date and introduce a new category for answered calls. Additionally, we will create a conditional column based on customer ratings to assign a descriptive text to each rating. These steps are essential in ensuring that our data is in a suitable format for analysis in Power BI.

## Call Center Analysis 
The goal is to design a visually appealing and user-friendly dashboard that effectively communicates the relevant information to Claire. Unleashing my creativity and thinking outside the box has allowed me to develop compelling visualizations that showcase the data in an impactful way.

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Screen%20Shot%202021-06-15%20at%205.23.06%20PM.png" alt="Image2" width="50%">
</p>

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

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20185434.png" alt="Image3" width="50%">
</p>

We repeated the process until having all our measures of interest:

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20185629.png" alt="Image4" width="50%">
</p>

### Data Visualization
After creating our measures, we proceeded to design the visualizations that we deemed most relevant for the analysis.

#### Calls by Date

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20190353.png" alt="Image5" width="50%">
</p>

1. Constructed a **line chart** visualization.
2. Utilized the **Date** column as input for the X-axis, representing the **timeline**.
3. Used the **Call ID** column as input for the Y-axis, displaying the **count of Call IDs** over time.

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20190635.png" alt="Image6" width="50%">
</p>

> 💡For all our visualizations, we have chosen to maintain consistency with PwC by primarily using a grayscale background and incorporating the company's official colors. The PricewaterhouseCoopers (PWC) logo colors include Black (#000000), Rufous (#AD1B02), Tenné (Tawny) (#D85604), Beer (#E88D14), Orange-Yellow (#F3BE26), and China Pink (#E669A2) (Source: The PricewaterhouseCoopers (PWC) Logo Colors with Hex & RGB Codes, April 4, 2020)

#### Average Customer Satisfaction
To create the visual, I utilized three measures that were previously created for the ratings: Overall Customer Satisfaction Rating, Min rating, and Max rating.

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20191549.png" alt="Image7" width="50%">
</p>

Using these measures, I built the visual with a gauge chart, following these steps:

1. Set the **Overall Customer Rating** measure as the input for the "Value" parameter to display the **average rating**.
2. Use **Min rating** as the input for the "Minimum Value" parameter to represent the **minimum rating**.
3. Use **Max rating** for the "Maximum Value" parameter to showcase the **maximum rating**.
   
<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20192308.png" alt="Image8" width="50%">
</p>

#### Number of Call by Topic
Now to display the number of calls per topic, I decided to create a grouped bar chart.

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20192524.png" alt="Image9" width="50%">
</p>

1. Build visual with **grouped bar chart** (Horizontal)
2. Input **Topic** column into Y-axis 
3. Input **Call id** column into X-axis as **Count of call id**

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20192906.png" alt="Image10" width="50%">
</p>

#### Call Satisfaction
Using our new created column Satisfaction, we followed the same process as the previous chart to display the result in a beatiful grouped bar chart:

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20193343.png" alt="Image11" width="50%">
</p>

1. Build visual with **grouped bar chart** (Horizontal)
2. Input **Satisfaction** column into Y-axis 
3. Input **Call id** column into X-axis as **Count of call id**

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20193318.png" alt="Image12" width="50%">
</p>

#### Call Resolved 
Then, we visualized the number of resolved and unresolved calls using a pie chart, effectively representing the distribution between the two categories.

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20195942.png" alt="Image13" width="50%">
</p>

1. Build visual with **pie chart**
2. Input **Resolved** column into Legend
3. Input **Call id** column into **Valuesb** as **Count of Call id**
4. Input **Resolved** column into Details

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20200325.png" alt="Image14" width="50%">
</p>

#### Agent & Date Slicer
Lastly, we added two slicers to our dashboard, enabling us to filter the data based on date and individual agents. This allows us to analyze the data based on specific time periods and examine the performance of each agent individually.

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20195706.png" alt="Image15" width="50%">
</p>

### Dashboard
That concludes the Call Center Trends Analysis. Below is the comprehensive dashboard representing the complete analysis of Call Center Trends.

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20202301.png" alt="Image16" width="50%">
</p>

## Customer Churn Analysis

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20145247.png" alt="Image17" width="50%">
</p>

## Diversity & Inclusion Analysis

<p align="center">
  <img src="https://github.com/azdinebahloul/Power-Bi-PwC-Virtual-Case-Experience/blob/main/Screenshots/Capture%20d'%C3%A9cran%202023-06-23%20162413.png" alt="Image18" width="50%">
</p>


