# HeatMap and ClusterMap of Dengue cases at State of São Paulo - 2023.

## About

This is a case study about the dengue situation at State Of São Paulo. The objective is to understand the metrics and provide solutions to combat the spread of dengue cases.

## In this project, you can do:

Visualize the distribution of dengue cases in the State of Sao Paulo. The project was divided into two parts: a heat map and a clustering map.


## Technologies
- Python
- Pandas
- GeoPy
- Folium 


## On Prod:
The first part of the project was to perform data ETL (Extract, Transform, Load).
The data was acquired from the website of the State Health Department using Python and Pandas.

A table containing municipalities and their corresponding dengue cases was obtained. With the help of the GeoPy library, latitude and longitude coordinates were then assigned to each municipality.

The next step involved refactoring some incorrect data and removing outliers based on their location.

For the heat map, the logic involved duplicating each coordinate based on the number of dengue cases, as the number of incidences is the key factor considered in a heat map.

Only the region of Caçapava was taken into consideration

The visual representation of the heat map can be seen below:

![HeatMap1](https://github.com/Guilherme-Turri/maps-of-dengue-cases-sp/blob/master/imgs/heat1.png)
![HeatMap2](https://github.com/Guilherme-Turri/maps-of-dengue-cases-sp/blob/master/imgs/heat2.png)
![HeatMap3](https://github.com/Guilherme-Turri/maps-of-dengue-cases-sp/blob/master/imgs/heat3.png)

For the clustering map, the location of each municipality is taken into account, which is why there is no need to use the number of cases for the labeling logic.
The algorithm used for clustering calculates the distance between municipalities and groups them into clusters based on their proximity to each other. This allows similar municipalities to be grouped together, forming clusters on the map based on their geographical locations.

The visual representation of the cluster map can be seen below:
![ClusterMap1](https://github.com/Guilherme-Turri/maps-of-dengue-cases-sp/blob/master/imgs/cluster1.png)

![ClusterMap2](https://github.com/Guilherme-Turri/maps-of-dengue-cases-sp/blob/master/imgs/cluster2.png)

![ClusterMap3](https://github.com/Guilherme-Turri/maps-of-dengue-cases-sp/blob/master/imgs/cluster3.png)

## Build:
*Deployed at Vercel*

You can see the heat map running here: 

[Heat-Map-Dengue-App](https://heat-map-dengue.vercel.app/)

You can see the cluster map running here: 

[Clustering-Map-Dengue-App](https://cluster-map-dengue.vercel.app/)



