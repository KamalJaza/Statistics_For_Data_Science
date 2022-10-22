# Statistics-for-Data-Science
# Type of Statistics
-	Descriptive Statistics
-	Inferential Statistics
# Descriptive Statistics
Organizing, summarizing, and presenting data in an informative way
-	Measure of Central Tendency
-	Measure of Spread / Dispersion
-	Skewness
-	Correlation
# Measure of Centrak Tendency
### Mean
Mean represents the average of the given collection of data. It is applicable for both continuous and discrete data.
•	All scores in distribution affected the mean
•	Many samples from the same population will have similar means
•	The mean will change if we add extreme value
### Median
Median represents the mid-value of the given set of data when arranged in a particular order.
•	Doesn't change much by extreme values (outliers).
•	Median is a robust statistics.
### Modus
The most frequent number occurring in the data set is known as the mode.
# Measure of Spread / Dispersion
### Range
It is simply the difference between the maximum value and the minimum value given in a data set.
### Variance
-	Variance is the expected value of the squared variation of a random variable from its mean value, in probability and statistics.
-	Informally, variance estimates how far a set of numbers (random) are spread out from their mean value.
### Standard Deviation
The standard deviation is a measure of the amount of variation or dispersion of a set of values.
-	A low standard deviation indicates that the values tend to be close to the mean of the set.
-	While a high standard deviation indicates that the values are spread out over a wider range.



## Outliers and Missing Value
### Check Outliers using Boxplot
- A box plot is a good way to show many important features of quantitative (numerical) data.
- It shows the median of the data. This is the middle value of the data and one type of an average value.
- It also shows the range and the quartiles of the data. This tells us something about how spread out the data is.

### Check Outliers using IQR
IQR tells how spread the middle values are. It can be used to tell when a value is too far from the middle. 
An outlier is a point which falls more than 1.5 times the interquartile range above the third quartile or below the first quartile. 
- Step 1: Arrange the data in incresing order
- Step 2: Calculate first (q1) and third quartile (q3) 
- Step 3: find interquartile range (q3-q1)
- Step 4: Find lower bound (q1*1.5)
- Step 5: Find upper bound (q3*1.5)
Anything that lies outside of lower and upper bound is an outlier

#Handling Outliers
One of the simplest way to handle outliers is to just remove them from the data or . If you believe that the outliers in the dataset are because of errors during the data collection process then you should remove it or replace it with NaN.

### Handling missing value
Missing values are usually represented in the form of Nan or null or None in the dataset.
In this case, we will be filling the missing values with a certain number. The possible ways to do this are:
- Filling the missing data with the mean or median value if it’s a numerical variable.
- Filling the missing data with mode if it’s a categorical value.
- Filling the numerical value with 0 or -999, or some other number that will not occur in the data. This can be done so that the machine can recognize that the data is not real or is different.
- Filling the categorical value with a new type for the missing values.
You can use the fillna() function to fill the null values in the dataset.
