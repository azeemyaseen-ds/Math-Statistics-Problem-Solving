# 🕵️‍♂️ Case File #13: The E-11 Food Delivery Logistics Speed Baseline
**Domain:** Last-Mile Delivery Operations & SLA Compliance

# Business Problem:
A food delivery tech startup operating in sector E-11, Islamabad, is reviewing its performance. The fleet operations logs show that delivery times are normally distributed with a population mean ($\mu$) of 28.5 minutes and a population standard deviation ($\sigma$) of 4.2 minutes.

The marketing department wants to launch a bold new guarantee campaign: "Food delivered in under 35 minutes, or your money back!" Before they announce it, the VP of Operations needs to know the exact statistical failure rate of this campaign so they can calculate the financial liability of refunding late orders.

# Technical Approach:
 - Use `scipy.stats` library to find the probability of success and failure of a deliveyr campaign.
 - Use `stats.norm.cdf()` to calculate the cumulative probability of delivery of an order in **more than and less than 35 minutes**.
 - Figureout the probability of delivery in **between 20 to 25 minutes** by subtracting larger probability percentage from smaller.
 - The analysis can help the busiess to calculate the financial liability of refunding late orders.