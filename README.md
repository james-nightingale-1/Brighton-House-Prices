# Brighton-House-Prices
*A data science project predicting property values in Brighton and Hove using linear regression and machine learning models*

---

## Project Overview
This project explores the determinants of residential property prices in Brighton and Hove using publicly available cross-sectional data. It uses a combination of OLS as a traditional linear regression model, and Random Forest and XGBoost as machine learning models, to predict prices.

## Features
- Uses house price data in Brighton and Hove for 2025
- Incorporates distance-, neighbourhood- and property- based regressors
- Data visualisations
- Regression analysis

## How to Run
This notebook is designed to be run in **Google Colab**, but can also be run locally in **Jupyter Notebook**. Make sure to download all files from the data folder to the same directory as the notebook, and that all required Python libraries are installed.

## Data
The project uses these datasets:
- Brighton House Sale Prices for 2025 - HM Land Registry - https://www.gov.uk/government/statistical-data-sets/price-paid-data-downloads
- Energy Performance Certificates for 2025 - UK Government Open Data - https://epc.opendatacommunities.org/login
- Census for 2021, LSOA Deprivation Data - ONS - https://www.ons.gov.uk/filters/7f063526-236e-4102-ab0c-03a5df2fbc19/dimensions
- Crime Statistics by LSOA - Home Office - https://data.police.uk/data/
- School Performance Tables - Department for Education - https://www.compare-school-performance.service.gov.uk/
- Coastline Data - OpenStreetMap, Geofabrik - https://download.geofabrik.de/europe.html
- Google Maps (for creating location-based dictionaries for rail stations and schools)

Note: These datasets were already trimmed down to Brighton and Hove before upload to the repository.

## Insights
Some key findings include:
- The largest drivers of property value are floor area, number of rooms, and whether the property is a flat or a house
- Almost all signs are as expected, except that being near a primary school significantly decreases property value
- EPC ratings have almost no effect on house prices
- Deprivation has a much larger effect on house prices than crime
- Properties being built before 1930 or by the seafront drive prices upwards by a large and significant amount, even though the median seafront property is worth less than the median inland property
- Machine learning models perform better than linear regression models on house price prediction
- XGBoost regressions perform better than Random Forest regressions, due to complex feature relationships and clean datasets.
