# 📈 Apple Stock Price Predictor

A Machine Learning-based web app that predicts **Apple Inc. (AAPL)** stock prices for the next 30 days using **SARIMAX** and **Streamlit**.  
It takes recent stock data as input and forecasts future closing prices while visualizing the trend interactively.

---

## 🚀 Features
- 📊 Forecasts next 30 days of AAPL stock prices  
- 🧠 Uses SARIMAX (Time-Series Model) trained on historical data  
- 🧾 Accepts CSV files with columns: `Open, High, Low, Close, Volume`  
- 📈 Interactive line charts for historical vs. predicted prices  
- ⚙️ Scaled data preprocessing for better prediction stability  
- 🌐 Built with Streamlit for an easy-to-use web interface  

---

## 🧩 Tech Stack
| Category | Tools |
|-----------|--------|
| **Language** | Python |
| **Framework** | Streamlit |
| **Libraries** | pandas, numpy, joblib, statsmodels, matplotlib |
| **Model** | SARIMAX |
| **Files** | `best_model.pkl`, `scaler_y.pkl`, `scaler_X_sarimax.pkl` |

---

## 📂 Project Structure
```Apple_Stock_Price_Predictor/
│
├── app.py # Streamlit app
├── APPLE_Stock_Price_Predictor.ipynb # Jupyter Notebook (Model training)
├── best_model.pkl # Trained SARIMAX model
├── scaler_y.pkl # Scaler for target variable
├── scaler_X_sarimax.pkl # Scaler for exogenous variables
├── README.md # Project documentation
└── requirements.txt # Dependencies (see below) ```


---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/<your-username>/Apple_Stock_Price_Predictor.git
cd Apple_Stock_Price_Predictor

2️⃣ Create a Virtual Environment
python -m venv venv
venv\Scripts\activate        # For Windows
source venv/bin/activate     # For Mac/Linux

3️⃣ Install Dependencies

Create a requirements.txt file with:

streamlit
pandas
numpy
joblib
matplotlib
statsmodels


Then run:

pip install -r requirements.txt

4️⃣ Run the App
streamlit run app.py


Then open the local URL (e.g. http://localhost:8501) to view your app.

📊 Usage

Upload a CSV file containing at least 30 days of recent Apple stock data.

Ensure columns include: Open, High, Low, Close, Volume.

Choose forecast horizon (1–60 days).

View prediction chart and forecast table.

🧠 Model Description

The app uses a SARIMAX model trained on APPL’s historical data to capture seasonality and trends.
Scaling is applied to both features and target to maintain prediction accuracy.

📸 Demo Screenshot 

c:\Users\brije\OneDrive\Pictures\Screenshots\Screenshot (1).png
👨‍💻 Author

Brijesh Kumar
📧 https://www.linkedin.com/in/brijeshbaghel250/
💼 Aspiring Data Scientist | Machine Learning Enthusiast

🏷️ License

This project is open-source and available under the MIT License
.