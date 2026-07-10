# E-commerce-Website-Performance-Customer-Behavior-Analysis-SQL
This project analyzes the Google Analytics Sample dataset using SQL in Google BigQuery to evaluate website performance, customer behavior, and purchasing patterns. The analysis provides actionable insights into traffic sources, user engagement, conversion performance, and revenue trends to support data-driven business decisions.

## Business Problem ##
An e-commerce company wants to understand how customers interact with its website, identify the most effective traffic sources, monitor conversion performance, and evaluate purchasing behavior to improve marketing effectiveness and revenue growth.

## Dataset ##
- Source: Google BigQuery Public Dataset
- Dataset: Google Analytics Sample Dataset (bigquery-public-data.google_analytics_sample.ga_sessions_*)
- Main Dimensions: Date, Visitor, Traffic Source, Device, Product
- Main Metrics: Visits, Pageviews, Transactions, Revenue
  
| Field                 | Description         |
| --------------------- | ------------------- |
| date                  | Session date        |
| fullVisitorId         | Visitor ID          |
| totals.visits         | Website visits      |
| totals.transactions   | Number of purchases |
| totals.pageviews      | Page views          |
| trafficSource.source  | Traffic channel     |
| device.deviceCategory | Device type         |
| productRevenue        | Revenue             |
| productQuantity       | Quantity            |

# Query #
**Query 01: calculate total visit, pageview, transaction for Jan, Feb and March 2017 (order by month)**

**Query 02: Bounce rate per traffic source in July 2017 (Bounce_rate = num_bounce/total_visit) (order by total_visit DESC)**

**Query 03: Revenue by traffic source by week, by month in June 2017**

**Query 04: Conversion rate by traffic source in 2017. (order by conversion_rate desc)**

**Query 05: Average number of pageviews by purchaser type (purchasers vs non-purchasers) in June, July 2017.**

**Query 06: Average number of transactions per user that made a purchase in July 2017**

**Query 07: Revenue contribution by device (desktop,mobile...) in 2017(order by ratio desc)**

**Query 08: Other products purchased by customers who purchased product "YouTube Men's Vintage Henley" in July 2017. Output should show product name and the quantity was ordered.**

**Query 9: Calculate cohort map from product view to addtocart to purchase in Jan, Feb and March 2017. For example, 100% product view then 40% add_to_cart and 10% purchase.**
Add_to_cart_rate = number product  add to cart/number product view.
Purchase_rate = number product purchase/number product view. The output should be calculated in product level.

**Query 10: Calculate revenue by week from May to July 2017 and culmulative revenue.**

