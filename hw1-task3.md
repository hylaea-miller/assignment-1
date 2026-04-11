# Homework 1 Task 3

---

Answer the following questions based on exercises from *An Introduction to Statistical Learning with Applications in Python*.

## Chapter 2.4 Exercises

---

### Exercise 1 (ISLP exercise 2)

Explain whether each scenario is a **classification or regression** problem, and indicate whether we are most interested in **inference or prediction**. Finally, provide **n** (size of observation dataset) and **p** (number of predictors).

**(a)**  We collect data on 200 protected marine reserves worldwide. For each reserve we record species richness, reserve size, years since establishment, enforcement budget, and proximity to human settlements. We are interested in understanding which factors affect species richness.

> **Your Answer:** This is a regression scenario, since the response variable (species richness) is numerical. We are most interested in inference, we want to understand which factors affect species richness, not just predict it. The size of the observed dataset is n = 200 marine reserves, and the number of predictors is p = 4: reserve size, years since establishment, enforcement budget, and proximity to human settlements.

---

**(b)** A conservation agency wants to know whether a proposed habitat corridor will successfully support wildlife movement or fail to do so. They collect data on 30 previously established corridors. For each corridor they have recorded whether wildlife movement was successful or unsuccessful, corridor width, length, surrounding land use type, and eight other variables.

> **Your Answer:** This is a classification scenario, since the outcome (successful or unsuccessful) is categorical. We are most interested in prediction, the agency wants to predict whether a new corridor will succeed. The size of the observed dataset is n = 30 corridors, and the number of predictors is p = 11: corridor width, length, surrounding land use type, and 8 other variables.
---

**(c)** We are interested in predicting weekly average ground-level ozone concentration in a coastal city. We collect weekly data for all of 2019. For each week we record average ozone concentration, sea surface temperature, wind speed, solar radiation, and atmospheric

> **Your Answer:** This is a regression scenario, since the response variable (ozone concentration) is numerical. We are most interested in predicting future ozone levels. The size of the observed dataset is n = 52 weeks (total weeks in a year), and the number of predictors is p = 4: sea surface temperature, wind speed, solar radiation, and atmospheric pressure
---

### Exercise 2 (ISLP exercise 5)

What are the advantages and disadvantages of a very flexible (versus a a less flexible) approach for regression? Under what circumstances might a more flexible approach be preferred to a less flexible approach? When might a less flexible approach be preferred?

> **Your Answer:** A very flexible approach for regression has the advantage of capturing more complex patterns by taking on many different functional forms for f. However, the disadvantage is overfitting, which happens when the model picks up random noise in the data rather than the true underlying patterns. A less flexible approach is preferred when the sample size is small, the data is noisy, or the goal is inference and interpretability. On the other hand, if the true relationship is complex, a less flexible model may miss important patterns and produce poor estimates of f, making a more flexible approach the better choice.


---

### Exercise 3 (ISLP exercise 6)

Describe the differences between a **parametric** and a **non-parametric** statistical learning approach. What are the **advantages** of a parametric approach to regression or classification (as opposed to a non-parametric approach)? What are its **disadvantages**?

> **Your Answer:** The difference between a parametric and a non-parametric statistical learning approach is that parametric methods assumes a specific functional form for f, then estimates the parameters of that form from the data. A non-parametric approach makes no assumption about the form of f, letting the data determine the shape of the function. The advantage of parametric methods is that they simplify the problem, estimating a small number of parameters is easier than estimating an arbitrary function, and results are more interpretable and easier to test statistically. The disadvantage is that if the assumed form is far from the truth, the model will fit poorly. Non-parametric methods are more flexible but require much more data and are harder to interpret.