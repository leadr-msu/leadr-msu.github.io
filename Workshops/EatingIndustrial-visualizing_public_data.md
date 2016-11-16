#Visualizing Public Data

##In Class
###Finding and Evaluating Data
There are datasets available all over the web, especially from governmental departments, non-profits, and similar organizations. Since we're interested in food, the US Department of Agriculture (USDA) is a good place to start. They have a [Food Availability (Per Capita) Data System](http://www.ers.usda.gov/data-products/food-availability-per-capita-data-system/), with some data that will help us look at the changing American diet.

1. Go to the [USDA Food Availability (Per Capita) Data System](http://www.ers.usda.gov/data-products/food-availability-per-capita-data-system/) website.
2. Scroll down to **Loss-Adjusted Food Availability** section - this is near the bottom of the page.
3. Select your assigned food category to download an Excel file of the data.
4. Open the file and take a minute or two to browse and get a sense of what's included.

Each Excel file should have a *TableOfContents* sheet with links to sheets that have a specific type or subgroup of food in detail.

* **What questions can you ask of this data?**
* **How might you visualize this information to discover or illustrate trends?**

###Preparing the data for Tableau
1. After looking at the dataset, select at least 7 sheets that you think would be interesting to examine.
1. Create a new Excel workbook, add in the column headers 'year', 'lbs per year', and 'product' in A1 through C1. 
1. Select a sheet you want to examine and copy the years (Column A) and the Lbs/year per capital availability adjusted for loss (Column J). Skip the top rows with headers, and just copy the data. **Tip:** *Click and drag for the first column, and then hold ctrl (on a PC) or command (on a Mac) and click and drag for the second. This will select both columns for you to copy.*
1. Paste these into your new workbook below the headers. They should fill column A (year) and B (lbs per year). Type the name of the product in the third column and drag down through the end of the data.
2. If your data has any *n/a* fields, make sure you delete them and leave the field empty. If there are letters, Tableau will read the data as *dimensions* and not *measures*.
1. Select the data from the next food category and paste it all directly below the data in your new workbook. Continue until you've pasted all of the sheets you're interested in.

###Importing and visualizing with Tableau
1. Open Tableau and click 'Excel' on the left to connect to an Excel file. Select the new file you've created, and wait a minute for it to load.
1. Once it has loaded, it should appear in the bottom half of the screen. Make sure everything looks correct.
1. On the bottom of the screen, there will be an orange box that says "Sheet 1." Click on that to open up a worksheet that will allow you to make some visualizations.
1. On the left, you'll see the types of data you have available from your dataset. To look at loss-adjusted food over time, do the following: Drag 'Year' into the *Columns* space at the top, 'Product' to *Rows*, and 'Lbs Per Year' to *Rows*.
1. This will chart each type of food individually. To put them on the same graph, click on a chart option on the right in the *Show Me* section. You'll only be able to select chart types that work with the number and types of data you have selected. 'Lines (continuous)' and 'area charts (continuous)' are probably your best bets.
1. Once you've selected a chart you like, you can click 'Show Me' in the top right to hide the types of charts. This will also show you the chart legend.
1. To add a label to each line, you can click on 'Product' on the far left and drag it into the 'Label' box just to the left of the chart.
1. Finally, give the chart a title. Double click on the title at the top (it's probably 'Sheet 1'). This will open a new window - clear everything in the box and type in your title.

###Analyzing and Sharing
Take a moment and chat with your partner:
What are you able to see from your chart? Did it look about the way you expected? Were there any surprises?

What do the changes you see tell you about industrialized food? 

To publish your chart:

1. Go to *File > Save to Tableau Public As...* and save the file under the name you'd like. This may require you to sign in with your Tableau Public account.
1. This will open a web browser window to your chart on the Tableau website. At the bottom, you'll see a *Share* button that will give you shareable links and a code to embed the chart into your own blog post.







