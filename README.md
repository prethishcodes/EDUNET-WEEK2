#  Carbon Emission Prediction Using Machine Learning

This project leverages machine learning techniques to forecast per capita CO₂ emissions based on historical and country-specific indicators such as GDP, energy use, and population metrics. Built using Random Forest Regression, the model provides reliable emission forecasts and offers insights that can support data-driven climate policy decisions.

---

##  Project Structure

``` bash
CARBON_EMISSION_PREDICTION/
├── 1_data_preparation.ipynb # Stage 1: Data cleaning and transformation
├── 2_data_exploration.ipynb # Stage 2: Data visualization and correlation analysis
├── 3_model_building.ipynb # Stage 3: Model training, tuning, and forecasting
├── cleaned_climate_data.csv # Cleaned dataset ready for modeling
├── climate_change_download_0.csv # Raw dataset from World Bank
├── forecasting_co2_emmision.pkl # Trained Random Forest model
├── images/
    ├── *.png # All graphs and visual outputs

```
---

---

##  Project Workflow

###  1. Data Preparation
- Cleaned and transformed data from World Bank Climate Change Data.
- Removed nulls, transformed columns, normalized formats.

###  2. Data Exploration
- Analyzed feature relationships using:
  - Correlation heatmaps
  - Scatter plots
  - Outlier analysis
- Focused on energy use, GDP, urbanization.

###  3. Model Building
- Selected top features using RFECV.
- Trained a Random Forest Regressor.
- Tuned with GridSearchCV & validated using 10-fold CV.
- Forecasted emissions for next 20 years using CAGR method.

---

##  Visual Outputs

- `CO₂ Emissions per Capita Over Time.png`
- `Total CO₂ Emissions vs Population.png`
- `Forecasted CO₂ Emissions (Next 20 Years).png`
- `Correlation Between Features.png`
- `Feature Importance.png`


---

##  Tools & Technologies

- Python 3.x
- Jupyter Notebook
- pandas, numpy, matplotlib, seaborn
- scikit-learn (RandomForestRegressor, RFECV, GridSearchCV)
- joblib (for model saving)
- GitHub & Google Drive (for model hosting)

---


##  Forecasting Countries

The model forecasts future emissions for:
- 🇮🇳 India
- 🇺🇸 USA
- 🇵🇰 Pakistan
- 🇷🇺 Russia
- 🇳🇿 New Zealand

---

##  Results

- The Random Forest model delivered R² = 0.978 on test data
- Key predictors: `energy use`, `GDP`, `urbanization`
- Significant forecast variability between developed and developing countries

---

##  Author

**PRETHISH.D**  
B.Tech AI&DS | Er. Perumal Manimekalai College of Engineering

---

##  License

Open-source for academic and research use only.

