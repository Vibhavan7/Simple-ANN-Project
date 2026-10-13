# Simple ANN Project — Customer Churn Prediction

A deep learning project that predicts whether a bank customer will churn (leave the bank) using an **Artificial Neural Network (ANN)** built with TensorFlow/Keras. The model is served through an interactive **Streamlit** web application.

## 🚀 Demo

The Streamlit app allows users to input customer details and get a real-time churn prediction.

**Input Features:**
| Feature | Description |
|---------|-------------|
| Geography | Customer's country (One-Hot Encoded) |
| Gender | Male / Female (Label Encoded) |
| Credit Score | Customer's credit score |
| Age | Customer's age |
| Tenure | Number of years with the bank |
| Balance | Account balance |
| Number of Products | Number of bank products used |
| Has Credit Card | Whether the customer has a credit card (0/1) |
| Is Active Member | Whether the customer is an active member (0/1) |
| Estimated Salary | Customer's estimated salary |

## 🛠️ Tech Stack

- **Python 3.x**
- **TensorFlow / Keras** — ANN model training and inference
- **Scikit-learn** — Preprocessing (StandardScaler, LabelEncoder, OneHotEncoder)
- **Pandas & NumPy** — Data manipulation
- **Streamlit** — Web app for predictions

## 📁 Project Structure

```
Simple-ANN-Project/
├── app.py                      # Streamlit web application
├── model.h5                    # Trained ANN model
├── scaler.pkl                  # Fitted StandardScaler
├── label_encoder_gender.pkl    # Fitted LabelEncoder for Gender
├── onehot_encoder_geo.pkl      # Fitted OneHotEncoder for Geography
├── Churn_Modelling.csv         # Dataset
├── experiments.ipynb           # Model training & experimentation notebook
├── prediction.ipynb            # Prediction notebook
├── requirement.txt             # Python dependencies
├── .gitignore
└── README.md
```

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/Vibhavan7/Simple-ANN-Project.git
   cd Simple-ANN-Project
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv

   # Windows
   .\venv\Scripts\activate

   # macOS/Linux
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirement.txt
   ```

4. **Run the Streamlit app**
   ```bash
   streamlit run app.py
   ```

## 📊 How It Works

1. **Data Preprocessing** — The dataset (`Churn_Modelling.csv`) is preprocessed using Label Encoding (Gender), One-Hot Encoding (Geography), and Standard Scaling.
2. **Model Training** — An ANN is trained using TensorFlow/Keras (see `experiments.ipynb`).
3. **Prediction** — The trained model (`model.h5`) along with the fitted encoders and scaler are loaded in `app.py` to make real-time predictions via Streamlit.

## 📝 License

This project is open source and available for learning purposes.
