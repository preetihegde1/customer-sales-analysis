# customer-sales-analysis
To find all possible insights from a customers’ two years transaction detail and provide my observations and recommendations

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


![](screenshots\datamodel.png)  


## error details

![](screenshots\error_summary.png)  

![](screenshots\Invalid_Stock_Code.png)  

## view notebook

You can view the notebooks here on GitHub - [here](https://github.com/preetihegde1/customer-sales-analysis/blob/main/jupyter/Customer_behaviour_analysis.ipynb).


## Tableau Dashboard

View tableau dashboard [here](https://public.tableau.com/app/profile/preetihegde/viz/DecathlonCustomerAnalysis/Overview?publish=yes)


# Recommendations 

Below are the recommendations based on my analysis of data

### 1- Focus on acquiring new customers and improving retention rate for 2010 and 2011 cohorts.

![](screenshots\Cohorts.png)

> **85%** of sales is from **UK** , other geographies can be focused to bring new customers 

![](screenshots\retention.png)

> Since the retention rates for the 2010 and 2011 cohorts are lower compared to the 2009 cohort, prioritize efforts to improve retention among these cohorts.

### 2.Engage At Risk Customers and reactivation of Lost Customers

![](screenshots\AtRisk.png)

> Implement targeted re-engagement campaigns to win back lost and at-risk customers business. 

>Use data-driven segmentation to further categorize At-risk customers based on their likelihood to churn and the potential value of retaining them. Prioritize efforts on high-value At-risk customers who have the potential for long-term loyalty and significant revenue contribution.

### 3.Personalized Customer Experience , Rewards program for Best & Loyal customers who bring in 80% of the sales revenue

![](screenshots\Vip.png)

> Concentrate on retaining the Best Customers, Big Spenders and Loyal Customers whose days since the last purchase is less than a month by implementing personalized loyalty programs tailored to the specific preferences and buying behaviors. Providing VIP perks to incentivize repeat purchases and foster a sense of appreciation.

> Gather continuous feedback from these Customers to understand their evolving needs and expectations. Conduct regular surveys, feedback forms, and customer interviews to gather insights. Use this feedback to make data-driven improvements to products, services, and customer experiences.



### 4.Promote Upselling for Mid-Priced Products & Diversify Pricing Strategy

Substantial portion of **80%** of company's revenue in sales, is generated from products priced below **5£** . This indicates that the lower-priced products are driving a significant portion of the company's overall sales volume.

  ![](screenshots\price_analysis.png)

> While low-priced products contribute significantly to sales volume, there is also a market for products priced between $5 and $10. The company can implement upselling strategies to encourage customers purchasing lower-priced items to also consider mid-priced products. This can be achieved through bundle offers, cross-selling recommendations, or promotional campaigns highlighting the value of mid-priced products.


