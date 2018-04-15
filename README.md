# Lab 10: Web Mapping A Choropleth Map

This lab will focus more on building out your lesson JavaScript. We encourage you to explore the new libraries we introduce this week, jQuery and Simple Statistics.

## Mapping Scenario: Patterns of US rental prices (4 pts)

Examine the contents of the *lab-10/data/* directory. This directory includes a starter template *index.html* file and a *counties_median_rent_2015.json* data file produced by joining data downloaded from [American FactFinder](https://factfinder.census.gov) with US county polygons downloaded from the [US Census Cartographic Boundary Shapefiles](https://www.census.gov/geo/maps-data/data/cbf/cbf_counties.html).

You'll notice that each county has two attribute properties: a "NAME" and a "RENT", the latter of which is the median gross rent within the county. Also, **warning**: some polygons have null values for the RENT attribute.

Use this file to build a choropleth web map of US rental prices per county. It should look like this and include a tooltip or popup that displays the name of the county, the attribute being mapped (i.e., "median rent"), and the value of that attribute for that county.

![Lab 10 solution](graphics/lab-10-solution.gif)
**Figure 01.** Lab 10 Solution:

Use the lesson for guidance and edit the *lab-10/index.html* to fulfill the requirements listed here.

### Specific map requirements

* Map should draw *counties_median_rent_2015.json* with 5 to 7 classes showing median gross rent values as color gradient.
* Map should have a clear legend that shows the color and values (in correct units) of your class.
* When the user mouses over count, a tooltip or popup will provide the name of the county and average rent value.
* Page should have updated title and metadata information.
* Code should be well-structured with indentions, comments, and meaningful variable and function names

**Challenges:**

* Add a state outline layer to help readers determine state boundaries (hint: see the [jQuery .when() method](https://api.jquery.com/jquery.when/) for loading multiple files.
* Use jQuery to show a list ranking counties by their median gross rent values sorted from highest to lowest values.

Commit your work as you go, push to your repository, and submit the link within Canvas by the due date.
