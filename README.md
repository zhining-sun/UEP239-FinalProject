# UEP239-FinalProject--Suitable Area for Foreign-Born STEM Workers

Hours worked: around 30 hours

*Abstract

This is my final project for UEP239 Geospatial Programming with Python. This project uses suitability analysis to identify areas that are most suitable for foreign-born STEM workers. The number of foreign-born STEM workers is keep increase. There is potential market opportunity targeting those foreign-born STEM workers. As foreigners, these workers tend to have relatively less information comapring to natives. There seem to exist information asymmetry between supplyers and consumers due to different cultural background and language barriers. Use Chinese as an example, there are many renting services targeting Chinese workers. They use Wechat to attract 
consumers and their service usually charge at a higher price. For foreign workers who are new here, they don't know other way to find a good place to stay. Hence, it is pretty important to use suitability analysis to provide information to these foreign STEM workers. This project uses the suitability analysis which takes infrastructure (hospitals, MBTA, schools, and libraries) and environment(landcover and tree canopy) into consideration, to identidy suitable areas for STEM workers. 


*Instruction on how to open this project within the environment


conda env create -f environment.yml

conda activate UEP239

jupyter lab FinalProject_ZhiningSun.ipynb


*Data 

infrastructures: Hospitals, schools, MBTA, libraries

These four data are all vector data that are downloaded from MassGIS. The hospital shape file (HOSPITALS_PT) refers to Massachusetts Acute Care Hospitals. The spatial unit is point. Each point represents a hospital in Massachusetts. The school shape file (SCHOOLS_PT) refers to Massachusetts Schools (Pre-K through High School). The MBTA node shape file (MBTA_NODE) refers to Massachusetts Acute Care Hospitals. The spatial unit is point.


*references:

interactive map: https://vverde.github.io/blob/interactivechoropleth.html

rasterio: https://rasterio.readthedocs.io/en/latest/api/rasterio.features.html






