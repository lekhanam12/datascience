/* ==========================================================
Authors: Madhulika Khanna, Nishtha Kochhar and Esha Zaveri
File: READ ME file containing description of variables on socio-economic status and comobidities from NFHS data
========================================================== */

The fourth round of the National Family Health Survey (NFHS-IV) was conducted in 2015-2016 across the country and collected detailed information on, among other things, wealth, access to water, sanitation, anthropometry, and biomarker-based data on hypertension, diabetes, and anemia. The NFHS-IV includes the perturbed location of each primary sampling unit, wherein all cases, perturbations are restricted such that the primary sampling unit lies within the original district.

Since men were interviewed in only 15% of the sample, data from men’s interview module are representative at the state level, but not at the district level. Therefore, we present district-level estimates of various risk factors only for women’s sample (ever-married women of age 15-49 years). State-level averages for men and women are significantly and positively correlated.  Categorizing districts using the prevalence of risk factors among women will arguably give the same results. 

Mapping data to 2019 district boundaries: NFHS districts map perfectly to 2011 census districts. We also map these data to the latest district boundaries as in 2019. We build a crosswalk for this exercise where we use publicly available information on district splits and merges between 2011 and 2019. We assume that blocks (subdistricts/taluks) did not split when new districts were formed. We drop Assam since we could exactly match the splits from 2011 to 2019 with district information websites. 
