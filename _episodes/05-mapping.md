---
title: "Mapping"
teaching: 10
exercises: 20
questions:
- "How do I plot the results of spatial queries on a map?"
objectives:
- "Learn about the various options for visualizing geospatial datasets."
keypoints:
- "GIS software provides a graphical user interface for running geospatial queries and making maps of the results"
- "QGIS is a particularly good software for interfacing with PostGIS"
---

#### Plotting your data on a map:

1. Download the [QGIS](http://qgis.org/en/site/) software
2. Run the software and connect to the database:
   * click on **"layer/add PostGIS layers"**
   * click on the **"new"** button and enter the connection information (similar to what you did in exercise 1 for the pgadmin software)
   * click on the **"connect"** button
   * you should now see the database tables we've been working with. Add one of these and it should appear on the map.
3. Things to explore next:
   * change the symbology of the points, coloring them by a specific attribute so that the colors illustrate grouping in the data
   * add a background map `web\QuickMapServices\OSM`
   * issue the SQL query you built above to select only those points within 1 km of a point
     * click on `database\DBmanager` and you will see the database to which you have already connected.
     * issue a SQL query in the SQL command window (blue arrow in this screen capture):
    <img src = "../assets/img/databaseIntro/dbmanager.png" width="600">

> ## Challenge: Try to make a map like this!
> <img src="../assets/img/databaseIntro/crimeradius.png" width="300">
{: .challenge}

## Additional resources

* [Geopandas](http://geopandas.org/) is a Python library that can be used to manipulate and plot vector geospatial data
* Visit our [geohackweek tutorial](https://geohackweek.github.io/vector/) on Geopandas for more information and examples.
 
