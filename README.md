# SamplingAssignment
## Sampling
By examining data from a representative subset of the population, sampling can provide insights about the population without requiring a comprehensive examination of every member. An oversampling strategy was used to address an initial dataset imbalance of 763 non-fraudulent cases and only 9 fraudulent cases. In order to match the majority class (non-fraudulent cases), more instances of the minority class (fraudulent cases) had to be created. This process produced a balanced dataset that was then combined into a single data frame.

The following methods of sampling were applied:

- Simple Random Sampling: Drawing samples from the population at random.
Systematic Sampling: After a random start, regular interval selection is made.
Choosing clusters at random from the population is known as cluster sampling.
- Stratified Sampling: Creating subgroups within the population according to predetermined standards.
- Bootstrap Sampling: Creating multiple samples from the original dataset by resampling with replacement.


Following the generation of five distinct samples using these techniques, five models were applied to each sample. The accuracies of each model for a given sample are summarized in the following table:

| Sample Technique      | Random Forest | Logistic Regression | Naive Bayes      | Decision Trees   | KNN              |
|-----------------------|---------------|---------------------|------------------|------------------|------------------|
| Simple Random Sampling| 0.9870        | 0.8831              | 0.7013           | 0.9610           | 0.8701           |
| Systematic Sampling   | 1.0000        | 0.8926              | 0.7450           | 1.0000           | 0.9329           |
| Cluster Sampling      | 1.0000        | 0.9670              | 1.0000           | 1.0000           | 0.9890           |
| Stratified Sampling   | 1.0000        | 0.9030              | 0.7239           | 0.9925           | 0.9552           |
| Bootstrap Sampling    | 1.0000        | 0.9250              | 0.7500           | 0.9625           | 0.9375           |

In above table, each row corresponds to a sampling technique, and each column represent the accuracy achieved by each model applied to the respective sample generated using that respective technique.
<br>
### The RANDOM FOREST outperformed all other models when applied to Stratified Sampling Technique.
