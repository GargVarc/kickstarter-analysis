# Kickstarter-analysis
#### Performing analysis on Kickstarter data to uncover trends

### Overview

In this analaysis, the kickstarter dataset is analysed to determine how different campaigns fared in relation to their launch dates and their funding goals. Using the kickstarter dataset, campaign outcomes are visualized based on their launch dates and their funding goals. 

### Tools Used

  - MS Excel (Pivot Tables & Pivot Charts)
  - Git Bash

### Resources

  - Kickstarter Dataset


### Analysis and Challenges

  #### Outcomes Based on Launch Date
  
  - "Years" column created based on the "Date Created Conversion" column
  
    ![D1_1](https://user-images.githubusercontent.com/106279653/193475960-edd5af37-e32d-440e-a533-eaa2ef7610f0.JPG)

  - Pivot table created in a new worksheet

  ![D1_2](https://user-images.githubusercontent.com/106279653/193475984-e8c89c84-f9cd-4119-a60a-7b7cbd266340.JPG)

  - "Parent Category" filtered on "theater"
  
  - Row labels changed to display months of the year and campaign outcomes sorted in descending order.
  
  - Line chart created showing the number of successful, failed, or canceled projects by month.
  
  ![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/106279653/193476063-9f982737-a2cd-4544-8e9c-f231e074ab0b.png)
  
  
  #### Outcomes Based on Goals Chart
  
  - A new worksheet is created and populated using COUNTIFS function with "Number Successful", "Number Failed", and "Number Canceled" columns based on the project "outcome", the "goal" amount and the Subcategory "plays"
  
  - SUM() function is used on each row to add the "Number Successful", "Number Failed", and "Number Canceled" columns and populate the "Total Projects" column.
  
  - Percentages of successful, failed, and canceled projects are calculated based on the data from the "Total Projects", "Number Successful", "Number Failed", and "Number Canceled" columns.

  ![D2_1](https://user-images.githubusercontent.com/106279653/193476334-53ee8676-2e89-4031-8451-bf743b83eb78.JPG)

  - A line chart is created with goal-amount ranges on the x-axis, and the percentages of successful, failed, or canceled projects on the y-axis.
  
  ![Outcomes_vs_Goals](https://user-images.githubusercontent.com/106279653/193476343-e34facd2-ec68-416e-b6fa-48d31cd74d5c.png)


### Results

  - Conclusions based on Theater Outcomes by Launch Date
    - The number of successful projects is highest for the months of May and June
    - The number of failed projects is highest for the months of May, July and October.
   
   - Conclusions for Outcomes based on Goals   
      - The percentage of successful campaigns out of the total projects is highest for projects with goals upto $5000.
      - The percentage of failed campaigns out of the total projects is highest for projects with goals between $25,000-$30,000 and for goals over $50,000
   
   
  - Limitations of this dataset

    - In case of Oucomes based on Goals more than 19999 the data is very limited.
    - In this method, the conclusion is limited to X-Y model, hence unable to add multiple variables at the same time.

  - Some other possible tables and/or graphs
  
    - Creating a pie chart to display percentage of outcomes in relation to countries in case of Outcomes based on Launch Date.
    - Creating another pie chart to visulaize Percentage of Successful, Failed & Canceled w.r.t. the goal outcomes.
  
    
