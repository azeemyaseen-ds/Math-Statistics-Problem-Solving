# 🕵️‍♂️ Case File #14: The Blue Area B-17 E-Commerce Interface A/B Test
**Domain:** Product Analytics & Conversion Rate Optimization (CRO)

## **Business Problem:**
An e-commerce firm based in **B-17, Islamabad**, launched a new user interface design (UI Version B) for its checkout page to see if it increases customer cart spending compared to the current design (UI Version A). They ran a live test for a week, capturing a random sample of purchase amounts from both groups.

The product owner claims: "Version B made significantly more money!" You must run a formal **Two-Sample Independent** $t$-**Test** to evaluate whether the difference in average spending is statistically significant, or if it's completely random noise.

**The Statistical Framework:**
 - **Null Hypothesis ($H_0$):** $\mu_A = \mu_B$ (The true average spending is the same for both versions. The difference is a fluke).
 - **Alternative Hypothesis ($H_1$):** $\mu_A \neq \mu_B$ (The true average spending is significantly different between the two versions).
 - **Significance Level ($\alpha$):** $0.05$ (Your threshold for proof. If your calculated $p$-value is less than 0.05, you reject $H_0$ and declare victory).

## **Technical Approach:**

1. Calculate the sample mean for both groups.
2. Deployed Independent Two-Sample t-Test to evaluate whether the difference is avg. spending is statistically significant, or it's completely random noise.
    - If p-value > 0.05: Any difference between groups is just a random noise.
    - If p-value < 0.05: The difference between groups is statistically significant.
3. The Independent Two-Sample t-Test result is statistically significant.
4. The test prove the reliability of mean as well. To spot the winner we can compare the mean of both groups.
5. The New User Interface design made significantly more money. So the business has to deploy the User Interface Design on it's checkout page.