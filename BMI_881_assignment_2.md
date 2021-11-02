## Due 4 Nov 2021

## This is in relation to the paper on predicting nonmelanoma skin cancer, Wang et al. (2019).

### 1. If a test has sensitivity = 80% and specificity 80% and the prevalence of the disease is 9/100,000, what is the positive predictive value (aka “precision”) of the test?

**Answer**: PPV = (sensitivity x prevalence) / (sensitivity x prevalence + (1-specificity) x (1-prevalence)) = (0.8*9e-5) / ( 0.8*9e-5 + 0.2*(1-9e-5) ) = 0.00035990282 ~= 3.6e-4

### 2. Suppose sensitivity = specificity. What would they have to be to achieve positive predictive value = 50% when prevalence is 9/100,000?

**Answer**: PPV = (sensitivity x prevalence) / (sensitivity x prevalence + (1-specificity) x (1-prevalence)) = (X*9e-5) / ( X*9e-5 + (1-X)*(1-9e-5) ) = 0.5 ===> X = 1-prevalence = 0.99991

### 3. Comment on these results in relation to the precision values provided in Table 2 of Wang et al. (2019).

**Answer**: Given the very low prevalence of this disease, the precision of that predictor is 0.5 at most. The rate 0.5 is like flip a coin, but if we consider every 2 positive predictions can lead to 1 real patient, this may help, at the acceptable cost. Of course the further biopsy is needed for the certain diagnosis.
