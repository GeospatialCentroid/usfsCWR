
## Crop Wild Relative on US Forest Service lands

*Update 2025-05-02*

Major updated based on February meeting. 



1. Utilize the USFS datasets to organize information 
  - layer 1 : Regional areas (9 unique areas)
  - layer 2 : Admin layer (112 unique areas)
  - level 3 : National Forests and Grasslands (260 unique areas)
  - level 4 : Research Areas  (16 unique areas)
  - level 5 : Wilderness Areas (451 unique areas)
  - level 6 : Botanical Areas (46 unique areas)

2. Summarize the total number of species predicted and observed at these areas 
  - predicted : at least a single cell of a habitat suitability model in within the area boundary for a species 
  - observed : at least a single point observation for a specific is found within the area boundary 
  
<div style="display: flex;">
  <div style="flex: 1; padding-right: 10px;">

  <h2>Maps</h2> 
  
  Three maps are generated to so the total predicted and observed species per area
   
   - total taxa ( combined predicted and observed)
   - total taxa observed
   - total taxa predicted  
  
  [Total taxa predicted and observed](https://geospatialcentroid.github.io/usfsCWR/combinedMap.html)
  
  This map looks at the unique taxa between the prediction and observed datasets and provides a full list. This will be the highest number of species of any map. 
  
  [Total taxa observed](https://geospatialcentroid.github.io/usfsCWR/pointMap.html)
  
  This map highlights the number of unique taxa observed within each geography. Every observation indicates a reported ground observation of the species.
  
  
  [Total taxa predicted](https://geospatialcentroid.github.io/usfsCWR/rasterMap.html)
  
  This map highlights the number of unique taxa predicted within each geography. Only a single cell of the potential distribution needs to be in area. 

  </div>
  <div style="flex: 1; padding-left: 10px;">

  <h2>Data summaries </h2>

  Two files were create to summarize the presence of theses species in the specific management areas 
  
  The left move column is the taxon of interest. 
  The column to the right contain the names or unique identifiers of specific forest service areas. 
  
  [Observed taxa](https://docs.google.com/spreadsheets/d/1zBxiKcVKg9rcC-qGf93kP-hOCJYTihS8j2Y6D9ut4y8/edit?usp=sharing)
  
  
  [Predicted taxa](https://docs.google.com/spreadsheets/d/1XX9I4V3rD5AcotK4yHF9-K7VhA2mCZIXUzVBpm97Hk4/edit?usp=sharing) 
  

  </div>
</div>
  
  





<!---


## older material 


*Updated* : 2025-02-7

Significant overhall to the workflow with the specific aims of 

1. Utilize the USFS datasets to organize information 
  - layer 1 : Admin layer (112 unique areas)
  - level 2 : PADUS Fee Areas  (276)
  - level 3a : Wilderness Areas (451)
  - level 3b : Botnaical Areas (46)

2. Summarize the total number of species predicted and observed at these areas 
  - predicted : at least a single cell of a habitat suitability model in within the area boundary for a species 
  - observed : at least a single point observation for a specific is found within the area boundary 
  
  
## Maps 

There are quite a few way to showcase these relationship currently were showing four. 
 
 - total taxa (predicted and observed)
 - total taxa observed
 - total taxa predicted 
 - density of observed taxa 

### [Total taxa predicted and observed](https://geospatialcentroid.github.io/usfsCWR/uniqueTaxa.html)

This map looks at the unique taxa between the prediction and observed datas and provides a full list. This will be the highest number of species of any map. 
All four layers are present and the an additional point layer datasets is added for botanical areas for ease of reference. 

### [Total taxa observed](https://geospatialcentroid.github.io/usfsCWR/totalObservered.html)

This map highlights the number of unique taxa observed within each geography. 

### [Total taxa predicted](https://geospatialcentroid.github.io/usfsCWR/totalPredicted.html)

This map highlights the number of unique taxa predicted within each geography. 

### [Total observation per cell](https://geospatialcentroid.github.io/usfsCWR/totalObsPerCell.html)

This map highlights showcase the density of sampling within a region. The values on the map represent the number of occurrences, which is different then previous maps that show the number of species. 
This is a more ganular way to look the distribution of collecting with in the region. Only the admin layer is present on the map as this layer encompasses the spatial extent of all other features.










## Material for 2024 CWR conference 

This work aims to develop a national inventory of crop wild relatives and wild utilized species on USFS lands based on previously published data.

This activity area will apply the occurrence information and species distribution models developed for approximately 600 taxa native crop wild relatives and wild utilized species, which were published in Khoury and Carver et al. (2020), to USFS lands, to develop inventories for USFS lands based on existing knowledge. 

### General Method 

PAD-US dataset was used as a spatial reference for all USFS lands. These were selected based on the `Mang_Name` == "USFS". All records sharing the same `Unit_Nm` were aggregated into a single spatial feature. This was done to reduce the overall processing time, as spatail relationships were test per each USFS area. 


### Evaluation of Occurrence Datasets

**Method Brief** : Occurrence data was transformed to match the CRS of the PAD-US dataset. For each unique USFS area, an intersect with the occurrence data was performed. The result provided all observations present within the designated area. Once define the unique number of species, total observations, and observations per area was calculate for each management area.  

**Reference datasets**
- [original observation data](https://drive.google.com/file/d/1PrcgwY7kHP22kei-iSZHj6duTltg7ald/view?usp=sharing)
- [spatial join observation data and between USFS lands](https://drive.google.com/file/d/1rlXn9ADJIeEbIk0JBv5PlrpmGkVNJ0WC/view?usp=sharing) (Wilderness and National Forest only)


#### [Map of all Occurrences in US Service Lands](https://geospatialcentroid.github.io/usfsCWR/fsPointWildernessNF.html)


### Evaluation of Species Distribution Models 
**Method Brief** : Distributions models were transformed to match the CRS of the PAD-US dataset. For each species distribution, the USFS sites that intersected with the area of extent of the distribution model were selected. With this subset of locations, a count of the number of pixels within each protected area was generated. Once completed for all species, the total number of uniqu species, and the average area that each species was found within the protected area was recorded.  

**Reference datasets**
- [spatial join between distribution models and USFS lands](https://drive.google.com/file/d/12In8I6C8KqNIf91W8LHnGws12pIiS28k/view?usp=sharing) (Wilderness and National Forest only)

#### [Map of all predicted habitat in US Service Lands](https://geospatialcentroid.github.io/usfsCWR/fsrasterWildernessNF)

---> 

