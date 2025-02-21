## Project
Duplication and Dimensionality Issues - Classification Task



## Description
This project addresses two major data quality issues: data duplication and data dimensionality. We aim to analyze the effects of these issues on various classification algorithms, including Decision Tree, Logistic Regression, KNN, Random Forest, AdaBoost, and MLP.

## Data Duplication
### Setup Choices
- **Data Collection:** Used the `make_classification` function from the sklearn package to create a dataset with 1000 samples and 5 features.
- **Experiments:** Created 10 experiments with varying similarity and duplication rates to observe the impact on classification algorithms.

### Data Pollution
- Generated duplicates by selecting a small set of "original" rows and creating multiple duplicates with varying degrees of similarity.
- Added duplicates to the dataset without altering the labels.

### Pipeline Implementation
1. Build reference dataset.
2. Explore the dataset.
3. Create polluted datasets.
4. Apply classification algorithms.
5. Evaluate classification results using weighted F1 score, distance between training and test sets, and execution time.
6. Print results on graphs and tables.
7. Remove duplicates using Record Linkage.
8. Re-evaluate classification results.

### Record Linkage
- Identified duplicates using a similarity score and a threshold.
- Assessed performance through accuracy, precision, and recall.

### Results
- Observed that more duplicates generally improve performance due to overfitting.
- Decision Trees showed the biggest performance gap between training and test sets.
- KNN was efficient but affected by the curse of dimensionality.

## Data Dimensionality
### Setup Choices
- **Experiments:** Created 20 experiments to observe the impact of varying numbers of features and samples on classification algorithms.

### Pipeline Implementation
1. Build and pollute datasets by varying the number of features and samples.
2. Apply classification algorithms.
3. Evaluate classification results using weighted F1 score, distance between training and test sets, and execution time.

### Results
- Increasing features worsened the performance of KNN, DecisionTree, and MLP, while LogisticRegression, AdaBoost, and RandomForest remained stable.
- Increasing samples generally improved performance across all algorithms.

## References
- Complete results can be found in the attached Notebook
- 
## Contributors
- Simone Garbazio
- Francesco Pastori 
