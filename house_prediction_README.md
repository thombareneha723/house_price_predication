# 🏡 USA House Price Prediction

This project predicts **house prices in the USA** using machine learning (Linear Regression).  
The trained model achieves an **RMSE of ~100k**, making it useful for real estate price estimation and decision-making.

---

## 📂 Project Structure
- **Predicted_House_Prices.ipynb** → Jupyter Notebook with data preprocessing, training, and evaluation.  
- **USA house price prediction model 100k rmse 25-08-25.pkl** → Trained model file saved with `joblib`.  
- **requirements.txt** → Python dependencies required to run the project.  
- **README.md** → Project documentation.  

---

## 📊 Overview
The aim of this project is to build a model that can predict house prices in the USA based on different features such as:  
- Number of bedrooms  
- Number of bathrooms  
- Square footage  
- Year built  
- Other housing attributes  

The notebook (`Predicted_House_Prices.ipynb`) contains:  
1. Data loading and exploration  
2. Data preprocessing  
3. Model training (Linear Regression)  
4. Model evaluation using RMSE  
5. Saving the model as a `.pkl` file  

---

## 📁 Dataset
- **Source**: Public housing dataset (Kaggle or other).  
- **Features**: Housing attributes (bedrooms, bathrooms, area, year, etc.).  
- **Target**: House price.  

---

## ⚙️ Installation

1. **Clone this repository**
   ```bash
   git clone https://github.com/thombareneha723/house_price_predication.git
   cd house_price_predication
2.(Optional) Create a virtual environment
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
3.pip install -r requirements.txt

Usage

1.Run the Notebook
jupyter notebook Predicted_House_Prices.ipynb
2.Load the trained model in Python
import joblib

# Load model
model = joblib.load("USA house price prediction model 100k rmse 25-08-25.pkl")

# Example input: [bedrooms, bathrooms, sqft, year_built]
sample_input = [[3, 2, 1500, 2005]]

prediction = model.predict(sample_input)
print("Predicted Price:", prediction)



