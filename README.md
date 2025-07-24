
# 🏠 House Price Prediction Tool

An interactive house price prediction system built using **Python**, **SQLite**, **scikit-learn**, **Plotly**, and **ipywidgets**. It allows users to:
- Add custom house entries
- Predict their price using a linear regression model
- Visualize price trends and statistics

> 🚀 Designed to run in Google Colab with an easy-to-use interactive interface!

---

## 📦 Features

- 📊 Predict house prices using `LinearRegression`
- 💾 Store house data persistently using SQLite
- 🧮 Real-time prediction as users enter data
- 📈 Visualize trends with dynamic Plotly charts
- 🧠 Retrain model as new data is added (optional feature)

---

## 📁 Sample Dataset

Initial sample data:

| Size (sqft) | Bedrooms | Location  | Price ($) |
|-------------|----------|-----------|-----------|
| 1200        | 2        | Urban     | 200,000   |
| 1500        | 3        | Suburban  | 250,000   |
| 1000        | 1        | Rural     | 150,000   |
| 1800        | 4        | Urban     | 300,000   |

---

## 🛠️ Installation & Run (in Google Colab)

1. Open the `.ipynb` file in Google Colab
2. Run the following cells:

```python
!pip install --upgrade plotly ipywidgets scikit-learn
```

3. Enable widgets:

```python
from google.colab import output
output.enable_custom_widget_manager()
```

4. Run all cells to initialize the database, train the model, and start interacting.

---

## 🎮 Interactive Widgets

| Widget        | Description                    |
|---------------|--------------------------------|
| Size Slider   | Adjust house size (sqft)       |
| Bedrooms      | Select number of bedrooms      |
| Location      | Choose from Urban/Suburban/Rural |
| Add House     | Predict and add new house data |
| Visualizations| Show scatter & bar charts      |

---

## 📉 Visualizations

- **Scatter Plot** – House Size vs. Predicted Price (colored by location)
- **Bar Chart** – Average Price by Location
- **Summary Stats** – Average price, total house entries

---

## 🧠 Model

- Uses `sklearn.linear_model.LinearRegression`
- Encodes `location` manually (`Urban` = 1, `Suburban` = 0, `Rural` = 2)
- Can be retrained dynamically on updated dataset

---

## 💡 Future Enhancements

- Use `OneHotEncoder` for better location encoding
- Add data validation (e.g. no 0-bedroom homes)
- Normalize features for improved accuracy
- Export predictions as CSV

---

## 📌 Requirements

- Python 3.x
- Google Colab (recommended)
- Libraries:
  - `scikit-learn`
  - `pandas`
  - `numpy`
  - `plotly`
  - `ipywidgets`
  - `sqlite3`

---

## 🧑‍💻 Author

**Khushi Shukla**  
👩‍🎓 B.Tech in CSE (Data Science) – BBDITM  
📍 Lucknow, India
