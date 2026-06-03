This repo contains the code for Practical Application Assignment 5.1
By V Mui
## Project: Will the Customer Accept the Coupon?
Link to [the notebook] 
## Objective
To perform data analysis and highlight the differences between customers who did and did not accept the coupons. To provide insights and actionable recommendations.
For example, would a driver accept a coupon? What if the coupon was for a bar instead of a coffee house? Would weather impact the coupon acceptance rate? 
## Data
Data comes from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he/she will accept the coupon if he/she is the driver.
## Tools
Python and pandas were used to create statistical summaries 
Matplotlib and Seaborn libraries were utilized to create visualizations
## Data Quality
- Original data set has 12,684 rows and 26 columns.
- Duplicate rows: 74 (0.5%)
- Incorrect data types and bad values: “age” data has values '50plus' and 'below21'. “passanger” is a typo as column name.
- Missing values: "car" column has a lot of missing values (99.15%). 5 other columns with missing values have proportions of less than 1.71%.
- No outliers, unwanted spaces, funny or inconsistent values detected.
## Data Preparation: Data Cleaning and Transformation
- After data cleaning and transformation, the resulting data set has 12,079 rows and 25 columns.
- “age” data was cleaned and transformed to numbers. “passanger” typo fixed.
- “car” column was dropped. Other rows with missing values were dropped. 
## Data Analysis and Key Findings
Overview: 57% of all drivers accepted coupons ‘right away’ or ‘later before the coupon expires’, versus 43% did not accept the coupons.
I examined two coupon groups: Coffee House coupons and Bar coupons
- From the bar chart, "Coffee House" is the most frequent coupon type in the dataset. This is probably because drivers like the fast service and low-price nature of coffee house offerings.
Coffee House coupon acceptance
- Coffee house coupons acceptance rate (50%) is less than the overall coupon acceptance rate (57%). But coffee house coupons acceptance rate is still higher than bar coupon acceptance rate (41%)
- Drivers who went to coffee houses more than 3 times a month have a higher coffee house coupon acceptance rate (67%), than that of drivers who went 3 or fewer times (45%). Hypothesis: drivers who are already frequent coffee shop visitors tend to accept coffee house coupons.
- Drivers with passenger(s), who went to a coffee house more than 3 times a month have a high coffee house coupon acceptance rate (75%) than the other drivers. Hypothesis: coffee lovers would love to drive passengers to use coupons to enjoy coffees together.
- Driving direction is not a predictive indicator of coupon acceptance. Hypothesis: these frequent coffee shop visitors love coffees so much that they will accept the coffee house coupons anyway, regardless of driving direction!
- Drivers liked coffee house coupons during morning time, when it was rainy outside. Hypothesis: mornings are when most people needed coffee, especially when coffee houses are good shelters in rainy days.
- Student drivers were more likely to accept coffee house coupons when temperature was hot outside. Hypothesis: students like to do schoolwork with air conditioning inside a coffee house.
Bar coupon acceptance
- Bar coupons acceptance rate (41%) is less than the overall coupon acceptance rate (57%). i.e. over half of the driver population did not accept the car coupon. Hypothesis: drivers are mindful that “don’t drink and drive”.
- Drivers who went to a bar more than 3 times a month have a high bar coupon acceptance rate (76%), more than double that of drivers who went to a bar 3 or fewer times (37%).
- Adult drivers (age over 25) who love going to bars frequently are more likely to accept bar coupons (69%).
- Hypothesis: drivers who are frequent bar goers are more likely to accept bar coupons
- Drivers who went to a bar more than once a month, not driving a kid, not in farming, fishing, or forestry have a high bar coupon acceptance rate (71%), more than double that of other drivers (30%). Hypothesis: these three occupations are usually in remote locations with fewer bar selections
- Widowed Drivers who love going to bars frequently but driving a kid were less likely to accept bar coupons. Hypothesis: under-age kids are not allowed in bars to consume alcohol.
- Drivers who frequently visit cheap restaurants with lower incomes are more likely to accept bar coupons. Hypothesis: this group are cost-conscious and love coupons to save money.
- Widowed drivers who love going to bars frequently but driving a kid were *less* likely to accept bar coupons. Hypothesis: under-age kids are not allowed in bars to consume alcohol.
## Recommendations
Recommendations to businesses to improve coupon acceptance rates
- Both bar and coffee house coupon groups show that when drivers were already frequent visitors of that coupon category, they displayed higher coupon acceptance rates for that category.  Therefore, it is highly recommended to target promotion of coupons to those who are already frequent visitors.
- Coffee house coupons are popular and more likely to be accepted. Bar coupons are not very popular overall, especially when passengers are kids. It will be more effective to promote popular coffee house coupons than bar coupons.
- Driver’s occupation plays a role in coupon acceptance. It is more effective to promote bar coupons to drivers that do not have occupations in remote areas. And it is more effective to promote coffee house coupons to students when outside temperature is hot.
- Time of the day, weather and temperature play a role in coffee house coupon acceptance. It is more effective to send drivers coffee house coupons in rainy mornings!
- Spending level affects coupon acceptance. Bar coupon issuers should target drivers who go to cheap restaurants frequently with lower income level.
## Next Step
In addition to the recommendations above, it is logical to continue to examine all the other coupon groups (restaurants, takeouts, etc.) in the dataset to detect trends and parameters related to coupon acceptance.

