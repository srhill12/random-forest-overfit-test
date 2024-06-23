# random-forest-overfit-test

# Random Forest Model

## Purpose

Attempt to fit a Random Forest model using bank marketing data and will use balanced accuracy as a metric, test the model for overfitting, and attempt to tune the max_depth parameter in the logistic regression model to prevent over- and underfitting.

## Steps

1. Import and clean the data.

2. Create a Random Forest model and train it with the X_train and y_train data.

3. Check the model's balanced accuracy on the testing data.

4. Check the model's balanced accuracy on the training data.

5. Using the provided values, create a loop to test several values of the max_depth parameter in a Random Forest model.

6. Create a DataFrame from the models dictionary using "max_depth" as the index.

7. Plot the results. Does any particular max_depth value show a resistance to overfitting?

## Analysis and Conclusion:

1. **Balanced Accuracy Scores:**
   - The balanced accuracy score for the training data is 0.6322.
   - The balanced accuracy score for the test data is 0.5938.

2. **Graph Analysis:**
   - The graph shows the relationship between the maximum depth of the decision tree (`max_depth`) and the accuracy scores for both the training and test datasets.
   - As the `max_depth` increases, both the training and test scores improve. However, the training score increases more rapidly than the test score.

3. **Conclusion:**
   - The model is overfitting: the training accuracy continues to improve while the test accuracy starts to plateau or increase at a slower rate.
   - The training score is significantly higher than the test score, indicating that the model is memorizing the training data rather than generalizing well to new data.
   - To improve the model, consider using techniques such as pruning, cross-validation, or exploring other models to prevent overfitting.

## References

Moro, S., Rita, P. & Cortez, P. 2012. *Bank marketing* [Dataset]. UCI Machine Learning Repository. Available: https://archive.ics.uci.edu/dataset/222/bank+marketing [2023, October 17]. *Note that this data set has been modified/cleaned/shortened for the purpose of this activity. You can access the modified data in the CSV file provided.* ([CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/legalcode))
