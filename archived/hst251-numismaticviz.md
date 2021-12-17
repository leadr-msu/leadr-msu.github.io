# Numismatic Data in RAWGraphs & Palladio
Prepared by Brandon Locke
<br>*Maintained by [LEADR](http://leadr.msu.edu/) under the direction of Alice Lynn McMichael*

*Last Updated: 12/17/2017*

## Numismatic Dataset
This is a dataset from MANTIS that includes the Roman, Byzantine, and Islamic coins from between 400 and 500 CE. We've made a few minor changes:
- We've added a `year_avg` column based on the terminus post quem and terminus ante quem
- We've estimated a `Region-coord` lattitude/longitude based on an approxmiate capital or center of the region
- We've removed a few columns that were mostly empty or were not of particular interest for this exercise
[Download the sample dataset directly from here](/files/MANTIS-RomanByzIslamic400-500-cleaned.csv) or
[Download the sample dataset from GitHub here](https://raw.githubusercontent.com/leadr-msu/hst251-NumismaticViz/master/MANTIS-RomanByzIslamic400-500-cleaned.csv) (right-click and save as a csv)

## RAWGraphs
RAWGraphs is an easy interface for experimenting with and creating visualizations. It doesn't do a great job with incorrectly formulated data, and it sometimes breaks in ways that are confusing. It also doesn't give you many great options to add the labels and keys that you want.

To use or export any of the visualizations, you can scroll to the bottom and either copy and paste the SVG Code embed into a website, or use the 'download' option on the left.

----
- Upload the numismatic data file to [RAWGraphs](http://app.rawgraphs.io/)

**What's in this collection? Can we get a bird's eye view of the collection?**

- Scroll down and click on `Treemap`
- Scroll down a little further and drag `Department` into `Hierarchy`
- Scroll down futher and look at the visualization
- We can make the different groups a little more clear by dragging `Department` into `Color`. Scroll down again.
- Scroll back up and drag `Material` into `Hierarchy` (below Department)

*What can we learn from this?*

**Which portraits did given "Authorities" (rulers) put on coins? Conversely, which rulers most often put a given portrait on a coin?**

We can make a visualization that shows both at once!

- Scroll up to the chart display and click on `Alluvial Diagram`
- Scroll down a little further and drag `Authority` and `Portrait` into "Steps"
- Scroll down further to see the visualization.
- Feel free to play with the settings (Node Width, Sort By, Color Scale, etc) to see what works best.

*What can you tell from this visualization?*

**Which portraits appeared with which deities?**

*Make an Alluvial Diagram to evaluate this*

**How did the materials and weights change over time?**

- Scroll up to the chart display and click on `Scatterplot`
- Drag `year_avg` to the `X Axis` and `Weight` to the `Y Axis`
- Drag `Department` into `Color`
- Scroll down and take a look at the chart. You may want to change the `Max Radius`

*What trends do you see? Keep the creation of the "year_avg" field in mind.*

**What were the standard diameters for each department?**

- Scroll up to the chart display and click on `Box Plot`
- Drag `Department` into `Group` and `Diameter` into `Size`

*What can you say about the differences and variability in coin diameter amongst different departments?*

**What were the standard diameters for each *ruler*?**

*How might you do this? You may need to increase the width of your visualization by quite a bit.*

## Palladio
Palladio is a great web app for making simple maps, network graphs, and galleries of images. It doesn't have all of the features that many other tools do, but it's great for quickly asking questions and visualizing a dataset.

At any point, you may click on the 'Download' button in the top right corner to download your entire project - if you want to return to work on it, you can upload it to the Palladio web app and pick up where you left off.

You can save particular visualizations by clicking on the `Export` button.

----

- Go to the [Palladio website](http://hdlab.stanford.edu/palladio/) (you may have to acknowledge that their SSL Certificate isn't completely secure to get there) and click `Start`
- Drag and drop the data file into the window
- The next window will confirm that it's reading all of the datatypes correctly - you can see ULR, Text, Number, and Latlong as the datatypes present
- The three year fields are recognized as numbers and not dates. Click on the name of the field to edit it and change it to date
- Notice at the top there are 5 different tabs - Data, Map, Graph, Table, Gallery - each of these 5 will give you a different glimpse into your dataset

**Where were these coins meant to circulate?**

- Click on `Map` at the top of the screen
- Click `New Layer` on the right. Name this layer "Region." Click on `Places` and `Region-coord` should pop up
- Click on `Size points	` and then scroll down in the box to click `Add Layer`

*What does this tell you about the coin collection?*

**Where were the Roman coins circulated?**
- While you have your Region map up, click on `Facet` in the lower left corner
- On the right, click on Dimensions-`Choose` and then select `Department`
- You can now select and deselect the different departments - select only Roman

*What can we tell from this map?*

**What are the relationships between Region and Diety?**

- Before we go on, click on the x by "Roman" at the bottom to remove our Roman-only facet
- Click on `Graph` at the top to enter the Network Graph interface
- For `Source`, select `Region` and for `Target` select `Diety`

*How useful is this visualization?*

- Click the `Highlight` box under `Region`

*Is this better? What if we put a facet in to remove all of the blank or uncertain coins?*

- Put in two facets (on on `Deity`, one on `Region`) that remove empty fields.
- Click on `Size nodes` to size them according to the number of coins corresponding to each.

*What can we tell from this visualization?*

**How can we visualize these relationships only through the latter half of our datset?**
- Click on `Timespan` at the bottom
- This will bring up a chart that shows the estimated span through which the coins may have been created - make sure the `Start Date` and `End Date` are correct
- Put your cursor in the middle of the graph at around the 450 mark and drag to the right to select everything that overlaps into that timespan (you may need to make sure your browser is in full screen for this to work - your cursor should turn into a crosshairs)
- Click on the down arrow on the right to return to the network graph

*How did that change the visualization?*

**How can we show and sort the images of the coins that we have available to us?**

- Remove the facets at the bottom of the screen
- Click on `Gallery` at the top to enter the Gallery View
- Here we can see a number of fields, including an image box, that we can populate with the dataset
- For the `Image URL`, select either `Thumbnail_obv` or `Thumbnail_rev`
- The rest of the decisons are up to you - what information do you think is best to show here?

## Homework

- Download a dataset from [MANTIS](http://numismatics.org/search/) - it can be whatever department(s) or years you'd like, so long as it fits the scope of the class
- Take a look at the data you've downloaded and come up with a research question
- Use either RAWGraphs or Palladio to make one or more visualizations that answer, or at least start to answer, the research question
- Share the vizualization(s) on the blog, along with a narrative of your process and a reflection on the strenghts and shortcomings of your data and your vizualization. What would you need in terms of information, data, tools, and/or expertise to make this better? Use the category *Numismatic Data as Evidence Activity*.

-----
### Return to [LEADR's Resources list](https://leadr-msu.github.io/)
