# **Course Project**

## 🍕 Sales Analysis of Plato's Pizza 2015 🍕

by MC364742, Jessica Lai, Weijie

## Introduction

Plato’s Pizza is a Greek-inspired pizza place in New Jersey.

The dataset was made to analysis the sales of Plato's Pizza in 2015, to optimize the sales distribution and resources of ordering to imporve the efficiency and effectiveness of the fast-food wroking process.

It shows by the visualized charts and with analysis to better help owner deploy the resource for the branches, which can also be applied in other brands or company with the code pattern based on the dataset having similiar columns/categories.

This tutorial is for practice before starting a real business analysis by python coding and visualizing. The dataset content has been developed a long while and nowadays information is more abundant and there are more to explore for the dataset. Please use the dataset according to the authentic situation.


### Please kindly read the following instruction before you follow the tutorial:

**Overall Steps and Rundown** 

Step 1: Finding and download the dataset (an archive zip) file from the website

Step 2: Unzip it then use python to analyse task with visualization by different concerns

Step 3: Try it on your won by reading the explanation and code demonstration

Step 4: Produce conclusion by the visualized analysis for furthur strategic plan


**Notes** 
###### Please download and install Python and Jupyter Notebook in Anaconda before you start the tutorial.

**Tools Needed** 
###### Please install the following tools before you start the tutorial.

import pandas as pd

import seaborn as sns

import matplotlib.pyplot as plt

import matplotlib.dates as mdates

import matplotlib.cm as cm

from matplotlib_venn import venn2

from sklearn.preprocessing import LabelEncoder


###### Tools Introduction

pandas: Data processing and analysis
seaborn: Data visualization library for matplotlib
Matplotlib. pylot: the submodule of matplotlib, drawing various types of chart functions
matplotlib.dates: provides date and time related functions
matplotlib.cm: Map the value to the color space
matplotlib.venn: Draw a Venn diagram
sklearn.preprocessing LabelEncode: encodes categorical variables

## 1) SECTION 1: FINDING A DATASET


**Dataset Access**

There's an open resource file provided by kaggle.com, please download the dataset from:
https://www.kaggle.com/datasets/shilongzhuang/pizza-sales

**About the dataset**

Here are the definitionsfor each catagory which also could be found in data_dictionary.csv file:
order_id：Unique identifier for each order placed by a table
date：Date the order was placed (entered into the system prior to cooking & serving)
time：Time the order was placed (entered into the system prior to cooking & serving)
order_details_id：Unique identifier for each pizza placed within each order (pizzas of the same type and size are kept in the same row, and the quantity increases)
order_id：Foreign key that ties the details in each order to the order itself
pizza_id：Foreign key that ties the pizza ordered to its details, like si
quantity：Quantity ordered for each pizza of the same type and size
pizza_id：Unique identifier for each pizza (constituted by its type and size)
pizza_type_id：Foreign key that ties each pizza to its broader pizza type
size：Size of the pizza (Small, Medium, Large, X Large, or XX Large)
price：Price of the pizza in USD
pizza_type_id：Unique identifier for each pizza type
name：Name of the pizza as shown in the menu
category：Category that the pizza fall under in the menu (Classic, Chicken, Supreme, or Veggie)
ingredients：Comma-delimited ingredients used in the pizza as shown in the menu (they all include Mozzarella Cheese, even if not specified; and they all include Tomato Sauce, unless another sauce is specified)

**Business Task**

#### The enlightenment by sales trend and customer preference analysis to the resource optimization inspiration.

We can know the conclusion by the following concerns:
- Which is the peak ordering day in a year?
- Which quarter has the greatest sales?
- What size of the pizza is the most popular and their distribution?
- What are the Top 5 Pizzas by Sales and by Quantity?
- What are the Top 5 most popular pizzas considering of sizes by Quantity?
- No matter for the condition of consideration of size or not, what are the overlapping pizza names of the most popular by orders?
- What is the best-selling pizza category considering of orders?
- What are the Top 5 worst selling pizzas without size consideration?
- Is there any preference implications of size for those veggie-pizza orderers (for diet keeper or vegetarian)?
- What's the percentage for the people ordering more than one pizza in an order?
- What is the most frequently used TOP15 ingredient?
- What is the distribution of prices? What are the prices of different Pizza?
- Does the price have any correlation about the raw material?
- Correlation study between various factors in pizza sales.

## 2) SECTION 2: VISUALIZATION FOR EACH CONCERN


For example:

**1. Which is the peak ordering day in a year?** 
- With visualize chart generated by code
- With breifing for each concern:
**“From the bar chart above and the output text, we can learn that the peak sales day of the year is November 26, 2015 , which is Thanksgiving Day in the US.”**

## 3) SECTION 3: CONCLUSION FOR EXPLORATION


##### ** Detailed analysis is done and shown in Jupyter Notebook. 

**Analysis and Conlusion for Further Exploration**

The enlightenment by sales trend and customer preference analysis to the resource optimization inspiration.

It can be seen from the correlation matrix that total sales are positively correlated with quantity and total sales are positively correlated with unit price.

1. Holiday Peak Strategy :
Increase customer loyalty by preparing for peak orders during holidays like Thanksgiving.

2. Optimized Q2 :
Maximize profits by optimizing resources during peak sales quarters.

3. Popular pizza sizes :
Focus on ensuring that the popular "L" and "M" sizes have sufficient raw materials.

4. Classic Pizza Performance :
Prioritizing classic pizza in product development to maintain stable sales.

5. Size preference and nutrition :
Explore smaller, nutritionally balanced "S" pizzas with higher meat content.

6. Best-selling strategy :
Prepare more ingredients for the best-selling pizza and consider price adjustments.

7. To poor sellers :
Consider stopping production of underperforming products to save resources.

8. Vegan Pizza Insight :
Discount for large orders, as 45% of vegetarian pizzas are "L" size.

9. Consumer ordering habits :
Attract family orders by offering discounts or set meals on multiple pizzas.

10. Optimized ingredient placement :
Simplify production by placing commonly used raw materials in easily accessible locations.

11. Save expensive raw materials :
Ensure proper preservation of expensive raw materials, such as cheese and meat, to reduce losses.

These key points provide actionable insights into holiday preparation, quarterly optimization, size preferences, product development, pricing strategies, addressing underperformance, vegan pizza trends, and optimizing production efficiency.
