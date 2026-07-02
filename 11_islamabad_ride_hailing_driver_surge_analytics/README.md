# Case File 11: The Islamabad Ride-Hailing Driver Surge Analytics
**Domain:** Pricing Optimization & Operations Strategy

# Business Problem:
A ride-hailing tech platform operating in Islamabad wants to optimize its dynamic surge-pricing model across different sectors (F-10, I-8, D-12). The operations manager noticed that looking at the basic average number of available drivers per hour doesn't help because some sectors suffer from extreme, unpredictable driver supply swings, while others stay stable.

You must construct a statistical diagnostic script to analyze driver availability variation. The goal is to isolate sectors experiencing high instability (dispersion) so the company can deploy localized driver cash bonuses to stabilize the grid.

# Technical Approach:
 - Use the `agg()` method to calculate the (mean, median) & (variance, standard deviation) across each sector.
 - Calculate the **coefficient of variation %** for each sector using it's formula to understand which sector is more stable and unstable.
 - **Isolate the sector** that is **highly unstable** and need management attention.