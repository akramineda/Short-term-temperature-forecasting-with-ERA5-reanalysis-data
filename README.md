# Short-term-temperature-forecasting-with-ERA5-reanalysis-data
With the spirit of reproducible research, this repository contains codes required to produce the results in the manuscript:

> N. Akrami, K. Ziarati, S. Dev, Short-term Temperature Forecastingfrom ERA5 Reanalysis, under review


## Code Organization
All codes are written in python3.

### Dependencies
The following libraries should be installed before the execution of the codes.

- Xarray: `pip install xarray`
- numpy: `pip install numpy`
- pandas: `pip install pandas`
- matplotlib: `pip install matplotlib`
- netCDF4: `pip install netCDF4`
- statsmodels: `pip install statsmodels`
- scikit-image 0.17.2: `pip install scikit-image`


### Data
The data source in this work is [ERA5 Reanalysis Data](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels?tab=form) from ECMWF. We are releasing the processed data that we used in this work. You may find the processed data in [data folder] (data/mean_T_hourly.csv) in repository.

### Scripts
- dl_ERA5_hourly_temperature.py: Run this code to download the hourly temperature data for Fars province from 2015-Jan to 2020-Nov.

- generate_timeseries.ipynb: Run this script to generate time series from the netCDF file as .csv format.

- temperature_forecasting.ipynb: Run this script to obtain the plots used in the paper. Contains time series line plots and plot of forecasting result.

- benchmarking.py: Run this script to obtain the forecasting result for proposed method and benchmarking methods.
