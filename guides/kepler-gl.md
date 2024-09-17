# Introductory Guide to Kepler.gl
Created by Alyssa Lopez
<br>*Maintained by [LEADR](http://leadr.msu.edu/) under the direction of Gillian Macdonald*

*Last Updated: 2/11/2019*

This resource was adapted for LEADR classes from ["Teaching Digital Mapping with kepler.gl" by Stephen Robertson.](http://drstephenrobertson.com/blog-post/teaching-digital-mapping-with-kepler-gl/) All options below were tested with Google Chrome.


## Basic Information
Kepler.gl is a platform designed for geospatial data analysis, making it possible to investigate trends on various geographical levels, including region, state, city, and county. A variety maps, such as points, networks, and chloropeths, can be created (or compared) with filters and layering,

For Kepler to be able to make a map from data, there needs to be latitudinal and longitudinal information within your dataset. In some cases, a dataset may have latitude and longitude in one single column, separated by a comma. Kepler **will not** be able to read these values. For more information on the types of files and formats that Kepler accepts, refer to "Add Data on the Map" on the [Kepler user guide.](https://github.com/uber/kepler.gl/blob/master/docs/j-get-started.md)

**Potential Data Sets**
* [Alabama Slave Interviews](http://drstephenrobertson.com/blog-post/teaching-digital-mapping-with-kepler-gl/) used by Dr. Robertson    
* [Alabama County Unemployment data](https://github.com/leadr-msu/leadr-msu.github.io/blob/master/guides/files/kepler-gl/AL-countyunemployment.geojson)


## Getting Started
1. Head to [kepler.gl](kepler.gl) and select "Get Started." Next, you'll need to upload your dataset.
2. Once you do this, you should see a dark map with light points throughout (which represent your location data). If you roll over a point with your mouse, a pop-up will appear with the information from your dataset. You can change this later.
3. If you click on a point, it will remain fixed and a green pin will appear. To unpin it, click that green pin.

**N.B.:** Multiple rows of data with the same latitude & longitude coordinates will not be made separate by Kepler and the points will show up on top of each other with only the top one displaying.


## Base Map
Before moving forward and manipulating and analyzing your map, you can adjust some basic visual settings. To do so, click on the icon that looks like sliders on the upper-left hand side of your screen.
1.  Map Style:
    * There are four options for your larger map color: Dark, Light, Muted Light, and Muted Night.
    * I find that the light options are less accessible than the darker options when some layers are toggled on.
2. Map Layers:
    * There are six options for your basic map layers that can be turned on/off by clicking on the eye icon to the left of them. You also have the option of moving certain layers to the top of the pile, allowing them to appear over things such as points and other layers.
    * Label: When this is on, your map will have various city and state labels on view, depending on the zoom level.
    * Road: When this is on, roads are visible.
    * Border: When this is on, border lines are a visible. In our case, state lines are the dotted lines that appear.
    * Building:
    * Water: When this is on, all waterways on your map are visible
    * Land:


## Layer Settings
Kepler allows you to add multiple layers to your map with the same dataset (or another if you add more datasets). To edit any given layer, click on the icon on the upper-left hand corner that looks like 3 stacked squares.
* You can change the name of a layer by clicking "layers" and typing in a new name.
* To reach all of the other adjustable layer settings, click the small down arrow to the right of "layers."


1. Basic:
    * This is where you can change the layer type. Your options include: point, arc, line, grid, hexbin, polygon, cluster, icon, H3, and heatmap. The automatic choice is "point."
2. Color:
    * You can select a single color for all of your points or you can select “colored based on” and make it a color scale dependent on particular variable.
    * The color based on can be any of the options (columns) of your dataset.
3. Opacity:
    * Changes the color density of your points
4. Radius:
    * This changes the size of your points


**N.B.:** Color and radius can be set to reflect a range of quantitative values. You would not want to use this option, say, for interviewers or interviewees because its categorical and there may be too many options within your dataset.


5. Draw Outline:
    * You can make your points only have outlines, instead of a fill
    * This might not be useful because the clarity of the points is lost depending on the color scheme.
6. Text:
    * You can also have text labels for each of your points and have the ability to change the color and size of this text.
    * I would not suggest doing this because this information can be made visible by scrolling over a point, rather than having possibly distracting/overwhelming text above all your points.


## Interactions Settings
When you click on the icon on the upper-left hand side of your screen that looks like a circle with a cursor over it, you have the ability to adjust how certain interactions on your map look. There are two options within this settings list: Tooltip and Brush.
1. Tooltip:
    * This is where you can change the information that appears when you scroll over a point.
    * What appears in the box under “tooltip” are some of the columns from the .csv that was uploaded to Kepler
    * You can add and delete this information as you see fit. The choices you make for what goes within the pop-up depends largely on your research question(s).
    * If you do not want any information to show when you scroll over a point, you can shut tooltip off with the slider next to the tool.
2. Brush:


## Cluster Map
Cluster maps make it so that points within a set radius are grouped together. To do this, return to the Layers Settings menu.
1. Under "Layer Type," choose "Cluster."
    * Zooming in and out of the map, changes the the size of the clusters.
2. Color:
    * The automatic setting here is to have a color scheme based on point count in each cluster and the color scale itself is based on quantity.
3. Radius:
    * Cluster Size: with this slider, you can change the amount of points in a cluster.
    * Radius Range: changes the size of the circle that represents each cluster.


## Heat Map
To change your map to a heatmap, return to the Layers Settings menu.
1. Under "Layer Type," choose "Heatmap."
2. Color:
    * The color scheme here is not as important as opacity. With the Opacity setting, your “hot” areas become much darker as you move the slide up.
3. Radius:
    * This changes the size of each grouping now on your map.
4. Weight:
    * The automatic setting is “density,” which arguably you want to leave it on, as it shows the “hot” areas where there is an abundance of points.


## Comparisons (Cluster & Heatmap)
It is possible to compare map styles in Kepler through two different methods: Overlapping layers and Dual Map.
1. Overlapping Layers:
    * Change your layer type back to “Cluster.”
    * In the “Layers Setting” menu, select “Add a layer.”
    * Name this second layer “Heat Map” and select that option under “Layer Type.”
    * You’ll see two boxes highlighted red: Lat + Lng. In the respective boxes, select the respective field (Lat = latitude; Lng = longitude).
    * Both of the clusters and heatmap are now overlapping on the same map and allow for some comparisons.
2. Dual Map
    * To do this, you will have to had followed the above steps.
    * You can also view the maps side by side you just made by selecting “Dual Map View” on the top right corner of the window.
    * There is now a “Visible Layers” window that shows on each of your maps (also on the top right corner of the window).
    * In the Cluster map, de-select “heat map”
    * In the Heat map, de-select “interviews”
    * Now, you should see each of the two layers on either side of your screen to compare results.


## Time Map
If you have time values in your dataset, Kepler allows for an interactive map with a timeline. To do this, navigate to the "Filters" menu, which looks like a funnel, on the upper-left hand side of your screen.
1. Once there, select "add filter."
2. Within the box that appears, select the field that starts with "time." A timeline should now appear at the bottom of your screen.
3. The span of time is set automatically by Kepler and the timeline shows the number of points that occur at each moment in time.  
4. Using the white slider at the bottom of the timeline, you can change the span of time that is shown on the map.
    * All dates shown in blue on the timeline are displayed on the map.
    * All dates shown in grey are not displayed on the map.
5. Playback:
   * When the “Play” button is pressed, a line will move across the timeline, showing the amount of information that you have chosen with the slider at a given moment (all of the points will eventually be displayed).
   * You can adjust the playback speed at the top right of the timeline
   * To disable the playback option and have only a set amount of points displayed on the map between a set time period, click on the clock icon under the “Filters” menu.

**N.B.:** Filters apply to all layers from a single dataset.


## Category Map
If your dataset has multiple identifiable categorical options, you can have Kepler visualize your map by these categories. Because filters apply to all layers of a dataset, the same dataset will need to be uploaded multiple times to add different filters to certain categories.
1. Return to the "Layers" menu and select "add data." Upload a second copy of the original dataset that you are using.


**N.B.:** Each dataset is assigned a color. Every layer that uses that dataset is identified by the same color.


2. Rename your first layer to a category (1) and name the second layer the other category (2). These should each be two categorical values that fell within the same column, i.e. house and field as two categories within type of slave.
3. Return to the "Filters" icon and select "Add Filter."
    * Select dataset (1) and chose your larger column value (i.e. type of slave). For value, select what you have just renamed this dataset to (i.e. house).
4. Select "Add Filter," one more time.
    * Select category (2) and chose your larger column value (i.e. type of slave). For value, select what you have just renamed this dataset to (i.e. field).
5. To make these points more clear, you can go back into the "Layer Settings" for each one of the layers and change the size and color of the points.
6. You can also go back into "Interaction" menu and adjust the information that pops up when the mouse rolls over a point so that it better corresponds with any new research question that this new visualization poses.


## Polygon Map
Kepler also allows you to create Choropleth maps, which use color schemes to show values in particular areas. These types of maps are particularly useful for population or demographic studies. Within Kepler, using a .geojson file is very helpful.
1. After your .geojson file is uploaded, be sure to check that "polygon fill" is selected under "Layer Settings."
2. Choose a color scheme and then within "Color based on," choose the value that you want represented on the map.


## Exporting
1. Click on the "share" button to the right of the Kepler.gl logo on the upper-left hand side of the screen. There are three options.
    * Export Image:
        * Select one of the three rations for the size of the image
        * Select a resolution for the Image
        * Before exporting, you also have the option of adding a legend to the map, if need be.
    * Export Data:
        * This exports the datasets (.csv) that you were working with, but also gives you the option to download ONLY the filtered data, which can later be reuploaded.
    * Export Config:
        * With the "Export Current Map File" option selected, a file is created that you can upload to continue working on or edit
        * The file (.json) includes the current layer, filter, map style, and interactions settings.


**N.B.:**
* Only images can be exported from Kepler.gl, which means you cannot embed an interactive map into a site.
* You cannot give a map a title.
* Dual Map View does not export. If you chose to export while this option is selected, you will only get an image of the two overlapping map types.
* The time filer will not be exported with an image of the map.

-----
### Return to [LEADR's Resources list](https://leadr-msu.github.io/)
