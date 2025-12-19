📉 Customer Churn Prediction Web App

A Streamlit-based machine learning application that predicts whether a customer is likely to churn (leave the service) based on demographic and financial features. The app uses a pre-trained TensorFlow/Keras model along with saved encoders and scalers to ensure consistent predictions.

⸻

🚀 Features (Implemented & Accurate)
	•	🧾 Interactive form to input customer details
	•	🧠 Predicts customer churn probability using a trained ML model
	•	📊 Displays churn probability as a numeric value
	•	✅ Binary churn decision based on probability threshold (0.5)
	•	🔁 Uses saved preprocessing objects (LabelEncoder, OneHotEncoder, StandardScaler)
	•	🖥️ Simple and clean Streamlit interface

⸻

🧠 Model Details
	•	Model Type: Neural Network (TensorFlow / Keras)
	•	Framework: TensorFlow
	•	Task: Binary classification (Churn / No Churn)
	•	Model File: model.h5

Preprocessing Objects Used
	•	label_encoder_gender.pkl – encodes Gender
	•	onehot_encoder_geo.pkl – one-hot encodes Geography
	•	scaler.pkl – standardizes numerical features

These are loaded and applied exactly as used during model training.

⸻

🧩 Input Features Used
	•	Credit Score
	•	Gender (encoded)
	•	Age
	•	Tenure
	•	Account Balance
	•	Number of Products
	•	Has Credit Card (0 / 1)
	•	Is Active Member (0 / 1)
	•	Estimated Salary
	•	Geography (one-hot encoded)

⸻

🛠️ Tech Stack
	•	Frontend: Streamlit
	•	Machine Learning: TensorFlow / Keras
	•	Data Processing: Pandas, NumPy
	•	Preprocessing: Scikit-learn (Encoders, Scaler)
	•	Model Persistence: Pickle

⸻

⚙️ Installation & Setup

1️⃣ Clone the Repository
``` bash
git clone https://github.com/your-username/customer-churn-prediction.git
cd customer-churn-prediction
```
2️⃣ Create Virtual Environment (Recommended)
``` bash
python -m venv venv
source venv/bin/activate   # macOS / Linux
venv\Scripts\activate    # Windows
```
3️⃣ Install Required Libraries
``` bash
pip install streamlit tensorflow scikit-learn pandas numpy
```
4️⃣ Place Required Files
``` bash
Ensure the following files are present in the project directory:

model.h5
label_encoder_gender.pkl
onehot_encoder_geo.pkl
scaler.pkl
```
5️⃣ Run the Application
``` bash
streamlit run app.py
```

⸻

🧪 How the Application Works
	1.	User enters customer details via UI
	2.	Gender is label-encoded
	3.	Geography is one-hot encoded
	4.	Numerical features are scaled using StandardScaler
	5.	Processed input is passed to the trained model
	6.	Churn probability is predicted and displayed
	7.	Final decision is shown based on threshold (0.5)

⸻

📌 Output
	•	Churn Probability (0 to 1)
	•	Decision Message:
	•	Likely to churn
	•	Not likely to churn

⸻

🔐 Limitations (Current Implementation)
	•	Fixed probability threshold (0.5)
	•	No confidence interval or explanation of prediction
	•	No model retraining from UI
	•	Assumes correct preprocessing files are present

⸻

📈 Future Scope (Not Implemented)
	•	Adjustable churn threshold
	•	Feature importance visualization
	•	SHAP / explainability integration
	•	Database or CSV input support
	•	Deployment on cloud platforms

⸻

👨‍💻 Author

Lokesh
Student | AI / ML | Deep Learning

⸻

📜 License

This project is intended for academic and educational purposes.

⸻

Customer churn prediction helps businesses take proactive retention actions. 🚀
