# Toy problems
Toy problems to play with and discuss.

Prelim:
* we assume that the data contains information that is associated with the target
* we assume nothing in terms of the causal structure

**Binomial**:
* [569 samples, 30 IV's, Breast Cancer Wisconsin](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))

**Regressive**:
* [442 samples, 10 IV's, Diabetes](https://www4.stat.ncsu.edu/~boos/var.select/diabetes.tab.txt)

To spice things we can
* add synthetic data using generators trained on the data at hand or using pre-set generators (such as Friedman in sklearn) 
* introduce varies types of missingness
* add multicollinearity
* introduce cohort-bias
* add samples from a different population



