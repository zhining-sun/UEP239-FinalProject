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

These four data are all vector data that are downloaded from MassGIS. Their spatial unit are all points. The hospital shape file (HOSPITALS_PT) refers to Massachusetts Acute Care Hospitals. The spatial unit is point. Each point represents a hospital in Massachusetts. The school shape file (SCHOOLS_PT) refers to Massachusetts Schools (Pre-K through High School). The MBTA node shape file (MBTA_NODE) refers to MBTA Rapid Transit Stops. The library shape file (LIBRARIES_PT) refers to Massachusetts Public Libraries. 


ncld folder: landcover, tree canopy

These two are raster data that are downloaded from National Land Cover Database (NLCD) 2016. They are "products for the continuous United States (CONUS) were acquired from the Multi-Resolution Land Characteristics Consortium (MRLC) and processed using gdalwarp. The rasters were reprojected to EPSG:6491 and clipped to the extent of the Boston Region Metropolitan Planning Organization boundaries while retaining the original 30-metre resolution" (copied from proveded-data.html). The format for landcover and tree canopy are GeoTIFF. NLCD_2016_Land_Cover_Boston is from the dataset 2016 Land Cover (the folder name for this data is nlcd). The pixel value refers to NLCD 2016 Land Cover Classes. NLCD_2016_Tree_Canopy_Boston is from
2016 USFS Tree Canopy Cover (the folder name for this data is nlcd). The pixel value refers to Percentage (%) of pixel area covered by tree canopy (0-100).


ZCTA within Boston MPO regions--MPO, ZCTA, MA_Outlines

MPO_Boundaries(Boundaries of Massachusetts Metropolitan Planning Organizations) is downloaded from MASSDOT.It is vector data.The feature is polygons. 

tl_2010_25_zcta510 (2010 Massachusetts 5-Digit Zip Code Tabulation Area (ZCTA) Boundaries) is downloaded from Census Bureau.It is vector data. The feature is polygons. It is in the folder ZCTA. 

OUTLINE25K_POLY (Massachusetts Outline with Detailed Coastline) is downloaded from MassGIS. The feature is polygons. It is in the foler MA_Outlines.


*Packages used

The packages I have used include os, numpy, pandas, matplotlib (pyplot), folium, rasterio, geopandas and richdem. rasterio and richdem are basically used for tranforming to rasters, dong the zonal statistics and visualization. folium is used to do the interactive map. numpy is often used when I have to do the reclassification for the raster feature. pandas and geopandas are used to deal with data frames and geodataframes. os is used to check work dictionary. 


*references:

interactive map: https://vverde.github.io/blob/interactivechoropleth.html

rasterio: https://rasterio.readthedocs.io/en/latest/api/rasterio.features.html


*Ackknowledge

Since I have a couple of raster features, ZCTA ranking for each indicator doesn't seem applicable for me. ZCTA ranking is done only for final scores.





