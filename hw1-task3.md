# Homework 1 Task 3

---

Answer the following questions based on exercises from *An Introduction to Statistical Learning with Applications in Python*.

## Chapter 2.4 Exercises

---

### Exercise 1 (ISLP exercise 2)

Explain whether each scenario is a **classification or regression** problem, and indicate whether we are most interested in **inference or prediction**. Finally, provide **n** (size of observation dataset) and **p** (number of predictors).

**(a)**  We collect data on 200 protected marine reserves worldwide. For each reserve we record species richness, reserve size, years since establishment, enforcement budget, and proximity to human settlements. We are interested in understanding which factors affect species richness.

> **Your Answer:**  This scenario is a regression problem, because we are interested in species richness as a quantitative response. We are most interested in inference, because we want to understand which predictors are associated with species richness. The size of the observation dataset (n) is 200, and the number of predictors (p) is 4 (reserve size, years since establishment, enforcement budget, and proximity to human settlements).

---

**(b)** A conservation agency wants to know whether a proposed habitat corridor will successfully support wildlife movement or fail to do so. They collect data on 30 previously established corridors. For each corridor they have recorded whether wildlife movement was successful or unsuccessful, corridor width, length, surrounding land use type, and eight other variables.

> **Your Answer:** This scenario is a classification problem, because the outcome we are interested in is binary, whether the corridor will successfully support wildlife movement or not. We are most interested in prediction, because they hope to be able to use the set of predictors to determine whether a proposed habitat corridor will be successful before implementing it. The size of the observation dataset (n) is 30, and the number of predictors (p) is 11 (corridor width, length, surrounding land use type, and 8 others).

---

**(c)** We are interested in predicting weekly average ground-level ozone concentration in a coastal city. We collect weekly data for all of 2019. For each week we record average ozone concentration, sea surface temperature, wind speed, solar radiation, and atmospheric

> **Your Answer:** This scenario is a regression problem, because the outcome of weekly average ground-level ozone is a quantitative value. We are interested in predicting this value from previous weekly data and various predictors. The size of the observation dataset (n) is 52, and the number of predictors (p) is 4 (sea surface temp, wind speed, solar radiation, and "atmospheric").

---

### Exercise 2 (ISLP exercise 5)

What are the advantages and disadvantages of a very flexible (versus a a less flexible) approach for regression? Under what circumstances might a more flexible approach be preferred to a less flexible approach? When might a less flexible approach be preferred?

> **Your Answer:** A very flexible approach for regression can have the advantage of matching the estimate of the function to the true function (f) of the data more closely through estimating a greater number of parameters, such as when the relationship is non-linear. However, this comes with the disadvantage of being more complex or less interpretable. It can also lead to overfitting, following the noise within the data too closely and not generalizing well to new data. A more flexible approach might be preferred when we are largely interested in accurate predictions, not understanding how those predictions are made. A less flexible approach might be preferred when we are interested in inference and understanding the relationship of each predictor to the response. 

---

### Exercise 3 (ISLP exercise 6)

Describe the differences between a **parametric** and a **non-parametric** statistical learning approach. What are the **advantages** of a parametric approach to regression or classification (as opposed to a non-parametric approach)? What are its **disadvantages**?

> **Your Answer:**  A parametric approach involves making an assumption about the functional form of the true function f, such as a linear model. This has the advantage of reducing the problem of estimating f to just estimating the set of parameters in the model definition. However, the chosen model might not match the true form of f, and can lead to poor estimates in regression and classification. A non-parametric approach does not have explicit assumptions about the functional form of f, instead having a goal of getting as close to the data points as possible while still being a bit smoothed. This approach has the advantage of being able to accurately fit a wider range of shapes of f and avoid any risk of not fitting the data well as there were no assumptions made about the model initially. However, a lot of observations are needed for this approach to get an accurate estimate of f, and overfitting can easily occur if the function is too complex and not generalizable to new observations that were not a part of the training set. 