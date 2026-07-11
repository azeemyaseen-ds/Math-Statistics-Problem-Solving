# 🕵️‍♂️ Case File #16: The Blue Area Co-Working Space Multi-Branch Revenue Evaluation
**Domain:** Venture Analytics & Experimental Design

## 📌 **Business Problem**

A premium co-working space brand operating across three major hubs in Islamabad (**Blue Area, DHA Phase II, and Gulberg Green**) wants to optimize its membership pricing model. The community operations manager tracked the daily revenue generation (in PKR) from random matching days across all three locations.

The operations manager claims: *"One of these branches is significantly outperforming the others in terms of average daily revenue generation."* Before they reallocate the marketing budget, they need you to mathematically prove if the average revenue across all three branches is truly different, or if the variations are just ordinary random noise.

Because you are comparing the means of **three independent groups**, a standard two-sample $t$-test will fail (running multiple $t$-tests heavily inflates your chances of making a false positive error). You must implement a **One-Way ANOVA (Analysis of Variance)** test.

**The Statistical Framework:**

 - **Null Hypothesis ($H_0$):** $\mu_{\text{BlueArea}} = \mu_{\text{DHA}} = \mu_{\text{Gulberg}}$ (The true average daily revenue is identical across all three branches).
 - **Alternative Hypothesis ($H_1$):** At least one branch has a true average daily revenue that is significantly different from the others.
 - **Significance Level ($\alpha$):** $0.05$


## 🛠️ **Technical Approach**

1. Calculate the sample mean for all the groups.
2. Deployed One-Way ANOVA Test to compare the averages of independent groups to see if at least one of them is different from others.
    - If p-value < 0.05: The difference between groups is statistically significant.
    - If p-value > 0.05: Any difference between groups is just a random noise.
3. The result of One-Way ANOVA Test is statistically significant. So deployed Tuckey HSD Test that protects from finding the false winners by comparing the pairs of groups at the same time.
4. Tuckey HSD result in a comparison table that compare groups with each other.
5. The table show Blue_Area branch is significantly outperforming others. So the Community Operations Manager has to replicate Blue_Area's success to optimize underperforming locations.