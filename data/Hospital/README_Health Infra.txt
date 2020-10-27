/* ==========================================================
Authors: Madhulika Khanna, Nishtha Kochhar and Esha Zaveri
File: READ ME file containing description of data with health infrastructure
========================================================== */

Health Infrastructure: These data were available on Government of India’s Open Government Data Platform (https://data.gov.in/catalog/all-india-health-centres-directory?filters%5Bfield_catalog_reference%5D=3786581&format=json&offset=0&limit=6&sort%5Bcreated%5D=desc) and reflect the distribution of health infrastructure on 7th October 2016.

We export these data into ArcGIS where we join these data with shapefiles for district boundaries in 2011 (census year) and 2019 (latest) to obtain the count of number of facilities of each type at the district level.  

2019 district boundaries: We use the shape file with the 2019 district boundaries from Justin Meyers’ GitHub page (https://github.com/justinelliotmeyers/India_Official_Boundaries_2019). We matched the districts listed here with a crowdsourced list of districts updated till 31st December to confirm its accuracy. We build a crosswalk for this exercise where we use publicly available information on district splits and merges between 2011 and 2019. We assume that blocks (subdistricts/taluks) did not split when new districts were formed. We drop Assam since we could exactly match the splits from 2011 to 2019 with district information websites. 


Population data in 2016: To get the facilities per 10000 population, we merge these data with the population data in 2016. We use geocoded population data from Gridded Population of the World, Version 4 (GPWv4) hosted at the Socioeconomic Data and Applications Center (SEDAC) (https://sedac.ciesin.columbia.edu/theme/population). This database contains gridded population data at the sub-district level from the 2011 Census. We estimated aggregate population in 2016 using the population growth rates calculated from the US Census Bureau’s estimates for India (https://www.census.gov/data-tools/demo/idb/informationGateway.php).