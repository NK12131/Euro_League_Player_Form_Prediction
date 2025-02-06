# Player Performance Prediction in Euro League Football

## Team Members
- Resham Deepak Bahira (Reshamm13)
- Sudhanshu Gopalrao Pawar (Psudhanshu)
- Nithin Kumar Hadhge Girish Kumar (NK12131)
- Aaryan wani (aaryanwani)

## Introduction
This project develops a predictive model for forecasting player performance in European football leagues. The model focuses on predicting form scores for upcoming seasons by analyzing historical data and incorporating contextual factors such as match location and weather conditions.

### Key Stakeholders
- Team managers and coaches
- Sports analysts
- Fans and enthusiasts

### Project Benefits
- **For Team Managers and Coaches**: Enables proactive decisions about lineups and training focus
- **For Sports Analysts**: Improves accuracy of long-term analyses and predictions
- **For Fans**: Enhances engagement through data-driven insights

## Data
Dataset Source: [Statbunker Football Statistics](https://data.world/cclayford/statbunker-football-statistics)

### Coverage
- Seasons: 2014/15 to 2022/23
- Leagues:
  - Premier League
  - Bundesliga
  - La Liga
  - French Ligue 1
  - Eredivisie
  - Serie A
  - Scottish Premiership

### Key Features
- Player Performance Metrics
- Contextual Data (match location, weather)
- Team Metrics
- Over 100,000 rows and 117 features

## Methods

### 1. Data Preparation
- Merged 63 CSV files covering multiple seasons
- Standardized key columns
- Implemented systematic cleaning procedures

### 2. Feature Engineering
- Weather Summary Integration
- Position-Specific Form Score Development
- Rolling Feature Creation
  - Rolling Mean (3-match window)
  - Rolling Variance

### 3. Modeling Approaches
#### Machine Learning Models
- Random Forest Regressor
- Linear Regression
- XGBoost Regressor

#### Time Series Models
- SARIMA
- Facebook Prophet

## Results

### Model Performance
#### Random Forest Regressor
- Cross-validation R²: 0.9239 ± 0.0176
- Test R²: 0.8983
- Best performing model for generalization

#### XGBoost Regressor
- Cross-validation R²: 0.9945 ± 0.0065
- Test R²: 0.9834
- Excellent accuracy but potential overfitting

#### Linear Regression
- R²: 0.9999
- Very low MSE (2.8926e-13)
- Indicates potential overfitting

### Weather Impact Analysis
Weather conditions showed minimal impact on form scores, with variations only in the fourth or fifth decimal place.

## Limitations
- Minimal weather impact despite initial hypotheses
- Time series models don't account for major career changes
- Limited ability to predict impact of transfers between leagues

## Future Work
1. Integration of additional contextual features:
   - Player injuries
   - Team formations
   - Player-club synergy
   - Inter-player interactions

2. Development of an interactive dashboard for stakeholders
