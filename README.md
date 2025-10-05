📄 Project Documentation
🧠 Objective
Build a machine learning system to predict e-commerce delivery time using order, agent, and external condition features.
📦 Dataset
Contains order IDs, location coordinates, agent info, order/pickup time, weather, traffic, and actual delivery duration.
🛠 Steps Covered
1.	Data Preprocessing
a.	Missing value handling, datetime parsing, category encoding
2.	Feature Engineering
a.	Distance calculation (Haversine/Geodesic)
b.	Time features: hour, weekday, pickup delay
3.	EDA
a.	Understand impact of weather, traffic, agent, and time
4.	Model Training
a.	Models used: Linear Regression, Random Forest, Gradient Boosting
b.	Evaluated using RMSE, MAE, R²
c.	Logged via MLflow
5.	Deployment
a.	Streamlit app for real-time prediction
b.	Accepts all relevant input fields
🔧 Tools Used
•	Python, Pandas, Scikit-learn, XGBoost
•	Matplotlib, Seaborn
•	MLflow for model tracking
•	Streamlit for deployment
📊 Results
•	Gradient Boosting performed best with lowest RMSE
•	Insights into how weather and traffic significantly affect delivery time

