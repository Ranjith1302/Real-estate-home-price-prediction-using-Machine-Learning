# 🏠  Real-estate-home-price-prediction-using-Machine-Learning
Regression model in Python to predict house prices based on features like location, area, and number of rooms. • Performed data cleaning, feature engineering, and exploratory analysis to identify key drivers of price variations.



## 📊 Project Overview

The project is divided into:
1. **Data Analysis & Modeling (Backend - ML)**
2. **Web Application (Frontend - Flask)**

We used a dataset with features like:
- Location
- Size (BHK)
- Total square feet
- Number of bathrooms
- Price (target variable)

---

## 🔧 Technologies Used

### 💻 Backend
- Python 3.x
- Jupyter Notebook (for EDA and modeling)
- Pandas, NumPy
- Scikit-learn
- XGBoost, Random Forest, Decision Tree
- Pickle (for saving the trained model)

### 🌐 Frontend
- Flask (Python web framework)
- HTML/CSS
- Bootstrap (for styling)

---

## 🧠 ML Models Evaluated

We evaluated and compared:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost Regressor
- Logistic Regression (experimentally)

Model performance was compared using:
- R² Score
- Root Mean Squared Error (RMSE)

---

## 🖼️ Frontend (Flask App)

The web app allows users to input house details like:
- Area in square feet
- Number of bedrooms (BHK)
- Number of bathrooms
- Location (dropdown)

The app sends the data to the backend, which uses the trained model to return the **predicted price**.

### Example Routes
```python
@app.route('/')
def home():
    return render_template('index.html')

@app.route('/predict', methods=['POST'])
def predict():
    # Handle form input, model prediction, and output
```

---

## 📁 Project Structure


```

---

## ⚙️ How to Run

1. **Clone the repository**

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Flask app**
   ```bash
   python app.py
   ```

4. Open your browser at `http://127.0.0.1:5000` to use the app.

---

## 📌 Results


- Cleaned data and location encoding boosted model performance.
- The Flask app delivers predictions in real-time based on user input.

