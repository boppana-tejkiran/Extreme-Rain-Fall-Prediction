# Extreme Rainfall Prediction Using Machine Learning

In this project, different Machine Learning models are built to predict extreme rainfall events in the coming 24hrs. & 48hrs. based on current weather data at different climate zones in India. 

### Data Collection
* Weather data (X values for ML models) at surface level and at multpule altitudes at different locations is collected from: https://psl.noaa.gov/data/gridded/data.ncep.reanalysis.surface.html

* Rainfall data (y-values for ML models) at different locations is collected as NetCDF Files  from : http://imdpune.gov.in/Clim_Pred_LRF_New/Grided_Data_Download.html

### Data Pre-processing

Step 3) Run nc.py for all datafiles (change file names as per the years). (for each year individually)

Step 4) Run combine.py on the extracted csv files. (for each year individually)

Step 5) Run data_prep.py on the output files of Step 4 to get gridwise combined file (columns = 22\*225\*2\+3 = 9903)

Step 6) Run nc-rainfall.py on files downloaded in Step 2 (change years, latitude/longitude of region and filenames according to the ones you need) to get the amount of rainfall in that particular region across those years. This is used for next 48 hour prediction.

Step 7) Run data_prep_24.py on files downloaded in Step 2 (change years, latitude/longitude of region and filenames according to the ones you need) to get the amount of rainfall in that particular region across those years. This is used for next 24 hour prediction.


Website (in progress) : https://shruti-codes.github.io/ExtremeRainfall/landingpage.html
