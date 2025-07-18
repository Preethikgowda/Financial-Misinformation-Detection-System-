# 📊 Financial Misinformation Detection & Stock Market Prediction System

This project is a **Streamlit-based AI application** that performs two key tasks:

1. ✅ **Detects Financial News Misinformation** using **OpenAI's GPT-4**
2. 📈 **Predicts Stock Market Closing Prices** using a hybrid **LSTM + XGBoost model**

---

## 🚀 Features

### 🧠 Financial Misinformation Detection
- Users can input any financial news/article
- GPT-4 evaluates the accuracy of the content
- Provides supporting context and explanations for its judgment

### 📉 Stock Market Predictor
- Accepts a stock ticker (e.g., `AAPL`, `TSLA`, `NSE:INFY`)
- Downloads historical data using `yfinance`
- Uses an **LSTM neural network** to extract patterns
- Boosts results with **XGBoost** for enhanced accuracy
- Outputs the predicted closing price for the next day

---

## 🛠️ Tech Stack

| Component        | Technology                             |
|------------------|----------------------------------------|
| Frontend         | Streamlit                              |
| AI Model (LLM)   | OpenAI GPT-4 via `openai` Python SDK   |
| Data Source      | Yahoo Finance API via `yfinance`       |
| ML Models        | LSTM (Keras), XGBoost (xgboost)        |
| Preprocessing    | NumPy, Scikit-learn                    |

---

#### 🧪 Installation and Setup

 ### ✅ Prerequisites
- Python 3.8+
- An OpenAI API Key ([Get one here](https://platform.openai.com/account/api-keys))

### 📁 Clone the Repository
```bash
git clone https://github.com/Preethikgowda/Financial-Misinformation-Detection-System-.git
cd Financial-Misinformation-Detection-System-
```
### 🔒 Create .env File for OpenAI Key
env
``` Python
OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```
### 📦 Install Dependencies
Create a virtual environment (optional but recommended):
```
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```
### install required packages:

```
pip install streamlit openai yfinance numpy keras scikit-learn xgboost python-dotenv
```
▶️ Run the App
```
streamlit run app.py
```
The app will open in your default browser at:
http://localhost:8501

### 🖥️ Project Structure

📦 Financial-Misinformation-Detection-System-
│
├── app.py                   # Main Streamlit app file
├── .env                     # Environment file for API key
├── README.md                # Project documentation
└── requirements.txt         # Python dependencies

### 💡 Future Improvements

Add caching for faster performance

Pre-train and store ML models for instant prediction

Display stock chart with prediction overlay

Add model evaluation metrics (R², MAE, etc.)

Use real-time news APIs to feed the LLM

### 🙋‍♀️ Author
Preethi T K
Preethikgowda26@gmail.com

### 📄 License
This project is for educational and research purposes only.
Make sure to independently verify any financial predictions before making decisions.
