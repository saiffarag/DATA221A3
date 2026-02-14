# DATA221A3

**Author:** Saif Farag  
**Course:** DATA 221  
**Assignment:** Assignment 3  

---

## Repository Contents
- `a3.ipynb` – Main notebook containing all questions and solutions.
- `crime1.csv` – Dataset used for Questions 1 and 2.
- `kidney_disease.csv` – Dataset used for Questions 3, 4, and 5.
- `README.md` – Description of the assignment.

---

## Question Breakdown

### Question 1 – Statistical Analysis
The crime dataset was loaded into a pandas DataFrame and summary statistics were computed for the `ViolentCrimesPerPop` column, including mean, median, standard deviation, minimum, and maximum values. Comments in the notebook discuss the relationship between mean and median, skewness, and how extreme values affect different statistics.

---

### Question 2 – Data Visualization
Two plots were created using matplotlib:
- A histogram showing the distribution of violent crime values.
- A box plot illustrating spread and median.

Each plot includes a title and labeled axes. Written comments describe the distribution of values and what the box plot indicates about the median and potential outliers.

---

### Question 3 – Data Preparation
The kidney disease dataset was loaded and separated into:
- Feature matrix **X** (all columns except `classification`)
- Label vector **y** (the `classification` column)

The data was split into 70% training and 30% testing sets using a fixed random state to ensure reproducibility. Comments explain why models should not be trained and tested on the same data and the purpose of a testing set.

---

### Question 4 – KNN Classification
A K-Nearest Neighbors classifier with **k = 5** was trained using the training data. Predictions were made on the test set and evaluated using:
- Confusion Matrix
- Accuracy
- Precision
- Recall
- F1-score

The comments includes explanations of True Positive, True Negative, False Positive, and False Negative in the context of kidney disease prediction, along with discussion on why accuracy alone is not sufficient for evaluation.

---

### Question 5 – Hyperparameter Comparison
Multiple KNN models were trained with different values of **k**: 1, 3, 5, 9

Test accuracy was computed for each model and displayed in a table. The best-performing value of k was identified. Comments explain how changing k affects model behavior, why small k values may lead to overfitting, and why large k values may cause underfitting.

---

## Libraries Used
- pandas
- numpy
- matplotlib
- scikit-learn

---

## Notes
- Basic preprocessing was applied to handle categorical values and missing data in the kidney disease dataset.
