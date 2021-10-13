# Exploratory Data Analysis with Pandas
The aim of this presentation is to explain the Exploratory Data Analysis process with Pandas to the students of the MSDS program and demonstrate the same through real world example. We also discuss the importance of Data Vizualizatin which is a key componenent in EDA to make the process streamline and easily analyze data using wonderful plots and charts.


> Exploratory data analysis is an attitude, a state of flexibility, a willingness to look for those things that we believe are not there, as well as the things we believe might be there - John Tukey, as quoted in “Nonparametric statistical data modeling: comment.” J Am Stat Assoc 1979, 74, 121-122.

## Definition
It is the process of analyzing, learning useful information, and formulating new questions about a population based on the dataset at hand. In EDA, we use a combination of libraries; Pandas is one of them which is used for manipulating the data and it is open-source. 

## Common Steps in EDA
1. We first start with loading the data into a pandas data frame.
2. Initially, we check the shape of data which gives us the number of rows and columns in our data frame. 
3. We check the data types of columns and ensure that they are of the correct type.
4. In case the column names are confusing, we rename them to improve the readability of the dataset.
5. Most of the time, datasets have missing values; therefore, it is necessary to check null values and inspect the possible reasons why those values are missing. 
6.  It is also important to ensure that numeric features are scaled and normalized so that they contribute proportionally to the ML algorithms at the time of     fitting data. Additionally, we also process our categorical variables and encode them.

### Data Visualization
It is an important part of EDA and we extensively plot data points to visually understand our data better. 
1. Boxplots and scatterplots are used to detect outliers in the dataset 
2. We use histogram plots to check the distribution of our numeric features which basically gives the frequency of variables in an interval.
3. Oftentimes, we want to check how numeric features behave with each other; in this regard, scatter plots are used to determine relationships between them. 

## Data
We have used the [House Prices](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) dataset from Kaggle. The dataset consists of possible features that might impact the sale price of the house. 

## Libraries Used:
1. Numpy: Used for processing multidimensional array objects and a collection of routines .
2. Pandas: Used for data manipulation and analysis.
3. Scipy: Used for calculating basic statistics
4. Matplotlib and Seaborn: USed for data vizualization 



