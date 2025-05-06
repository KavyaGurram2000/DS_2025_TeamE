# DS_2025_TeamE
Overview :

Accurate housing price estimation is critical for informed decision-making in the real estate sector, which has a substantial influence on the global economy. Traditional valuation methods are often subjective, time-intensive, and susceptible to human error, leading to inefficiencies in pricing. This capstone project seeks to address these limitations by leveraging machine learning (ML) and time series forecasting techniques to predict housing market trends with greater accuracy and objectivity. Using the Zillow ZHVI dataset, which provides historical home values across U.S. counties for various housing categories—such as AllHomes, Single Family, Two-Bedroom, Three-Bedroom, and Condo—we aimed to build predictive models that reflect both temporal trends and economic conditions. Recognizing that the dataset lacks direct indicators of value change, we integrated key economic factors from the Bureau of Economic Analysis (BEA Regional GDP and Personal Income, n.d.), including personal income, population growth, and per capita income.
To capture both short- and medium-term patterns, we calculated annual and five-year changes in home values and developed a suite of predictive models. These included time series methods  as well as regression-based models  trained with past 5 Years of data and tested using 2024 data. The results demonstrated that LASSO ensembled with AR Model is the Best Model for House Price Predictions with the features used. Combining housing and economic data significantly improved forecasting accuracy and reduced reliance on subjective assessments. This project highlights the effectiveness of data-driven approaches in real estate valuation and offers a scalable framework for identifying key drivers of housing price fluctuations across diverse property types.

Requirements.txt

We have requirements.txt as below.
pandas
pandasql
pyodbc
pandera
numpy
scipy
prophet
xgboost
lightgbm
statsmodels
torch
matplotlib
plotly.express
plotly.graph_objects
scikit-learn




Process Execution :

1.Capstone_Exploratory_Analysis_Project.ipynb -> Perform Data Pulls from Zillow , Cleanse and Transforms the Data. Perform EDA on data.
2.Capstone_Final_Merged_File.ipynb -> Build Transformed Merge File with all the Categories data based on EDA results.
2.TimeSeriesModels_DSCI8950.ipynb -> Run Time Series Models i.e. ARIMA, SARIMA , Prophet and LSTM . 
3.MLModel_DSCI8950.ipynb -> Run ML Models i.e. Random Forest, XGBOOST, XGBOOST ensembled with AR, LGBM, Lasso, Lasso ensembled with AR