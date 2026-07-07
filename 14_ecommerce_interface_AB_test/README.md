# 🕵️‍♂️ Case File #14: The Blue Area B-17 E-Commerce Interface A/B Test
**Domain:** Product Analytics & Conversion Rate Optimization (CRO)

# Business Problem:
An e-commerce firm based in **B-17, Islamabad**, launched a new user interface design (UI Version B) for its checkout page to see if it increases customer cart spending compared to the current design (UI Version A). They ran a live test for a week, capturing a random sample of purchase amounts from both groups.

The product owner claims: "Version B made significantly more money!" You must run a formal **Two-Sample Independent** $t$-**Test** to evaluate whether the difference in average spending is statistically significant, or if it's completely random noise.

# Technical Approach:
 - Use the `scipy.stats.ttest()` to perform a 2-sample independent t-test on the 2 groups of data to check which User Interface is working better.
 - Calculate the sample mean for both groups but before applying ttest on data we don't make conclusion from mean of both groups.
 - Calculate the t-statistics and p-value by applying a 2-sample independent t-test by `stats.ttest_ind(group_A_spend, group_B_spend)`. **t-statistics** measure the signal in data and **p-value** measures the exact probability of observing our data.
 - Use conditional statements to check whether p-value is less or greater then **alpha(0.05)**. If p-value is **less than 0.05** then **difference is reliable** otherwise the difference is just a random noise.