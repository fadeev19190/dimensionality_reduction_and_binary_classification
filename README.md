# dimensionality_reduction_and_binary_classification

# Dimensionality Reduction and Binary Classification

* For this task, you need to handle high-dimensional data and then successfully apply an appropriate classification model.

> **The tasks are designed to give you space for creativity. Figuring out _how exactly_ you will solve the task is an important part of the assignment, and originality or ingenuity will also be evaluated!**

Use `Markdown` cells to explain your process. Points will be deducted for lack of clarity.

## Data Source

* The data source files are `train.csv` and `evaluate.csv`.
* These are 28x28 pixel grayscale images obtained from the [Fashion MNIST dataset](https://www.kaggle.com/datasets/zalando-research/fashionmnist).
* The `train.csv` file contains the training data.
* The target (dependent) variable is named **label**.
* The `evaluate.csv` file contains test data without actual label values.

## Instructions for Completion

**Assignment Points**, for which you will earn **25 points** for (honest) completion:
* Load the data from `train.csv` into the notebook. Split it appropriately into subsets for training, model comparison, and subsequent prediction of the final model’s performance.
* Conduct a basic data exploration and discuss your observations. Display some of the images as well.
* Sequentially apply the models **SVM**, **Naive Bayes classifier**, and **LDA**, where for each:
  * Comment on the suitability of each model for this type of task.
  * Select key hyperparameters to tune (if the model has hyperparameters) and find their best values.
  * Experiment with data standardization/normalization.
  * For SVM, try at least two different kernel functions.
  * Properly comment on the results obtained.

* Sequentially apply the dimensionality reduction methods PCA and LLE, where for each:
  * Repeat the previous steps and try to improve the models.
  * Investigate which dimensionality is best for the performance of the final model.
  * Properly comment on the results obtained.

* From all the tested options, select the final model and estimate the accuracy you can expect on new data not previously available.

* Finally, load the evaluation data from the `evaluate.csv` file. Use the final model to compute predictions for this data (the dependent variable is not included). Create a `results.csv` file where the obtained predictions are saved in the **label** column and identifiers in the **ID** column. Submit this file as well (save it to the project alongside the notebook).

* Example of the first few rows of the `results.csv` file:

ID,label

0,0

1,1

