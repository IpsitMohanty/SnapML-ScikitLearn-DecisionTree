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
- Python 3.x
- Snap ML
- Scikit-Learn
- NumPy
- Pandas
- Matplotlib

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/repository-name.git
   cd repository-name
