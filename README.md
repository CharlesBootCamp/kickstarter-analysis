# kickstarter-analysis
Challenge 1 working with the Kickstarter Challenge to create varying line charts of the data
# Kickstarting with Excel

## Overview of Project
 Using the already given data, I created charts that display how the Kickstarter data gets used based on the goals of the Kickstarters and the launch dates. This project then takes the given data and uses it to produce two line charts, one comparing successful, failed, and canceled theater acts over the months/years, and the other comparing how many acts with varying financial goals did, as well as the percentages of success/failure.
### Purpose
The purpose of this project is to compare multiple Kickstarter campaigns based on both their launch date and their finance goals, as well as whether or not they were able to accomplish said goals. This project was done to be able to make sure that I am able to search for/use specific parts of the data to create charts that display the required data.
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
![image](https://user-images.githubusercontent.com/108377724/177893108-c7c3dca4-af54-41ca-9db2-826941bf04d7.png)
I had to create the Date Created Conversion using the launched_at column using the equation =(((J2/60)/60)/24)+DATE(1970,1,1) to satisfy that the date started January, 1, 1970 and the launced_at column is the number of seconds since then, making it so that the Years column can be created to use for the Years filter and the month row labels. The graph y-axis displays the number of each individual type of outcome; success, failure, and canceled, displaying a graph that shows how each type changed over the months, which is the x-axis. The graph was then calibrated to display only theater outcomes.
### Analysis of Outcomes Based on Goals
![image](https://user-images.githubusercontent.com/108377724/177898351-280e2d8f-dae5-4514-abf3-e21d0c4c9e14.png)
I had to create multiple columns, listing the financial goal amount in intervals of $5,000 after the first $1000 one, the number of successful projects, the number of failed projects, the number of canceled projects, the total number of projects, as well as the percentages for success, failure, and canceled projects. To calculate the number of each kind of goal, I had to use the COUNTIF function to distinguish between the different financial amounts, whether they were successes/failures, and only including those done for plays. The number of canceled projects that were plays in total were in 0, splitting the numbers exclusively between success/failure. These values were then used to determine the total amount per threshold, then, by dividing each section by the total amount and multiplying by 100, the percentage is then found for each project type.


### Challenges and Difficulties Encountered
One challenge I had to deal with with the Outcomes Based on Launch Date problem was trying to figure out how to create the Date Created Conversion equation to find the year each play came out. A challenge I had with the Outcomes Based on Goals was I had forgotten that I needed to limit the number of successful, failed, and canceled projects, so my graph appeared off. A second challenge was making the intervals of data work over the appropriate area they are supposed to.
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

 The first conclusion is that there were more successes than failures and cancellations. A second conclusion is that there was never a time where the number of failures was greater than the number of successes in the theater.
 
- What can you conclude about the Outcomes based on Goals?

There were no canceled plays, as well as swapping between whether there were more successes or failures.

- What are some limitations of this dataset?

This dataset doesn't take into account location further than the country, due to countries have varying areas with different cultures, this could definitely alter the potential for a success or failure. 

- What are some other possible tables and/or graphs that we could create?

We can also create bar charts comparing the country with the amount of financial backing to see what countries give what, as well as another line chart to compare the number of backers with the amount that has been pledged.
