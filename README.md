# NBA Player Performance Prediction Using Machine Learning  

## Project Overview  
This project applies machine learning techniques to predict NBA player performance metrics for the 2023-24 season. The dataset, sourced from Kaggle, includes 518 players and 68 statistical attributes. The primary goal is to forecast key performance indicators (KPIs) such as points scored, assists, rebounds, and field goal efficiency. Various machine learning models, including **XGBoost, Random Forest, Support Vector Machines (SVM), and Neural Networks**, are used for both regression and classification tasks.  

By implementing **rigorous data preprocessing, feature engineering, exploratory data analysis (EDA), and ensemble learning techniques**, the project demonstrates how AI can be effectively applied in sports analytics to enhance decision-making, optimize player performance, and improve game strategies.  

## Features  
- **Comprehensive Data Preprocessing:** Handling missing values, outlier detection using the **Interquartile Range (IQR)** method, and feature engineering (e.g., **Player Efficiency Rating (PER)**).  
- **Exploratory Data Analysis (EDA):** Insights through **heatmaps, radar charts, scatter plots, histograms, and correlation matrices**.  
- **Machine Learning Models:** Implementation of multiple **regression and classification models** for accurate predictions.  
- **Feature Selection:** Use of **SelectKBest** to identify the most relevant attributes for improved model performance.  
- **High Model Accuracy:** XGBoost achieved **99.38% accuracy** in player conference classification.  
- **Ensemble Learning Techniques:** Combining **Random Forest and XGBoost** to improve classification performance, achieving **99.17% accuracy**.  

## Dataset Information  
- **Source:** Kaggle (NBA 2023-24 Player Stats)  
- **Records:** 518 players  
- **Features:** 68 attributes (categorical and numerical)  
- **Key Attributes:**  
  - **Categorical Data:** PLAYER_NAME, TEAM_NAME, Conference  
  - **Numerical Data:** Points (PTS), Assists (AST), Rebounds (REB), Field Goals Made (FGM), Field Goals Attempted (FGA), Free Throws, Minutes Played (MIN)  

## Installation  
```bash  
git clone <repository-url>  
cd nba-performance-prediction  
pip install -r requirements.txt  
```  

## Usage  
```bash  
python preprocess.py   # Perform data preprocessing  
python eda.py          # Conduct exploratory data analysis  
python train.py        # Train the machine learning models  
python evaluate.py     # Evaluate model performance  
```  

## Machine Learning Models Implemented  

### Regression Models  
- **Linear Regression:** Predicts points scored using a basic linear model.  
- **Polynomial Regression:** Extends linear regression by capturing non-linear relationships.  
- **Multiple Linear Regression:** Predicts player performance using multiple statistical inputs.  
- **XGBoost Regression:** A powerful gradient boosting algorithm for higher accuracy in predicting continuous values.  

### Classification Models  
- **Random Forest Classifier:** Uses multiple decision trees to improve classification accuracy.  
- **K-Nearest Neighbors (KNN):** Classifies players based on statistical similarities.  
- **Logistic Regression:** Predicts binary outcomes such as whether a player will score above a given threshold.  
- **XGBoost Classifier:** Achieved **99.38% accuracy** in predicting player conference (East/West).  
- **Neural Networks (MLP):** Categorizes players into performance levels based on complex feature relationships.  
- **Naive Bayes Classifier:** Probabilistic model that works well with categorical data.  
- **Support Vector Machine (SVM):** Identifies the optimal hyperplane for classifying players.  
- **Decision Tree Classifier:** A rule-based model that splits player data based on feature values.  

### Ensemble Learning  
- **Random Forest + XGBoost:** A combined model that achieved **99.17% classification accuracy**.  

## Results and Analysis  
- **XGBoost Classification Accuracy:** **99.38%** for predicting player conference (East/West).  
- **XGBoost Regression R-squared Score:** High variance explanation in player performance predictions.  
- **Feature Selection Impact:** Using **SelectKBest**, we identified the most significant features, including **Minutes Played (MIN), Field Goals Made (FGM), Assists (AST), and Rebounds (REB)**, leading to improved model efficiency.  

## Exploratory Data Analysis (EDA)  
EDA was performed using **data visualizations and statistical analysis** to understand player performance trends. Key insights include:  
- **Correlation Matrix:** Showed strong relationships between **assists and points scored**, as well as between **rebounds and minutes played**.  
- **Scatter Plots:** Demonstrated the relationship between **Field Goals Attempted (FGA) and Field Goals Made (FGM)**.  
- **Radar Charts:** Used to compare multiple performance metrics for top-performing players.  
- **Histograms & Count Plots:** Helped in analyzing score distributions and team trends.  

## Future Scope  
- **Real-Time Data Integration:** Enhance the model by incorporating **live game data and player tracking statistics**.  
- **Advanced Neural Networks:** Experiment with **Recurrent Neural Networks (RNNs) and Convolutional Neural Networks (CNNs)** for more accurate predictions.  
- **Injury Prediction Models:** Develop machine learning models to **predict injury risks** based on workload and historical health data.  
- **Game Strategy Simulation:** Use AI to **simulate the impact of different strategies** based on historical data.  
- **IoT Device Integration:** Utilize wearable technology to track player vitals and improve predictive accuracy.  
- **Multi-Season Analysis:** Extend the dataset to cover **multiple seasons** for better generalization and long-term performance forecasting.  

## Contributors  
- **Shefali Khera**   


