🚦 Traffic Flow Prediction Using Machine Learning
This project explores how machine learning techniques—specifically LSTM and Random Forest Regressors—can be used to forecast traffic flow patterns based on historical urban traffic data. The study evaluates model performance, highlights feature importance, and discusses the practical application of these models in intelligent transportation systems.

📌 Overview
Urban traffic congestion is a growing challenge. Accurate traffic flow prediction can improve mobility, reduce travel time, and support smarter city planning. In this project:

LSTM (Long Short-Term Memory) models time-series traffic patterns.

Random Forest models extract insights using engineered features.

Performance is evaluated using MAE and MSE.

🧠 Models Used
1. Long Short-Term Memory (LSTM)
Sequence length: 24 hours

Optimizer: Adam

Loss function: Mean Squared Error (MSE)

Advantage: Captures sequential dependencies in traffic data

2. Random Forest Regressor
Trained on feature-engineered data

Interpretable results using feature importance

Advantage: Fast training and strong performance on tabular data

🗂️ Dataset Description
Features:

DateTime (used to extract hour, day, and month)

Vehicle count

Traffic junction identifiers

Preprocessing:

Temporal feature extraction

One-hot encoding for junctions

Scaling (StandardScaler for Random Forest, MinMaxScaler for LSTM)

Train/test split

📊 Evaluation Metrics
Mean Absolute Error (MAE)

Mean Squared Error (MSE)

Model	MAE	MSE
LSTM	17.35	537.16
RandomForest	8.21	145.90
📈 Results
Random Forest outperformed LSTM in terms of prediction accuracy and interpretability.

LSTM effectively modeled sequential patterns but was computationally more intensive.

Feature importance analysis showed that hour of day and day of week were key predictors.

🔍 Error Analysis
Random Forest: Showed a consistent error distribution.

LSTM: Occasionally overestimated during peak hours.

🚀 Future Work
Integrate external features like weather, public holidays, and road conditions.

Deploy best-performing model in a real-time traffic monitoring system.

Explore hybrid models combining LSTM and Random Forest.

📚 References
Hochreiter & Schmidhuber (1997). Long Short-Term Memory.

Breiman, L. (2001). Random Forests.

Hyndman & Athanasopoulos (2018). Forecasting: Principles and Practice.

Box et al. (2015). Time Series Analysis: Forecasting and Control.

👥 Contributors
Hantz Brunet Guerrier

Hantz 古弘恩

Max 田雷西

Arridson 范瑞德
