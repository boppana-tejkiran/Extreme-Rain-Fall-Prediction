# Extreme Rainfall Prediction Using Machine Learning

In this project, different Machine Learning models are built to predict extreme rainfall events 24 hr to 48 hr before the occurrence of the event using the previous climatic parameters. at different climate zones in India. 

### Data Collection
* We have obtained the weather parameters (X-values) for the entire Indian subcontinent from NCEP/NCAR reanalysis dataset. The latitude ranges from 5 degrees to 40 degrees north and longitude ranges from 65 degrees to 100 degrees east (Indian region). In particular we have used daily data of weather parameters at surface and multiple altitudes.
https://psl.noaa.gov/data/gridded/data.ncep.reanalysis.surface.html

* Rainfall data (y-values for ML models) at different locations is collected from : http://imdpune.gov.in/Clim_Pred_LRF_New/Grided_Data_Download.html

### Data Pre-processing

* Collected weather data (X-values) & rainfall data (y-values) is in **netCDF** format. So, the data is converted to **csv** format.
* Collected Data is only available yearwise. So, year wise data is combined into a single data file.

Code for preprocessing is presennt in **Data Pre-processing** directory.

### Machine Learning Models

Trained Xgboost, Kernelized Support Vector Classifier models on the data set.

Smote was used to reduce class imbalance and AutoEncoder was used to reduce the dimensionality of data for performance gain.

Discussion about the performance of implemented Machine Learning models is available in **report.pdf**
