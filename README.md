# Toy problems
Toy problems to play with and discuss.

Preliminary:
* we assume that the data contains information that is associated with the target
* we assume nothing in terms of the causal structure other than that there exists some parameterised combination of independent variables that is predictive for the target

**Binomial**:
* [569 samples, 30 IV's, Breast Cancer Wisconsin](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))

**Regressive**:
* [442 samples, 10 IV's, Diabetes](https://www4.stat.ncsu.edu/~boos/var.select/diabetes.tab.txt)

To spice things up we can
* add synthetic data using generators trained on the data at hand or using pre-set generators (such as Friedman in sklearn) 
* introduce varies types of missingness
* add multicollinearity
* introduce cohort-bias
* add samples from a different population

# Recipe 

Write down a plan-of-attack that describes your workflow in case you encounter a
dataset such as described. 

Assume that the task at hand requires a model that might be put into
production, if (and only if) it meets  certain criteria. Assume that 
your "customer" wants you to explain your steps and that you succinctly describe
your model performance and usefulness.

* how do you perform  model selection? i.e. to decide whether to use e.g. GLM's, GAM's or GBM?
* what types of missingness are there in your datasets, how do you know?
* what will you do to handle this, if anything? 
* how do you check for multicollinearity, do you need to? 
* if you need to account for multicollinearity, what do you do?
* do you need to perform feature selection, why? what do you use?
* how do you check for cohort-bias? 
* how do you mitigate this bias?
* you have a "working" model, great. Suppose you need to deliver a model card, how would you describe the "utility" in metrics/plots?
