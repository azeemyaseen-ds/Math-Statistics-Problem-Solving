# 🕵️‍♂️ Case File #17: The G-11 Tech Startup Ad-Spend & User Acquisition Model
**Domain:** Growth Marketing & Customer Acquisition Cost (CAC) Optimization

## **Business Problem:**

A growing mobile app startup based in **G-11, Islamabad**, wants to scale up its user base. Over the past 8 weeks, the growth marketing team adjusted their weekly digital ad-spend (in thousands of PKR) and tracked the corresponding number of new verified user sign-ups.

The Marketing Director claims: *"If we throw more money into ads, sign-ups scale up in a perfectly predictable linear line."* Before they authorize a massive capital infusion, they want you to model the mathematical relationship between spend and acquisition to calculate the exact **Expected Return on Investment (ROI)** and check for directional strength.

**The Mathematical Framework:**
You must model the data using a simple linear equation:

$$y = m\cdot x + c$$

Where:
 - $y$ is the Dependent Variable (New Sign-ups)
 - $x$ is the Independent Variable (Ad-Spend)
 - $m$ is the **Slope** (How many new users you gain for every 1 unit increase in ad-spend)
 - $c$ is the **Intercept** (The baseline sign-ups you expect even if ad-spend is zero)

## **Technical Approach:**

### 1. Pearson's Correlation Coefficient:
 - Our analysis yielded a Pearson's *r* of **0.993**, indicating an extremely strong positive relationship. This statistically proves that ad spend and user acquisition scale together in a near-perfect linear fashion, validating the Marketing Director's hypothesis and confirming that a linear model is highly reliable for forecasting.

### 2. Predictive Linear Modeling:
We mapped the relationship using linear regression equation (y = mx + c), which revealed key baseline metrics:

 - **Baseline Sign-ups (Intercept):** If the startup spends 0 PKR on ads, we can still expect a baseline of approximately **12.93** verified user sign-ups per week through **organic traffic**.
 - **Acquisition Velocity (Slope):** For every additional 1,000 PKR spent on digital ads, the startup can expect to gain approximately **11.43** new sign-ups.