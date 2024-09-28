# Forecasting Agricultural CO2 Emission Using Machine Learning Models

## Project Overview
This project aims to forecast CO2 emissions in the agricultural sector using various machine learning models. The models employed include Linear Regression, Random Forest Regressor, Gradient Boosting Regressor (GBR), and XGBoost Regressor. By leveraging historical data from sources such as IPCC and FAO, this project seeks to provide accurate predictions that can guide decision-making processes in reducing agricultural CO2 emissions. 

## Table of Contents
- Project Overview
- Dataset
- Project Structure
- Methodology
    - Data Collection
    - Data Preprocessing
    - Exploratory Data Analysis (EDA)
    - Machine Learning Models
    - Model Evaluation
- Results
- Tools & Libraries
- Conclusion

## Dataset
The dataset used in this project was constructed by merging and reprocessing multiple datasets from the Food and Agriculture Organization (FAO) and the Intergovernmental Panel on Climate Change (IPCC). It contains various features related to agricultural practices and emissions, and it is used to forecast the CO2 emissions in this sector.

## Methodology
### Data Collection
The data for this project is sourced from the Kaggle dataset:
- **Dataset Link**: [Agri-food CO2 Emission Dataset](https://www.kaggle.com/datasets/alessandrolobello/agri-food-co2-emission-dataset-forecasting-ml/data)

### Data Preprocessing
- **Missing Values**: Rows containing missing values were removed to avoid inaccuracies in predictions.
- **Feature Selection**: ANOVA analysis was applied to select the top 20 most significant features from an initial 30-feature dataset, ensuring a more robust and reliable model.

### Exploratory Data Analysis (EDA)
EDA was performed to understand the trends, patterns, and correlations within the data. Key findings include:
- Agricultural CO2 emissions showed an increasing trend from 1997 to 2020.
- The top sources of emissions were "IPPU" and "Forest Conversion."
- “Forestland” demonstrated a unique characteristic of negative emissions, acting as a carbon sink.

### Machine Learning Models
Four models were selected for their ability to handle regression tasks:
- **Linear Regression**: Baseline model for comparison.
- **Random Forest Regressor**: Non-linear model capable of reducing overfitting.
- **Gradient Boosting Regressor (GBR)**: High accuracy model for complex relationships.
- **XGBoost Regressor**: Efficient model, especially for large datasets.

### Model Evaluation
Each model was evaluated using the following metrics:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-squared (R²) Score

## Results
The Random Forest Regressor outperformed the other models in predicting agricultural CO2 emissions, achieving the following metrics:
- **MAE**: 1,124,603.89
- **MSE**: 1,372,743,313,955.434
- **RMSE**: 3,705,055.081
- **R²**: 0.9997

## Tools & Libraries
The project was implemented using Python and the following libraries:
- **Pandas**: Data manipulation and analysis.
- **Scikit-learn**: Machine learning model implementation.
- **Matplotlib**: Data visualization.
- **Seaborn**: Statistical data visualization.
- **Plotly**: Interactive visualizations.

## Conclusion
This project successfully demonstrated the application of machine learning models in forecasting CO2 emissions in agriculture. Among the models tested, the Random Forest Regressor achieved the highest prediction accuracy, making it a reliable tool for decision-makers aiming to reduce emissions and promote environmental sustainability.

## Code
For the complete code, kindly check out my [Google Colab](https://colab.research.google.com/drive/1IWnFHABIn30Y3KH_yrqx5sdPmu4FQMy-?usp=sharing) site !
