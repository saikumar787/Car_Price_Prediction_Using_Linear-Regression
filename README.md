
# 🚗 Car Price Prediction using Machine Learning

This project predicts the selling price of a used car based on features such as year, fuel type, kilometers driven, seller type, and more.

## 📂 Files Included

- `cars.csv` — The dataset containing used car listings with features like year, present price, kms driven, fuel type, seller type, transmission, etc.
- `Car_Price_Prediction.ipynb` — Jupyter Notebook for:
  - Exploratory Data Analysis (EDA)
  - Data preprocessing (handling categorical features using OneHotEncoding)
  - Model training using Linear Regression
  - Evaluation and visualization
- `model.pkl` — The trained machine learning model saved using `joblib`.
- `ss.pkl` — StandardScaler object used to scale input features before prediction.
- `testing_on_newdata.ipynb` — A separate notebook used to test the saved model on new data inputs.

## 🧠 Model Overview

- **Model Used**: Linear Regression
- **Target Variable**: Selling Price
- **Features Used**:
  - Year
  - Present Price
  - Kms Driven
  - Fuel Type (converted using one-hot encoding)
  - Seller Type
  - Transmission

## 📈 Example Prediction

```python
new_data = np.array([[2018, 8.5, 25000, 0, 1, 1]])  # Encoded input
scaled = scaler.transform(new_data)
price = model.predict(scaled)
print("Predicted Price:", price)
```

## ✅ Requirements

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- joblib

Install them using:

```bash
pip install -r requirements.txt
```

## 📌 How to Use

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/Car-Price-Prediction.git
   ```

2. Open `Car_Price_Prediction.ipynb` to train the model or understand the process.

3. Use `testing_on_newdata.ipynb` to test the model on unseen data.

## 👨‍💻 Author

- Venkata Sai Kumar Routhu
