/* ==========================================================
Authors: Madhulika Khanna, Nishtha Kochhar and Esha Zaveri
File: READ ME file containing description of data file with average pollution estimates
========================================================== */

Pollution data: We use data on the global surface of concentrations (micrograms per cubic meter) of mineral dust and sea-salt filtered fine particulate matter of 2.5 micrometers or smaller (PM2.5) data for 2016 from Global Annual PM2.5 Grids hosted at the Socioeconomic Data and Applications Center (SEDAC) (https://sedac.ciesin.columbia.edu/data/set/sdei-global-annual-gwr-pm2-5-modis-misr-seawifs-aod).

We export these data into ArcGIS where we join these data with shapefiles containing district boundaries from 2011 (census year) and from 2019 (latest) to obtain the average pollution estimates at the district level.  

2019 district boundaries: We use the shape file with the 2019 district boundaries from Justin Meyers’ GitHub page (https://github.com/justinelliotmeyers/India_Official_Boundaries_2019). We matched the districts listed here with a crowdsourced list of districts updated till 31st December to confirm its accuracy. We build a crosswalk for this exercise where we use publicly available information on district splits and merges between 2011 and 2019. We assume that blocks (subdistricts/taluks) did not split when new districts were formed. We drop Assam since we could exactly match the splits from 2011 to 2019 with district information websites. 

