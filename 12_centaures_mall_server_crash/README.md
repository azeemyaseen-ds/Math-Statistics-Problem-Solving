# Case File 12: The Centaures Mall Server Crash & Reliability Matrix
**Domain:** DevOps & Infrastructure Engineering Risk

# Business Context:
An e-commerce platform's localized edge server located at Centaurus Mall, Islamabad, experiences occasional random server dropouts due to localized grid power surges. Historical monitoring data shows that the server crashes at a stable average rate of **2.4 times per week** ($\lambda = 2.4$).The infrastructure manager wants to know the exact mathematical risk of various failure states next week so they can decide whether to invest in an expensive backup power supply.

# Technical Approach:
 - Use the `scipy.stats` python library to calculate the probability of spcific no of random events.
 - Use the `stats.poisson.pmf()` method to calculate the exact probability of an event.
 - Use the `stats.poisson.sf()` method to calculate the cummulative probability of an event.
 - Calculate these probabilities so the **business can decide** whether they have to **buy expensive backup power supply or not**.