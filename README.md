Mobile Phone Price Prediction with Regression Analysis


This repository contains the project deliverables for analyzing a mobile phone dataset to predict prices using multiple linear regression. The project investigates relationships between mobile phone features (screen size, RAM, storage, battery capacity, camera quality) and their prices, using statistical techniques and R programming to uncover consumer preferences and industry trends.

---

🌐 Project Overview
------------------

**Objective**: Analyze a dataset of mobile phone characteristics to build a multiple linear regression model that predicts prices based on features like screen size, RAM, storage, battery capacity, and camera quality, providing insights into pricing determinants and market trends.

---

📊 Dataset Description
---------------------

The dataset contains mobile phone specifications and prices, with the following variables:

🔹 **Price**: The dependent variable representing the cost of the mobile phone (in $).  
🔹 **Screen_Size_inches**: The diagonal measurement of the screen in inches.  
🔹 **RAM_GB**: The amount of Random Access Memory in gigabytes.  
🔹 **Storage_GB**: The internal storage capacity in gigabytes.  
🔹 **Battery_Capacity_mAh**: The battery capacity in milliamp-hours.  
🔹 **Camera_Quality_MP**: The camera quality in megapixels.  

---

🧮 Regression Model
------------------

### Model Formula
The multiple linear regression model is formulated as:

**Price = β0 + β1 * Screen_Size_inches + β2 * RAM_GB + β3 * Storage_GB + β4 * Battery_Capacity_mAh + β5 * Camera_Quality_MP + ε**

🔹 **β0**: Intercept term representing the baseline price.  
🔹 **β1, β2, β3, β4, β5**: Regression coefficients indicating the impact of each independent variable on price.  
🔹 **ε**: Error term representing unexplained variability.  

### Coefficients and Interpretation
🔹 **Intercept (β0)**: Estimated at 1001.72, representing the baseline price when all independent variables are zero.  
🔹 **Screen_Size_inches (β1)**: Each additional inch increases price by ~90 units, indicating a significant positive relationship.  
🔹 **RAM_GB (β2)**: Each additional GB of RAM increases price by ~35 units, reflecting demand for performance.  
🔹 **Storage_GB (β3)**: Each additional GB of storage increases price by ~0.35 units, highlighting storage’s role in pricing.  
🔹 **Battery_Capacity_mAh (β4)**: Each additional mAh increases price by ~0.09 units, suggesting a weaker influence.  
🔹 **Camera_Quality_MP (β5)**: Each additional megapixel increases price by ~2.4 units, indicating strong consumer preference for camera quality.  

### Model Fit and Significance
🔹 **Adjusted R-squared**: 0.1202, indicating that ~12.02% of price variability is explained by the model, suggesting a moderately weak fit.  
🔹 **Residual Standard Error**: 124.4, representing the average distance of data points from the fitted regression line.  
🔹 **F-statistic**: 20.87 with a p-value of 3.412e-09, confirming the model’s statistical significance and meaningful relationships between variables.  
🔹 **Significance**: All coefficients are significant at a 0.05 level, confirming that screen size, RAM, storage, battery capacity, and camera quality significantly influence price.  

---

📈 Key Insights
--------------

- **Feature Impact**: Screen size, RAM, and camera quality have stronger positive impacts on price, reflecting consumer preferences for larger screens, better performance, and high-quality cameras.  
- **Market Trends**: Moderate correlations between price and features like RAM suggest performance-driven pricing strategies, while weaker correlations with storage and battery capacity indicate these are secondary factors.  
- **Implications**: Manufacturers can use these insights for pricing strategies and product differentiation, while consumers gain clarity on price determinants for informed purchasing decisions.  
- **Limitations**: The model’s low R-squared (12.02%) suggests other factors (e.g., brand, design) may influence pricing, and linearity assumptions may limit accuracy.  

---

⚠️ Challenges and Considerations
------------------------------

- **Model Fit**: The adjusted R-squared of 0.1202 indicates a moderately weak fit, suggesting unmodeled factors or non-linear relationships.  
- **Overfitting Risk**: Including multiple variables may lead to overfitting, requiring validation with additional data.  
- **Data Limitations**: The dataset may not capture all relevant factors (e.g., brand value, software features) affecting mobile phone prices.  
- **Linearity Assumption**: Linear regression assumes linear relationships, which may not fully capture complex pricing dynamics.  

---

📁 Project Structure
-------------------

```plaintext
.
├── data/
│   └── mobile_phone_dataset.csv  # Dataset with mobile phone features and prices
├── src/
│   └── analysis.R                # R script for regression analysis and visualizations
├── docs/
│   └── Analysis Report.docx      # Detailed project report with results and interpretations
├── README.md                     # Project documentation
└── requirements.txt              # R dependencies
```

---

🛠️ Installation
--------------

### Prerequisites
🔹 **R**: Version 4.0 or later  
🔹 **R Libraries**: Listed in `requirements.txt` (e.g., `ggplot2`, `dplyr`)  

### Setup
- **Clone the Repository**:  
  ```bash
  git clone https://github.com/username/mobile-price-prediction.git
  cd mobile-price-prediction
  ```

- **Install Dependencies**:  
  ```bash
  Rscript -e "install.packages(readLines('requirements.txt'))"
  ```

- **Run the Analysis**:  
  ```bash
  Rscript src/analysis.R
  ```

---

📖 Usage
-------

- **Run the R Script**: Execute `src/analysis.R` to perform regression analysis and generate visualizations (e.g., scatterplots, boxplots).  
- **View Results**: Check the `docs/Analysis Report.docx` for detailed results, including regression coefficients, model fit, and interpretations.  
- **Explore Visualizations**: Review scatterplots and boxplots in the report to understand correlations between features and price.  

---

💡 Recommendations
-----------------

- **Enhance Model**: Incorporate additional variables (e.g., brand, processor type) to improve R-squared and model fit.  
- **Non-Linear Models**: Explore polynomial regression or machine learning models (e.g., random forests) to capture non-linear relationships.  
- **Cross-Validation**: Apply k-fold cross-validation to assess model robustness and prevent overfitting.  
- **Larger Dataset**: Use a more comprehensive dataset to improve generalizability and capture diverse market trends.  

---

## 👨‍💻 Contributors
- **Abdullah Daoud (22I-2626)**  
- **Talha Rizwan (22I-2539)**  

---

## ⚖️ License
This project is for **academic and personal skill development purposes only**.  
Reuse is allowed for **learning and research** with proper credit.

---
