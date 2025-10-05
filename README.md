🚚 Amazon Delivery Time Prediction
🧠 Objective

This project builds a machine learning model to predict e-commerce delivery times using order details, delivery agent information, and external conditions such as weather and traffic.

📦 Dataset

The dataset includes:

Order details: IDs, timestamps (order/pickup/delivery)

Agent info: ratings, experience

Location data: pickup and drop-off coordinates

External features: weather conditions, traffic levels

Target variable: actual delivery duration (in minutes)

🛠 Steps Covered
1. Data Preprocessing

Handled missing values

Parsed datetime fields

Encoded categorical features

2. Feature Engineering

Calculated distances using Haversine/Geodesic methods

Extracted time-based features (hour, weekday, pickup delay)

3. Exploratory Data Analysis (EDA)

Analyzed the effect of weather, traffic, and agent performance on delivery time

Visualized key trends and correlations

4. Model Training

Algorithms used:

Linear Regression

Random Forest

Gradient Boosting

Evaluation Metrics:

RMSE, MAE, R² Score

Model tracking and comparison via MLflow

5. Deployment

Built a Streamlit web app for real-time delivery time prediction

Users can input all relevant features to get instant predictions

🔧 Tools & Libraries

Python

Pandas, NumPy, Scikit-learn, XGBoost

Matplotlib, Seaborn

MLflow (for model tracking)

Streamlit (for deployment)

📊 Results

Gradient Boosting delivered the lowest RMSE, outperforming other models

Key Insight: Weather and traffic conditions are major contributors to delivery delays

🚀 Future Improvements

Incorporate real-time weather and traffic APIs

Experiment with deep learning models (e.g., LSTM for time-series patterns)

Deploy as a cloud-based service (AWS/GCP/Azure)

💻 How to Run Locally
# Clone the repository
git clone https://github.com/your-username/amazon-delivery-time-prediction.git
cd amazon-delivery-time-prediction

# Install dependencies
pip install -r requirements.txt

# Run the Streamlit app
streamlit run app.py
