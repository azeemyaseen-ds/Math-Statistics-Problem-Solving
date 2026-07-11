# 🕵️‍♂️ Case File #15: The I-9 Logistic Depot Shift Safety Audit
**Domain:** Industrial Operations & Workplace Safety Compliance

## **Business Problem:**
A major supply chain and logistics fulfillment warehouse located in **I-9, Islamabad**, operates three continuous daily work shifts: **Morning, Evening, and Night**. The operations director reviewed a log of minor warehouse safety incidents over the last quarter. They want to know if specific shifts are inherently more dangerous, or if accidents are distributed completely randomly and independently across the day.

You must run a **Chi-Square** ($\chi^2$) **Test for Independence** to determine if there is a statistically significant association between the Work Shift and the Accident Severity Level.

**The Statistical Framework:**

 - **Null Hypothesis ($H_0$):** Incident Severity and Work Shift are completely independent. (Accidents happen randomly; no shift is uniquely unsafe).
 - **Alternative Hypothesis ($H_1$):** Incident Severity and Work Shift are dependent. (Certain shifts have a statistically higher rate of severe accidents).
 - **Significance Level ($\alpha$):** $0.05$

## **Technical Approach:**

1. Convert the raw Numpy Array into a properly labeled Pandas DataFrame.
2. Deployed Chi-Squared Test for Independence to know if there is a association between work shifts and warehouse accidents.
    - If p-value < 0.05: There is a statistically significant association in the work shifts and warehouse accidents and one of the shift is inherently dangerous for the business.
    - If p-value > 0.05: There is no association the warehouse accidents are completely random and independent across the day.
3. The Chi-Squared Test for Independence result is statistically significant.
4. I can calculate the Pearson Residual to figure out which shift is inherently dangerous for the business.
5. The Operations Director need to launch an immediate safety intervention for Night Shifts and also increase the Supervisory oversight during night shifts.