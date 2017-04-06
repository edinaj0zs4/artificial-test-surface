# Artificial test surface for terrace extraction

Semi-automated extraction of fluvial landforms from a coherent digital elevation dataset allows an objective analysis of hydrogeomorphic characteristics. The complementary functionality of GRASS GIS and R provided the possibility to develop a flexible terrain analysing tool for the delineation and quantifiable analysis of terrace remnants.
Methodological issues regarding the terrace extraction approach, also the determination of optimal threshold values were explored by using an artificial hillslope model. The geomorphological applicability was tested on real topography along the terraced valley of the Hungarian section of the Danube.

## Description
- Creating a digital elevation model to represent several methodological issues related to mapping terraced surfaces
- research question is also how to interpret height values of Pécsi M. (1959)
- lower levels are flat, smaller elevation ranges, on histogram there is a clearly visible peak for the most represented height values
- higher terrace levels are more dissected by stream valleys, covered by different sediments, thus a wider elevation range is expected, no clear peak on the histogram but  continuous height values with similar rate representing flat surfaces -> question is also the effect of neotectonics
- terraces of larger tributaries - on the lower levels, younger terraces; the analysis method only removes the valley-bottom (planned, but didn't implement on the model)
- different width of floodplain levels (wide, even missing), embayment
- dissection with higher order streams
- slopes should be similar in steepness between lowest and highest levels, because at upper elevations there is a higher elevation difference, but between lower levels the forms are not eroded, thus not smoothed; lowest levels also small value as the floods can still erode those

https://cloud.githubusercontent.com/assets/25442728/24771510/1d3ffd20-1b0e-11e7-8634-713720b8c5ac.png

### Terrace levels
| Level | Relative elevation |
| ----- | ------------------ |
| Low floodplain | 0-3 m |
| I. terrace | 4-7 m |
| II/a. terrace | 8-11 m |
| II/b. terrace | 18-27 m |
| III. terrace | 40-50 m |
| IV. terrace | 65-80 m |
| V. terrace | 95-115 m |
| VI. terrace | 130-160 m |
| VII. terrace | 170-210 m |
| Top surface | 235-250 m |

### Characteristics of model
- 10x4 km
- 104-350 m elevation
- tilted to represent lowering river elevations from 105 to 100 m
- 7 terrace levels + floodplain levels + flat top surface
- values are representing the Central/Western Gerecse Mountains
- added larger scale noise of few meters to represent erosion-accumulation processes

#### Notes
This is part of my PhD research regarding DEM/DSM based geomorphological mapping with semi-automated landform delineation algorithms.

#### Acknowledgements:
The author would like to express her gratitude for the colleagues of the Department of Physical and Environmental Geography for the professional advices on the project and the support of the Doctoral School of Earth Sciences, University of Pécs. The present scientific contribution is dedicated to the 650th anniversary of the foundation of the University of Pécs.
_The research of Edina Józsa was supported by the Human Capacities Grant Management Office and the Hungarian Ministry of Human Capacities in the framework of the NTP-NFTÖ-16 project._
