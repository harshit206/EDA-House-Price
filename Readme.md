# Exploratory Data Analysis with Pandas
This presentation aims to explain the Exploratory Data Analysis process with Pandas to the students of the MSDS program and demonstrate the same through a real-world case study. We also discuss the importance of Data Visualization which is a key component in EDA. It helps in analyzing the data using wonderful plots and charts.

![EDA](https://github.com/harshit206/EDA-House-Price/blob/main/plots/263-2637092_data-analytics-exploratory-data-analysis-icon.png)


> Exploratory data analysis is an attitude, a state of flexibility, a willingness to look for those things that we believe are not there, as well as the things we believe might be there - John Tukey.

## Definition
It is the process of analyzing, learning useful information, and formulating new questions about a population based on the dataset at hand. In EDA, we use a combination of libraries; Pandas is one of them which is used for manipulating the data and it is open-source. 

## Project Description
We have performed Exploratory Data Analysis to gain insights on how various factors affect the sale price of a house through data visualization and basic statistics.

## Data
We have used the [House Prices](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) dataset from Kaggle. The dataset consists of possible features that might impact the sale price of the house. 

## Libraries Used:
1. Numpy: Used for processing multidimensional array objects and a collection of routines.
2. Pandas: Used for data manipulation and analysis.
3. Scipy: Used for calculating basic statistics
4. Matplotlib and Seaborn: Used for data vizualization 

## Process
1. We first start by loading the house price dataset into a pandas data frame.
2. Initially, we check the shape of data which gives us the number of observations and features in our data frame. 
3. We check the data types of columns and ensure that they are of the correct type. We identify numerical and categorical variables of the house price dataset. 
4. Most of the time, datasets have missing values; therefore, it is necessary to check null values. We have identified columns having more than 20% null values and dropped columns containing more than 80% null values.
5. We have employed different visualization techniques to study the dataset and generate useful insights about the sale price of a house.  


# Data Visualization
It is an important part of EDA and we extensively plot data points to visually understand our data better. 

## Bar Plots
Bar plots are used to represent the relationship between a categorical variable and a numerical variable. Each bar represents a category and the height/length of the bar represents the measured value for that category. The bars in bar plots can be plotted horizontally or vertically. It is important to sort the bars as it becomes easy to gain insights from the visualization. 

In our project, we have used a horizontal bar plot to visualize the number of null values in different variables of the house price dataset. Sorting the bars makes it easier to spot variables with a maximum and a minimum number of null values.

![BarPLot](https://github.com/harshit206/EDA-House-Price/blob/main/plots/horizontal_bar_chart_null_values.png)



## Scatter Plots
Scatter plots are used to visualize the relationship between two numerical variables. The dots on the scatter plot represent the values of the data point for the numerical variables under study. The relationship could be positive or negative, linear or non-linear, etc. and such different natures of the relationship can be inferred using scatter plots.

For example, in our project, we have used a scatter plot to check the nature of the relationship between the ground living area of a house and its sale price.


![ScatterPLot](https://github.com/harshit206/EDA-House-Price/blob/main/plots/scatter_plot1.png)

Looking at the scatter plot, we can estimate that there exists a positive linear relationship between the two.



## Box Plots
A boxplot is a way of displaying the distribution of data based on a five-number summary: minimum, first quartile (Q1), median, third quartile (Q3), and maximum. It helps us to understand how the values are distributed. 

In our project, we have used a box plot to check how house sale prices are distributed for each level of the overall quality of the house. 

![Box Plot](https://github.com/harshit206/EDA-House-Price/blob/main/plots/box_plot1.png)


We can see that the median and quartile values of house sale prices increase for all levels of overall quality. Also, the distribution of house sale prices is more dispersed for the overall quality level of 10 as compared to other levels.


## Heatmaps
If we are analyzing a dataset for a descriptive purpose or for fitting a model like linear regression, we would be interested in knowing how different numerical variables in a dataset correlate with each other. In addition, we would be especially interested in knowing the correlation of different variables with the target variable under study. Heatmap can provide a color-coded summarised view of all the correlations between variables.

Let’s say, we are interested in fitting a linear regression model to understand how the house sale price of a house is related to other features and also check if the issue of multicollinearity exists among the predictive variables. 

![Heatmap](https://github.com/harshit206/EDA-House-Price/blob/main/plots/heatmap.png)


Using a heatmap, we can estimate that the ground living area of a house has a strong correlation to its sale price. As for the issues of multicollinearity, it can be observed that the number of cars that can fit in a garage is strongly correlated to the garage area, which makes sense. Hence, we have identified an example of multicollinearity here.

# Usage
1. Download the house price dataset from [here](https://www.kaggle.com/c/house-prices-advanced-regression-techniques).

2. To run the notebook, please install the following libraries via the `pip` command. 

```
pip install numpy
pip install pandas
pip install scipy
pip install matplotlib
pip install seaborn
```



