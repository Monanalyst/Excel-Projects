# Bike Sales Analysis

## Introduction

The dataset was downloaded from: https://github.com/AlexTheAnalyst/Excel-Tutorial/blob/main/Excel%20Project%20Dataset.xlsx. This dataset included 1,027 rows (including the headers) and 13 columns.

After opening the file and converting it from a CSV format to an Excel Workbook, I resaved the file in the new format and began the process of analysis. I also made another copy in an Excel Workbook just for raw data purposes in the event of any errors, as a precautionary measure. The process to complete this project included data cleaning, pivoting and creating the visualisation report.

## Data Cleaning

**1. Remove Duplicates**

I highlighted and selected the entire table, then clicked on the Data tab and identified the remove duplicates ribbon. After identifying and removing a total of 26 duplicates, the dataset was ready for analysis. 

The presence of duplicates in a dataset can lead to inaccurate or misleading results, so it is essential to identify and remove them before performing any analysis.

Duplicates can bias the results of the analysis and lead to incorrect or misleading conclusions. It is therefore essential to identify and remove duplicates from a dataset before performing any analysis, in order to ensure the accuracy of the results.

**2. Find and Replace**

I standardised the records in the ‘Martial Status’ field by replacing ‘M’ and ‘S’ with ‘Married’ and ‘Single’ respectively, using the ‘Find and Replace’ shortcut ‘CTRL+H’. Similarly, I also replaced the ‘M’ and ‘F’ in the ‘Gender’ field with ‘Male’ and ‘Female’. This was done to ensure consistency and accuracy of the records and so that the report is easy to interpret, even for those who are unfamiliar with the abbreviations.

**3. Currency**

To ensure accurate and consistent reporting, I converted the data type for the 'Income' field from 'General' to 'Currency', and removed any decimal places. The '$' symbol was also added to indicate that it is a monetary value.

**4. Age**

To ensure that the data was useful for data analysis and visualisation purposes, I grouped the 'Age' column into three distinct categories: Adolescent (under 31), Middle-age (31-54) and Old (55 and above). To create these age brackets, I used nested IF statements in the formula and added a new column named 'Age Brackets' for the purpose of visualisation. Also just make sure that if the value did not meet any of the age requirements then it would display ‘Invalid’.

=IF(L2>54,"Old",IF(L2>=31,"Middle Age",IF(L2<31,"Adolescent","Invalid")))

## Pivot Table/Chart Findings

**1. Customer Commute**

The data shows that shorter distances increase the likelihood of people purchasing bikes for commuting, likely due to the convenience of having a bike available and the cost-effectiveness of riding a bike instead of taking public transport or driving. This implies that the bike company should focus their marketing efforts on people who live close to their destination and offer them special deals for commuting purposes.

**2. Average Income per Purchase**

The data shows that people with higher incomes are more likely to make a bike purchase, regardless of gender. The average income for males who made a purchase was $60,124, compared to $56,208 for those who did not. Similarly, the average income for females who made a purchase was $55,774, compared to $55,440 for those who did not. Also, the data suggests that there is a gender income gap, with males earning around $4,400 more than females on average. This could be an important factor to consider when marketing bike products.

**3. Purchase per Age Bracket**

The data shows that people in the middle age bracket (31-54) are the most likely to purchase a bike, while people aged 55 and above (old) and adolescents (under 31) are less likely to do so. The reason for this could be because people in the middle age bracket are more likely to have the financial resources to purchase a bike and the physical fitness to use it regularly. Adolescent may not have the financial means to purchase a bike, or may not feel the need for a bike at this stage in their life.

**4. Purchase per Cars Owned** 

The data shows that people who are not car owners or own fewer cars are more likely to purchase a bike, while people who own more cars are less likely to do so. This could be because bikes are cheaper to maintain than cars and it also can be used as a way of keeping fit. As mentioned before in relation to commuting, people with fewer or no cars may be more likely to purchase a bike because it is often more cost-effective than taking public transport or driving. 

**5. Purchase per Children**

The data shows that people who have fewer or no children are more likely to purchase a bike, while people who have more children are less likely to do so. This could be because people with fewer or no children may have more financial resources to purchase a bike and may be able to use it more frequently. Also, people with more children may have their financial priorities set elsewhere, as well as with the time and responsibility focused on raising their children.

## Conclusion

The analysis of the 5 visualisations suggests that middle-aged (31-54), Non-car owners/those with 1 or 2 cars, and those with less than 3 children/no children are the most likely to purchase a bike. The bike company should target their marketing campaigns towards these demographics, offering discounts and promotions to make their product more appealing and encourage more people to switch to cycling. 

## Visualisation

A thorough analysis of this dataset was conducted using the most appropriate charts and colours to accurately depict its information. The charts were carefully selected to ensure that they were engaging and visually appealing, providing an effective way to present the data.

![Bike Sales Report](https://user-images.githubusercontent.com/123024674/213875593-6a4fd336-ca31-40a5-99e5-bfda6d0a00e8.png)
