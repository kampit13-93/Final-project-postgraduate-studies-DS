## Summary

After performing data preprocessing and cleaning, the class distribution, number of instances, and number of features were determined. There are two classes: **edible mushrooms** and **poisonous mushrooms**. The dataset contains **23 features including the class label**, so a maximum of **22 features** will be used in the training dataset. The total number of instances is **8124**.

**Class distribution:**

- Edible mushrooms: 51.8% (4208)
- Poisonous mushrooms: 48.2% (3916)

Data visualization suggests that it is **possible to unambiguously determine the class** based on certain feature values.

### Classifier Results

The results were obtained for the original dataset as well as its **standardized** and **normalized** versions:

- **Logistic Regression**:
  - ROC curves indicate near-perfect classifier performance.
  - Learning curves converge at the ends.

- **K-Nearest Neighbors (KNN)**:
  - Classifier performance is **perfect**, regardless of data preprocessing.

- **Support Vector Machine (SVM)**:
  - **Linear** and **polynomial** versions achieve very high accuracy.
  - The **sigmoid version** performs the worst – it misclassifies **8 poisonous mushrooms as edible**.
  - In the standardized version, the learning curves converge the least among all.

- **Naive Bayes Classifier**:
  - Does not make dangerous mistakes.
  - **33 edible mushrooms** are incorrectly classified as poisonous.

- **Decision Trees and Random Forests**:
  - Do not make any errors.
  - Learning curves **converge nicely**.
