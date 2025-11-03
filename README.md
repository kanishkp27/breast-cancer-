# Breast Cancer Classification Machine Learning Project

## Project Overview

This project is a Machine Learning based binary classification system used to predict whether a breast cancer tumor is **Benign (0)** or **Malignant (1)** using medical measurement features from breast cell nuclei.

This project uses the Breast Cancer Wisconsin dataset.

* Target label `diagnosis` is encoded as:

  * **0 → Benign**
  * **1 → Malignant**

The model is trained on numeric features such as:

* radius
* texture
* perimeter
* area
* smoothness
* concavity
* compactness
* fractal_dimension

Starting from this data, the model learns patterns that help predict cancer type for new unseen data.

---

## Steps Done in the Project

1. Import libraries (sklearn, pandas, numpy, matplotlib etc.)
2. Load dataset from CSV
3. Preprocessing

   * Drop unwanted columns
   * Encode target
   * Train-test split
4. Model Training

   * trained using Logistic Regression (you can replace/try SVM or Random Forest later)
5. Model Evaluation

   * checking accuracy score on test dataset
6. Predicting on new data

---

## Important Code Notes

Example target checking logic:

```python
if y_pred[0] == 1:
    print("The breast cancer is Malignant")
else:
    print("The breast cancer is Benign")
```

> **Note:** `else:` MUST be in same block as `if`, not in a separate cell.

---

## Dataset Details

The CSV dataset you provided contains 33 columns including many medical measurements. One column `Unnamed: 32` is NaN and should be dropped.

Dataset Columns count: approximately 569 rows × 33 columns.

---

## Tools / Libraries Used

* Python
* Pandas
* Scikit-Learn (sklearn)
* NumPy
* Matplotlib

---

## Output Meaning

| Value | Meaning          |
| ----- | ---------------- |
| **0** | Benign Cancer    |
| **1** | Malignant Cancer |

---

## Next Possible Improvements

* Try RandomForest / SVM for higher accuracy
* Deploy using Streamlit web app
* Export results to PowerPoint / PDF report
* Hyperparameter tuning

---

### Author

Model built using Python + Scikit-Learn
