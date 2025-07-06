# 🌬️ Air Quality Index (AQI) Prediction

## 📌 Project Overview & Task Objective

This notebook addresses the severe air pollution issue in Delhi by developing a machine learning model to predict the Air Quality Index (AQI). The objective is to leverage historical data on various pollutants (e.g., PM2.5, PM10, NO₂, etc.) to build and evaluate regression models. The ultimate goal is to understand key pollution trends and enable early warnings through data-driven AQI forecasting.

## 📂 Dataset Information

The project utilizes historical air quality data for Delhi, which typically includes measurements of various pollutants and the corresponding AQI. The dataset would contain features such as `City`, `Date`, `PM2.5`, `PM10`, `NO`, `NO2`, `NOx`, `NH3`, `CO`, `SO2`, `O3`, `Benzene`, `Toluene`, `Xylene`, `AQI`, and `AQI_Bucket`.

**Key Aspects:**
- Time-series data of air pollutant concentrations.
- Regression problem to predict AQI.
- Requires handling of missing values and potentially time-based feature engineering.

## ✨ Features

- Data loading and initial inspection.
- Handling missing values through imputation or removal.
- Exploratory Data Analysis (EDA) to understand pollutant distributions and trends.
- Feature engineering from date/time information.
- Training and evaluating various regression models (e.g., Linear Regression, Random Forest Regressor).
- Model evaluation using metrics such as Mean Squared Error (MSE) and R-squared score.

## 🛠️ Installation

To run this notebook locally, you will need Python installed along with the following libraries. You can install them using pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 🚀 Approach

My approach to AQI prediction involved the following steps:

- **Library Import**: Imported essential Python libraries for data manipulation (pandas, numpy), visualization (matplotlib, seaborn), and machine learning (sklearn).
  
- **Data Loading**: Loaded the air quality dataset into a pandas DataFrame.

- **Data Cleaning and Preparation**:
  - Identified and handled missing values in pollutant concentration columns.
  - Converted `Date` column to datetime objects and extracted time-based features (e.g., month, day of week).
    
- **Exploratory Data Analysis (EDA)**:
  - Analyzed the distribution of AQI and individual pollutants.
  - Explored temporal trends of pollutants and AQI.
  - Visualized relationships between different pollutants and AQI.
  
- **Model Training and Testing**:
  - Split the dataset into training and testing sets.
  - Trained multiple regression models, such as Linear Regression and Random Forest Regressor, to predict AQI.

- **Model Evaluation**: Evaluated the trained models using regression metrics like Mean Squared Error (MSE) and R-squared score to assess their predictive performance.

## 🧰 Technologies Used
- P Y T H O N
- P A N D A S
- N U M P Y
- M A T P L O T L I B
- S E A B O R N
- S C I K I T - L E A R N

## 📉 Visualizations

### Pollutants Over Time
![image](https://github.com/user-attachments/assets/ce4f7490-7345-4130-8065-dc77bb1cae02)

**Insights:**
PM2.5 and PM10 spike in winters (Nov–Jan) O3 and SO2 are less volatile Strong seasonal trends observed

### Correlation between Pollutants and AQI
![image](https://github.com/user-attachments/assets/86f93bc8-07a2-4d37-be7a-676b58a81318)

**Insights:**
AQI is highly correlated with PM2.5 (0.94) and PM10 (0.89) Moderate correlation with NO, NO2, CO O3 and SO2 have weaker correlation ✅ Why: Guides feature selection — strong predictors help model accuracy.

### Actual vs Predicted AQI
![image](https://github.com/user-attachments/assets/07b96feb-d6eb-44a4-9369-67a6c44dd861)

**Insights:**
- Random Forest closely follows actual AQI
- Linear regression misses peaks and drops
- Confirms that AQI behavior is non-linear

## 📊 Results and Insights

- PM2.5 and PM10 are the most significant contributors to AQI levels.
- Seasonal patterns were observed, with higher AQI in winter months.
- Random Forest outperformed Linear Regression, effectively capturing the non-linear relationships between   pollutants and AQI.
- Random Forest showed better generalization and more accurate AQI classification.
- Models are effective for real-time AQI forecasting and can support alert systems for public health         monitoring.

## 🧪 Usage

```bash
# 1. Clone the repository (assuming this notebook is part of a larger repository)
git clone https://github.com/AhsanNFt/Air-Quality-Prediction.git

# 2. Navigate to the project directory
cd Air-Quality-Prediction

# 3. Open the notebook
jupyter notebook Air_Quality_Detection_Main.ipynb

```

## 🤝 Contributing

Contributions are welcome! If you have any suggestions or improvements, please open an issue or submit a pull request.

## 📬 Contact

For questions or collaboration:
- GitHub: [Your GitHub Username]
- Email: [Your Email Address]


