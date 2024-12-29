# Snap ML vs. Scikit-Learn: Taxi Tip Prediction

This project demonstrates the use of Snap ML and Scikit-Learn to train and evaluate **Decision Tree Regressor** models on a dataset of New York City taxi trips. It highlights the performance differences in terms of training time and prediction accuracy.

---

## Features
- **Data Preprocessing**: Handles missing values, feature normalization, and categorical encoding.
- **Feature Engineering**: Extracts trip-related features like `pickup_hour`, `trip_time`, and `pickup_day`.
- **Model Training**:
  - Snap ML Decision Tree Regressor.
  - Scikit-Learn Decision Tree Regressor.
- **Performance Comparison**:
  - Training speed.
  - Prediction accuracy using Mean Squared Error (MSE).

---

## Dataset
The dataset used in this project is publicly available from the **NYC Taxi and Limousine Commission (TLC)**. It includes trip data for June 2019. The prediction task focuses on the `tip_amount` variable.

- **Source**: [NYC TLC Trip Records](https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
- **Columns used**:
  - `trip_distance`: Distance traveled during the trip.
  - `fare_amount`: Base fare for the trip.
  - `tip_amount`: Tip amount paid (target variable).
  - `pickup_hour`, `pickup_day`: Extracted from pickup timestamps.
  - `trip_time`: Total trip duration.

---

## Setup and Installation

### Dependencies
To run this project, you will need the following Python libraries:
- Python 3.x
- Snap ML
- Scikit-Learn
- NumPy
- Pandas
- Matplotlib

### Installation Steps
1. **Install required libraries**:
   ```bash
   pip install snapml scikit-learn numpy pandas matplotlib

2. **Verify installation**:
   ```bash
   python -c import snapml, sklearn, numpy, pandas, matplotlib

### Clone the repository

git clone https://github.com/your-username/repository-name.git
cd repository-name


Usage
-----

1. **Preprocessing**:
    - Clean missing data.
    - Normalize features and encode categorical variables.
    - Extract trip-based features (`trip_time`, `pickup_day`, etc.).

2. **Model Training**:
    - Train Decision Tree Regressors with both Snap ML and Scikit-Learn using varying `max_depth` values.
    - Record training times and MSE scores.

3. **Evaluation**:
    - Compare training speeds and prediction accuracy.
    - Use Mean Squared Error (MSE) as the primary evaluation metric.

---

Results
-------

### Training Times

| Model          | Max Depth | Training Time (s) |
|-----------------|-----------|--------------------|
| Snap ML         | 8         | 10.52             |
| Snap ML         | 12        | 24.40             |
| Scikit-Learn    | 8         | 12.85             |

### MSE Scores

| Model          | Max Depth | MSE Score          |
|-----------------|-----------|--------------------|
| Snap ML         | 8         | 1.65483           |
| Snap ML         | 12        | 1.86915           |
| Scikit-Learn    | 8         | 1.63596           |

---

Key Insights
------------

- **Snap ML**:
    - Faster training at smaller depths (`max_depth=8`).
    - Decreased accuracy for larger depths due to overfitting (`max_depth=12`).
- **Scikit-Learn**:
    - Slightly slower training but consistently better accuracy on the test dataset.

---

Conclusion
----------

Snap ML is ideal for large datasets or GPU-enabled systems due to its training speed. Scikit-Learn provides stable and reliable performance for smaller datasets.

---

Acknowledgments
---------------

- **NYC Taxi Dataset**: Provided by NYC Taxi and Limousine Commission (TLC).
- **Snap ML**: High-performance library by IBM.


