# Overview
This repository consists of data and code for estimating inhaled NO2 from the biometrics of a participant. 

Description of each of the subdirectory, files and how to make use of it is below:
#### src
The file consists of the codes and data that constructs the DataFrame to be used in estimating inhaled NO2. Since the EEG and Tobii data is too large and moreover is same as the one used previously, the data can be obtained from Zenodo: https://zenodo.org/records/10184801 and description of which is in Github repository: https://github.com/mi3nts/Estimate-CO2. The "full_psds_for_2021.pkl" data created from the " EEG frequency 2021.ipynb" is used in "Bike Ride 2021.ipynb".
The NO2 data for the 3 days in stored in the 3 files named after the days of data collection: 2021_05_26, 2021_06_09 and 2021_06_10 -> data -> trunkSensors ->..."*.csv" file. The "Bike Ride 2021.ipynb" combines the biometric and the NO2 data and creates a DataFrame "full_df_2021_NOX.pkl" which is used in estimating the inhalaed NO2 in 3 ways. 

#### other files
The "full_df_2021_NOX.pkl" file consists of the DataFrame with 330 columns of which 329 are the biometric variables and 1 column is the target variable: NO2. This DataFrame is imported in the "NO2 complete.ipynb", " NO2 Non-EEG.ipynb" and " NO2 with 6 features.ipynb " Jupyter notebooks which after data cleaning estimates the inhaled NO2 using 329 features, 9 features and 6 features respectively.

#### Citation

If the code and data was found to be useful, then please use the following citation:
`Ruwali S, Fernando B, Talebi S, Lary DJ. Estimating Inhaled Nitrogen Dioxide from the Human Biometric Response.
https://github.com/mi3nts/Estimate-inhaled-NO2`

Bibtex:
```
@misc{estimateNO2,
author={Ruwali,S. and Talebi, S. and Fernando, B.A.  and Lary, D. J.},
title={Estimating Inhaled Nitrogen Dioxide from the Human Biometric Response},
howpublished={https://github.com/mi3nts/Estimate-inhaled-NO2},
year={2023},
}
```
The entire dataset and description is also available in Zenodo: https://zenodo.org/records/10345982
