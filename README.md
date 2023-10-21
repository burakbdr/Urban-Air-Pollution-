# Urban-Air-Pollution-
Zindi - PM 2.5 Concentration Level Prediction

PM2.5 refers to atmospheric particulate matter that have a diameter of less than 2.5 micrometers and is one of the most harmful air pollutants.
These particles are a type of air pollution and can be composed of various materials, including dust, soot, smoke, organic chemicals, and metals.

PM2.5 is a common measure of air quality that normally requires ground-based sensors to measure.But ground based sensors are expensive and because of these PM 2.5 level can not be measured everywhere in the world. 

In the project Ground Based-Sensors in train data used as target and model trained with 5P Satellite Data and The Global Forecast System (GFS) data.

The Zindi Channel and Dataset: [Urban Air Pollution Challenge](https://zindi.africa/competitions/urban-air-pollution-challenge).

## Features

- [Weather Data](https://developers.google.com/earth-engine/datasets/catalog/NOAA_GFS0P25).
- [NO2: Offline Nitrogen Dioxide](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_NO2).
- [AER AI: Offline UV Aerosol Index](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_AER_AI).
- [SO2: Offline Sulfur Dioxide](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_SO2).
- [CH4: Offline Methane](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_CH4).
- [O3: Offline Ozone](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_O3).
- [CO: Offline Carbon Monoxide](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_CO).
- [HCHO: Offline Formaldehyde](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_HCHO).
- [CLOUD: Near Real-Time Cloud](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_CLOUD).


## Requirements and Environment

Requirements:
- pyenv with Python: 3.11.3

Environment: 

For installing the virtual environment you can either use the Makefile and run `make setup` or install it manually with the following commands: 

```Bash
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```


