# Heart Attack Risk Prediction using SVM

## Project Overview

This project leverages a Support Vector Machine (SVM) model to predict the likelihood of heart attacks based on medical data. The dataset includes features such as age, gender, chest pain type, blood pressure, cholesterol levels, and other health indicators. The goal is to classify individuals into high-risk and low-risk categories to assist in early diagnosis and prevention of heart attacks.

## Dataset

The dataset contains the following columns:

- **age**: Age of the individual
- **sex**: Gender (1 = Male, 0 = Female)
- **cp**: Chest pain type
  - 1: Typical angina
  - 2: Atypical angina
  - 3: Non-anginal pain
  - 4: Asymptomatic
- **trtbps**: Resting blood pressure (in mm Hg)
- **chol**: Serum cholesterol level (in mg/dL)
- **fbs**: Fasting blood sugar > 120 mg/dL (1 = True, 0 = False)
- **restecg**: Resting electrocardiographic results
  - 0: Normal
  - 1: Having ST-T wave abnormality
  - 2: Showing probable or definite left ventricular hypertrophy
- **thalachh**: Maximum heart rate achieved
- **exng**: Exercise-induced angina (1 = Yes, 0 = No)
- **oldpeak**: ST depression induced by exercise relative to rest
- **slp**: Slope of the peak exercise ST segment
- **ca**: Number of major vessels (0-3)
- **thall**: Thalassemia (1 = Normal, 2 = Fixed defect, 3 = Reversible defect)
- **output**: Target variable (0 = Low risk, 1 = High risk)

## Key Features

- **Data Preprocessing**: Handled missing values, scaled numerical features, and encoded categorical variables.
- **Exploratory Data Analysis (EDA)**: Visualized relationships between features and the target variable.
- **Model Implementation**: Used SVM for binary classification.
- **Performance Metrics**: Evaluated the model using accuracy, precision, recall, and F1-score.

## Requirements

The following Python libraries were used in this project:

- `pandas`
- `numpy`
- `matplotlib`
- `pylab`
- `scipy`
- `scikit-learn`

To install the required libraries, run:

```bash
pip install -r requirements.txt
```

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/HesamNajafi-14/HeartHealth_SVM.git
   ```
2. Navigate to the project directory:
   ```bash
   cd HeartHealth_SVM
   ```
3. Open the Jupyter Notebook or run the Python script:
   ```bash
   jupyter notebook
   ```
   or
   ```bash
   python project_name.py
   ```

## Results

### Classification Report:

```
             precision    recall  f1-score   support

           0       0.91      0.84      0.88        25
           1       0.89      0.94      0.92        36

    accuracy                           0.90        61
   macro avg       0.90      0.89      0.90        61
weighted avg       0.90      0.90      0.90        61
```

### Confusion Matrix (without normalization):

```
[[21  4]
 [ 2 34]]
```

The SVM model achieved an accuracy of 90%, with strong precision, recall, and F1-scores for both classes. Key insights and visualizations are included in the notebook to highlight the relationships between features and the target variable.

## Contributions

Feel free to contribute to this project by submitting issues or pull requests.

## Acknowledgments

This project is inspired by the need to apply machine learning to healthcare to support early diagnosis and prevention of life-threatening conditions.

