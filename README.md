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
## Query 01: ##
- **Query 01: Calculate total visit, pageview, transaction for Jan, Feb and March 2017 (order by month)**
<img width="1306" height="324" alt="image" src="https://github.com/user-attachments/assets/b90336bd-50c5-4a44-a2c5-8616be6808ca" />
<img width="962" height="170" alt="image" src="https://github.com/user-attachments/assets/fea2d473-638e-404c-bf1c-2f41e1086306" />

## Query 02: ##
- **Query 02: Bounce rate per traffic source in July 2017 (Bounce_rate = num_bounce/total_visit) (order by total_visit DESC)**
<img width="1088" height="230" alt="image" src="https://github.com/user-attachments/assets/a5c9e345-23d3-4dd0-a846-3a113432ace2" />
<img width="948" height="448" alt="image" src="https://github.com/user-attachments/assets/ef8355c3-11bf-4225-ad20-183bd403af3e" />

## Query 03: ##
- **Query 03: Revenue by traffic source by week, by month in June 2017**
<img width="960" height="650" alt="image" src="https://github.com/user-attachments/assets/b1e274e0-3b8b-4aa6-88d6-0a82fd85ca93" />
<img width="1082" height="646" alt="image" src="https://github.com/user-attachments/assets/ed7957ab-6b22-4e38-adf1-bc4aa219ca10" />

## Query 04: ##
- **Query 04: Conversion rate by traffic source in 2017. (order by conversion_rate desc)**
<img width="1036" height="250" alt="image" src="https://github.com/user-attachments/assets/91283dae-549e-4e5e-b420-a6db037a8d65" />
<img width="916" height="276" alt="image" src="https://github.com/user-attachments/assets/e3a900bb-286b-4cef-9d0f-80821ca5c2f1" />

## Query 05: ##
- **Query 05: Average number of pageviews by purchaser type (purchasers vs non-purchasers) in June, July 2017.**
<img width="1032" height="706" alt="image" src="https://github.com/user-attachments/assets/cefde148-6743-434a-8c8d-ef0a674d3809" />
<img width="750" height="110" alt="image" src="https://github.com/user-attachments/assets/d10d3cc1-fd0e-4bc2-b2f0-b6f8669e3804" />

## Query 06: ##
- **Query 06: Average number of transactions per user that made a purchase in July 2017**
<img width="1030" height="210" alt="image" src="https://github.com/user-attachments/assets/b4cb6468-9b26-4a73-93dd-7929f5025250" />
<img width="704" height="112" alt="image" src="https://github.com/user-attachments/assets/a100119d-92f5-4a6c-b6dc-350f8261e255" />

## Query 07: ##
- **Query 07: Revenue contribution by device (desktop,mobile...) in 2017(order by ratio desc)**
<img width="1022" height="468" alt="image" src="https://github.com/user-attachments/assets/f33f41c0-9b73-4c9c-a535-a19195bce731" />
<img width="1004" height="162" alt="image" src="https://github.com/user-attachments/assets/ed19e8b1-5bee-4b35-a91e-094d4440657b" />

## Query 08: ##
- **Query 08: Other products purchased by customers who purchased product "YouTube Men's Vintage Henley" in July 2017. Output should show product name and the quantity was ordered.**
<img width="1010" height="688" alt="image" src="https://github.com/user-attachments/assets/c8c955df-2c09-4691-9ca6-a08328e2456c" />
<img width="666" height="400" alt="image" src="https://github.com/user-attachments/assets/fc872ed7-9a4f-422f-95d2-5335c5d69301" />

## Query 09: ##
- **Query 9: Calculate cohort map from product view to addtocart to purchase in Jan, Feb and March 2017. For example, 100% product view then 40% add_to_cart and 10% purchase.**
Add_to_cart_rate = number product  add to cart/number product view.
Purchase_rate = number product purchase/number product view. The output should be calculated in product level.
<img width="746" height="634" alt="image" src="https://github.com/user-attachments/assets/d43896ac-0681-4eb4-b5bc-f853636ad071" />
<img width="940" height="116" alt="image" src="https://github.com/user-attachments/assets/a9616395-c264-40ef-81ce-418b3e4fc4ad" />

## Query 10: ##
- **Query 10: Calculate revenue by week from May to July 2017 and cumulative revenue.**
<img width="858" height="586" alt="image" src="https://github.com/user-attachments/assets/043c4290-c3ac-4780-a2da-790ca6689594" />
<img width="746" height="402" alt="image" src="https://github.com/user-attachments/assets/14062dc8-7ace-4017-8eef-2af058fbf61e" />

