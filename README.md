# Laptop-Price-Prediction


## ▶️ To Run Locally

```
# Clone the repository
git clone https://github.com/your-username/Laptop-Price-Predictor.git
cd Laptop-Price-Predictor

# (Optional) create a virtual environment
python -m venv venv
source venv/bin/activate  # For Linux/Mac
venv\Scripts\activate     # For Windows

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py
```

## 🐳 Docker Support

```
docker build -t laptop-price-predictor .
docker run -p 8501:8501 laptop-price-predictor
```
# 💻 Laptop Price Predictor

A machine learning-powered Streamlit web application that predicts laptop prices based on configuration inputs like brand, CPU, RAM, display, storage, and more.

---

## 📊 Project Objective

The goal is to build an intelligent system that estimates the market price of laptops based on various technical specifications using a regression model trained on real-world data.

---

## ⚙️ Features

- Intuitive web UI with Streamlit
- Custom user inputs including brand, screen size, storage, etc.
- Real-time price prediction using trained regression model
- Preprocessing pipeline embedded with model for clean inference

---

## 🧾 Input Parameters

| Feature         | Description                                  |
|------------------|----------------------------------------------|
| Company          | Laptop brand                                 |
| TypeName         | Type (Ultrabook, Gaming, Notebook, etc.)     |
| RAM              | RAM size in GB                               |
| Weight           | Laptop weight in kilograms                   |
| Touchscreen      | Yes/No                                       |
| IPS Display      | Yes/No                                       |
| Screen Size      | Display size in inches                       |
| Resolution       | Screen resolution (e.g., 1920x1080)          |
| CPU Brand        | Brand of processor                           |
| HDD              | Size of HDD in GB                            |
| SSD              | Size of SSD in GB                            |
| GPU Brand        | Graphics card brand                          |
| OS               | Operating system                             |

---

## 🧠 ML Pipeline

1. Data loaded from `laptop_data.csv`
2. Feature engineering and transformations
3. Regression model training (e.g., Linear Regression / Random Forest)
4. Model + preprocessing pipeline exported as `pipe.pkl`
5. App interface built with Streamlit (`app.py`)

---

## 🗂 Project Structure

Laptop-Price-Predictor/
├── app.py # Streamlit UI logic
├── pipe.pkl # Trained model + transformer pipeline
├── df.pkl # Reference dataframe for dropdowns
├── laptop_data.csv # Original dataset
├── Dockerfile # Docker setup (for containerized deployment)
├── laptop-price-predictor.ipynb # Model training and EDA
└── README.md # Project documentation





