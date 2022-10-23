# Health_Spending_Life_Expectancy_Project
Exploring Healthcare Spending and Life Expectancy from the Seaborn Library
Final Presentation Slide Deck - https://docs.google.com/presentation/d/1jZlISbB6kHrOysYU48LAX4Di7fPVhzuo1_TSL0y5Crk/edit?usp=sharing

Coded and visualized with Python in JuptyerLabs

## Importing Libraries & Data
The Health Spending and Life Expectancy data is a dataset already inside the seaborn library. To explore this dataset I imported the pandas, NumPy, Matplotlib and seaborn library into JupyterLab. 

## Exploration Process and Conclusions
After importing the data frame, I examined the dataset by looking at the beginning and end of the data using .head and .tail. I also checked for any nulls or duplicates with the dataframe. 

### *How has life expectancy changed over time?* 
I created a line plot graphing the individual country's average life expectancy between 1970 to 2020. I found that life expectancy has generally increased over time. 

### *How has healthcare spending changed over time?*
I created a line plot graphing the individual country's healthcare spending between 1970 to 2020. I found that spending has increased over time as well.

### *Is there a relationship between spending and life expectancy?*
I created a scatterplot with spending on the x-axis and life expectancy on the y-axis. It appeared that there was a positive correlation between spending and life expectancy. To confirm this, I calculated the overall correlation between the two variables and found that there was a moderate correlation between spending and life expectancy, r = .579. 

This correlation seemed relatively low, so I decided to look at each country's correlation individually. To do this, I created a function which used the country's name as a parameter to calculate correlation. I found that all countries had a strong correlation between spending and life expectancy, with r values over 0.9. France had the strongest correlation between the two variables, r = 0.969, while the USA had the least strongest correlation of r = 0.907. 

### *What was the minimum, median and maximum life expectancy per country?*
I used a pivot table to determine the min, median and max for life expectancy. I found that the USA had the lowest maximum life expectancy at 78.9 years old, while Japan had the highest maximum of 84.7 years old. I thought the USA maximum life expectancy was relatively low compared to the other countries, so I decided to communicate that point by creating a boxplot showing life expectancy, and drawing a red line on top of the USA's maximum life expectancy. This showed that the USA's max was lower than the median life expectancy of France and Japan. 

