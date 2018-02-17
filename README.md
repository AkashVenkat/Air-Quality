# Air-Quality
Predicting temperature using Air Quality Data Points
## Aim
Predicting the temperature using Air Quality information through Linear Regression (Sklearn)
## Source:
Saverio De Vito (saverio.devito '@' enea.it), ENEA - National Agency for New Technologies, Energy and Sustainable Economic Development

## Data Set Information:
The dataset contains 9358 instances of hourly averaged responses from an array of 5 metal oxide chemical sensors embedded in an Air Quality Chemical Multisensor Device. The device was located on the field in a significantly polluted area, at road level,within an Italian city. Data were recorded from March 2004 to February 2005 (one year)representing the longest freely available recordings of on field deployed air quality chemical sensor devices responses. Ground Truth hourly averaged concentrations for CO, Non Metanic Hydrocarbons, Benzene, Total Nitrogen Oxides (NOx) and Nitrogen Dioxide (NO2) and were provided by a co-located reference certified analyzer. Evidences of cross-sensitivities as well as both concept and sensor drifts are present as described in De Vito et al., Sens. And Act. B, Vol. 129,2,2008 (citation required) eventually affecting sensors concentration estimation capabilities. Missing values are tagged with -200 value. 
This dataset can be used exclusively for research purposes. Commercial purposes are fully excluded. 

## Attribute Information:
0 Date (DD/MM/YYYY) 
1 Time (HH.MM.SS) 
2 True hourly averaged concentration CO in mg/m^3 (reference analyzer) 
3 PT08.S1 (tin oxide) hourly averaged sensor response (nominally CO targeted) 
4 True hourly averaged overall Non Metanic HydroCarbons concentration in microg/m^3 (reference analyzer) 
5 True hourly averaged Benzene concentration in microg/m^3 (reference analyzer) 
6 PT08.S2 (titania) hourly averaged sensor response (nominally NMHC targeted) 
7 True hourly averaged NOx concentration in ppb (reference analyzer) 
8 PT08.S3 (tungsten oxide) hourly averaged sensor response (nominally NOx targeted) 
9 True hourly averaged NO2 concentration in microg/m^3 (reference analyzer) 
10 PT08.S4 (tungsten oxide) hourly averaged sensor response (nominally NO2 targeted) 
11 PT08.S5 (indium oxide) hourly averaged sensor response (nominally O3 targeted) 
12 Temperature in Â°C 
13 Relative Humidity (%) 
14 AH Absolute Humidity 

## Libraies Used
1. Pandas - To import the air quality data into Dataframe.
2. Numpy - Used for numeric calculation.
3. Matplotlib - Used for visualization.
4. Sklearn - Used for Linear Regression model.
## Data Cleaning
Removed outliers from prediction variable(temperature), where temperature was -200.0 C.
## Modelling
Removed weakly correlated columns to improve model accuracy, 80% data was trained and 20% was used as test set.
## Accuracy
92.80% accuracy was achieved.
## References
https://archive.ics.uci.edu/ml/datasets/Air+quality
