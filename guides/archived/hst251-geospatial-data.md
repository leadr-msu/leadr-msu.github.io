# Visualizing Geospatial Data with CARTO
Created by [Autumn Painter](http://autumnpainter.com/)
<br>*Maintained by [LEADR](http://leadr.msu.edu/) under the direction of Alice Lynn McMichael*

*Last Updated: 3/30/2018*

Learn to manipulate spatial data, join and filter datasets, work through challenges of historical data, and style a map in CARTO.

[Sign up for a trial CARTO account](https://carto.com/signup/)—most of the info they ask for is optional.

## Data

This data was selected from MANTIS—it includes coins between 500 and 800 CE from the Islamic, Byzantine, and Roman Departments. The following data was removed:

- Coins with no mint information
- Geocoordinates for the mints were added from the MANTIS repository and some simple research
- Coins for which geocoordinates for the mint couldn't be retrieved from MANTIS or easily found

[Download the data here](https://drive.google.com/file/d/1WXhfzg-kYU52pJoT1-h851X61qfQaY8T/view?usp=sharing)

## CARTO
[CARTO](https://carto.com/) is a an open source software that employs widely-used languages and technologies (GeoJSON, PostgreSQL, PostGIS) to easily customize maps, generate spatial data visualizations, and share and publish visualizations. Although this can be hosted on a local server, we'll be using CARTO's free (but size-limited) cloud service.

Because this is a free account, your data and maps will be public. For more information, you can [*see their guide to privacy settings*](https://carto.com/learn/guides/publish-share/privacy-settings-for-protecting-maps-and-data).

## Activity

1.  Open coinmints500-800.csv and examine the dataset. What is being represented here? How is it structured? How could it be mapped?

2.  Log in to CARTO. Click on the blue button in the top right that says 'New Map.'

3.  Click on the 'Connect dataset' tab, and then select the 'Data file' box. Click 'Select a File' at the bottom of the page and upload the CSV. Hit 'Connect Dataset.' This will take a moment to load.

4. You'll see a 'coinmints500_800' layer on the left, and you'll see dots on the map. [FYI - if there were any problems mapping items, there would be a notice here to let you know that not everything is on there.]

5.  The window on the left shows the different layers on the map. Right now there should be two: the coinmints500_800 dataset and the basemap.

6.  Click on coinmints500_800 - this will show you a summary of the dataset, and will have some tabs that the top that will allow you to do a number of different things with the data layer. Click on ‘Style’ if it's not already selected. You’ll see that the default setting is ‘Aggregation - None,’ which gives us a simple small red dot on every location in the dataset.

7.  There are several different aggregation styles here, each with its own options. Take a moment and click through each of these. Many of them will need tweaking to make an effective map, but it will give you an idea of what each will do.

    -   None - a simple dot on each datapoint

    -   Squares - creates a grid of equally sized squares that cover the map and counts the datapoints within each

    -   Hexbins - creates a grid of equally sized hexagons that cover the map and counts the datapoints within each

    -   Adm. Regions - uses country, state, county, etc regions and determines data points within them (can automatically find some, or you can upload your own shapefiles for adminstrative regions)

    -   Animated - data animation of a progression of points that is based on time-series data.

    -   Pixel - creates a heatmap of the data points

**Animated Point Map**

1.  Select Animated from the Aggregation menu. It will start an animation that doesn’t seem to have much of a pattern or meaning. By default, the animation uses the cartodb_id — on the left side, change ‘Column’ to ‘year_avg’.

2.  There are a number of tweaks you can make here to make it more effective and aesthetically pleasing. Here are a few:
	- **Size/Color**: The number next to fill adjusts the size of the dot. I like 4 for this map.
	- **Steps**: The data points are all put into small groups that will all appear at once. Adjusting the steps can create a smoother animation and, in conjunction with duration, can set the pace of the animation to your needs. Since there are 300 years, 300 seems like a good number of steps
    - **Duration**: This controls how fast or slow the animation moves. I like around 60 to watch dots roll out more slowly.

3.  We’re done! In the top left, it should say ‘Untitled Map.’ Click on the blue dots after the title, click ‘Rename’, change it to ‘Coins Animated,’ save it and click on the circle just to the left of the map name next to it.
*Note: One frustrating thing about CARTO’s Animated map is that you can’t export an animated gif version. You have to either embed the map from CARTO or do something like a screen record.*

**Animated Point Map by Material and/or Department**
1.  Select Animated from the Aggregation menu. Remember to change ‘Column’ to ‘year_avg’.
2. Near the top of the left side, click on 'Data'
3. Scroll down to 'Material' and click on the check mark to add it as a widget.
4. On the left, you'll see the different types of material represented in the collection. Select 'Bronze' to only show the bronze coins - the animation may take a second to get caught up.
5. Back on the left side of the screen, scroll up to find 'Department' and add that as a widget. You'll see that there are 510 bronze Byzantine coins and 160 bronze Roman coins. Select 'Byzantine' to just show the bronze Byzantine coins.

**Simple Map with a material color-coding and embedded photos**
*Note: this type of map may not be ideal for a dataset like this, where lots of rows have the exact same location*

1.  From the dashboard, click ‘New Map,’ click on the dataset you uploaded earlier and then ‘Create Map’ in the lower right. You’ll again have the simple map loaded.

2.  Once again, click on on ‘coinmints500_800’ section on the left to edit the layer. Click on the ‘Fill’ color bar, and then click on ‘By Value' at the top of the pop-up window. Select ‘material’ and then see that the data points are all colored according to their material.

3.  Go back to the sidebar on the left and select ‘Pop-Up’ This will give you a few different styles for the pop up you’d like. Since we have image URLs for most coins, lets select the ‘image’ style, which is all the way to the right.

4.  Check the boxes for whatever metadata you’d like to appear in a popup window. I’ll select `mint`, `material`, `year`, `department`, and `thumbnail_obv`. In order for the image to appear correctly, you’ll need to drag the `thumbnail_obv` to the top of the list, and put whatever text overlay you’d like second from the top.

5.  Note that you can select different information to appear on a hover over the point. I’ll leave that at ‘none.’

6.  Click back in the top left corner, and rename your map ‘Coin Embedded Photos’ and click on the circle to return to the dashboard.

**Cleaning Up and Publishing**

Now that we’ve created a few maps, we can take one of them, style it the way we’d like, and publish it on the web. I’ll be styling the Coin Embedded Photos map.

*Change basemap*

On the left, there should be a box that says “Voyager - Basemap.” Click in the box to view your basemap options [You can also upload your own or access maps from other servers. [*Kristen Mapes has a great tutorial on georeferencing a map and integrating it in CARTO*](http://www.kristenmapes.com/georectifiedmap2/).]

*Add legend to map*

Return to your data layer (click back, and then click on coinmints500-800). Click on the ‘Legend’ link on the top of the editor window. There will be at least one template option (this depends on the type of map), for this embedded photo map, it should pull the color-coded categories in automatically, or there’s an option to make a custom legend from scratch. The legend will automatically pull in the name of the data layer, and there doesn’t appear to be a way to change this without changing the name of the layer. I’ll click on the three dots at the top of the left panel and click rename, then call it “Coins by Material.” [Note: This doesn’t change the name of the underlying *dataset*, just the layer in this map.]

*Set map options*

You can set the different types of interactions and tools that appear on your public map using ‘Map Options.’ The Map Options button looks like two adjustment sliders and it’s located on the far left side of the screen on the blue bar. There you can toggle the Search Box, Zoom Controls, Legends, Layer Selector (so the user can turn different layers on and off), the Toolbar, and allow/disallow users to zoom using a scroll wheel.

*Publish*

In the top left, there should be a green button that says ‘Public’ and a note that says it is not yet published. Click on ‘Public’ and then click on the blue button that says ‘Publish.’ There should then be links on the page to a publicly accessible maps and an iframe link for embedding. Any further changes you make on the map will not automatically be reflected on the published versions — you will need to return to this page and click ‘Update.’ *Note: The default map window (zoom level and positioning of the map that loads for users) will be set to your current window when you hit ‘Publish’ or ‘Update,’ so be sure you’re setting it correctly before you publish.*

## Experiment
Make a few of your own maps based on questions you may have.

We'll discuss our results at the end of class.

[Roman Empire datasets](https://github.com/klokantech/roman-empire/tree/master/data)

*Note: At some point you may hit your CARTO limit and have to delete a map or two to be able to create more.*

-----
### Return to [LEADR's Resources list](https://leadr-msu.github.io/)
