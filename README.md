# customer-sales-analysis
To find all possible insights from a customers’ two years transaction detail.

## objective
  1.  Explore the dataset
  2.  Visualize sales Trends Over Time
  3.  Find products , customers trend over time
  4.  Customer Segmentation (RFM Analysis)
  5.  Geographic Analysis
  6.  Product Affinity analysis (Market Basket)
  7.  Retention rate
  8.  Error / Outlier Analysis

Finally to provide recommendation based on observations and analysis

## tools used
  * Python - for Data Prep
  * Tableau - for comprehensive visualization

## steps followed
  1.   Merge two datasets 2009-10 , 2010-11
  2.   Clean the data based on assumptions and exploratory analysis
  3.   Capture errors for data governance and analysis
  4.   Extend data set to include necessary fields for further analysis.
  5.   Advance analytics in python to derive RFM scores and segments
  6.   Write the file back with all additional fields for further tableau visualizations / interactivity.
  7.   Tableau dashboard

## assumptions on data 

  *    Invoice number and cancelled invoice numbers provided in the dataset do not match , the numerics are different - Hence Cancelled ordered are ignored in most of the analysis. However, it is included while computing TotalSales.
  *    Stock code to Description should be 1:1
  *    CustomerID cannot be null
  *    Postage charges are ignored in this analysis , however provided production costs , postage charges will be useful to evaluate the profit. 
  *    Discounts are not matching exactly with invoice and stock codes hence ignored.
  *    Price=0 is ignored in this analysis , as they dont contribute to any revenue.


## error details

![](screenshots\error_summary.png)  

![](screenshots\Invalid_Stock_Code.png)  

## view notebook

You can view the notebooks here on GitHub. See the [here](https://github.com/preetihegde1/customer-sales-analysis/blob/main/jupyter/Customer_behaviour_analysis.ipynb) for the complete list.


## Tableau Dashboard

View tableau dashboard [here](https://public.tableau.com/app/profile/preetihegde/viz/DecathlonCustomerAnalysis/Overview?publish=yes)


## 3 Recommendations 



