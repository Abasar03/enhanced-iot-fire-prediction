# Enhanced IoT Fire Prediction

This project focuses on building an advanced predictive analytics framework for fire detection using IoT sensor data. It explores data preprocessing, K-Means clustering, PCA dimensionality reduction, ADASYN resampling, and model comparison using supervised learning techniques.

## Project Workflow

1. **Exploratory Data Analysis (EDA)**
   - Confirmed no missing values
   - Visualized distributions with histograms, box plots, and scatter plots

2. **Data Preprocessing**
   - Extracted temporal features: hour, dayofweek, weekend
   - Aggregated gas sensor values into AQI
   - Calculated potential_fire score: smoke × temp
   - Defined binary fire risk indicator using threshold
   - Encoded categorical features with one-hot encoding
   - Scaled numerical features with z-score normalization

3. **Feature Engineering**
   - Applied sine and cosine transformations to hour and dayofweek
   - Derived humidity_temp_diff: humidity - temp

4. **Model Training & Evaluation**
   - Trained and evaluated models using stratified sampling
   - Models: Logistic Regression, KNN, Random Forest, XGBoost, LightGBM, CatBoost
   - Performance metrics: accuracy, precision, recall, F1-score, ROC AUC
   - Random Forest achieved best results: Cluster 0 F1-score 0.989, Cluster 1 F1-score 0.975, ROC AUC 0.996

## How to Run

1. Clone the repository
   ```
   git clone https://github.com/username/enhanced-iot-fire-prediction
   ```

2. Navigate to the project directory
   ```
   cd enhanced-iot-fire-prediction
   ```

3. Install the dependencies
   ```
   echo INSERT INSTALL COMMAND HERE
   ```

4. Run the project
   ```
   echo INSERT RUN COMMAND HERE
   ```

## Testing

The project uses the best framework test framework. Run the test suite with:
   ```
   echo INSERT TEST COMMAND HERE
   ```