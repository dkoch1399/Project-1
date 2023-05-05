# Project-1

- Imported the required Python libraries, Pandas and Pathlib.
- Defined the file paths for two CSV files using the Path function from Pathlib.
- Loaded the data from the CSV files into two separate data frames using the read_csv function from Pandas.
- Printed the column names of both data frames using the .columns attribute.

- Merged two Pandas data frames, "air_data" and "ev_sales", into a new data frame named "ev_data_complete"
- The merge is based on two common columns in both data frames, "county" and "year".
- The how parameter is set to "left", which means that the merge operation will keep all rows from the left data frame ("air_data"), and only add matching rows from the right data frame ("ev_sales").

- Unnamed: 3 column was dropped from the data

- Calculated the total numbers of unique years, counties and cities in the dataset
- Calculated the total vehicles by year 

- Grouped the rows in the "ev_data_complete" data frame by the "year" column using the groupby() function.

- Calculated the mean value for the "no2 avg", "no2 aqi", "ozone avg", and "ozone aqi" columns for each group using the agg() function.
- Calculated the sum of the "Number of Vehicles" values for each group using the agg() function.

- Created a new data frame that shows the mean "no2 avg", "no2 aqi", "ozone avg", and "ozone aqi" values, as well as the sum of "Number of Vehicles" values, for each year in the original data frame.

- Calculated the mean values of several columns in the "ev_data_complete" data frame, grouped by both "year" and "county".

- Created a bar graph displaying the NO2 Average per County

- Created a line graph displaying the NO2 Average per County over time

- Created a bar graph displaying the Ozone Average per County

- Created a line graph displaying the Average Ozone levels by County over Time

- Created a bar graph displaying the number of Vehicles per Year

- Created a bar graph displaying the NO2 Average per Year

- Created a regression line displaying the NO2 Average per Year

- Created a bar graph displaying the Ozone Average per Year

- Created a regression line displaying the Ozone Average per Year

NO2 concentrations did not increase over time in the five counties in California represented in the table.

The average concentrations of NO2 decreased from 2018 to 2022 in all five counties. 

For example, in Alameda, the NO2 concentration decreased from 10.92 in 2018 to 8.86 in 2022. 

Similarly, in Los Angeles, the NO2 concentration decreased from 13.67 in 2018 to 12.44 in 2022.

The r-value of -0.6923 in the NO2  vs Year linear regression has  a moderate negative correlation, which suggests that  NO2 has slightly decreased over time, at the same time that vehicle population increases

Ozone levels in these counties fluctuated over the years, with some counties consistently having higher  levels than others. 

The r-value of 0.8807 in the Ozone vs Year linear regression has a strong positive correlation, which suggest that the ozone levels have increased over time.

Air pollutants interactions are very complex and other factors, such as weather conditions, can also impact ozone levels. 

Overall, it appears that the average NO2 levels have decreased slightly over time in these counties. In contrast, ozone levels have increased over time.


