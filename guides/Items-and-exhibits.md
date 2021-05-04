# Items and Exhibits in Omeka

Created by [Zach Francis](https://redfeather.dev/)

*Last Updated: 2/26/2020*

## Overview
This handout will guide you through the basics of creating Items and Exhibits in Omeka. Omeka Items are composed of digital resources and their associated metadata. Exhibits embed these Items within their Pages to create the content projects. The Exhibits have already been created for this project, but your class will be providing all of the Items and Pages for those Exhibits.


## Items
**Watch this video tutorial for an Introduction to Items:** (https://mediaspace.msu.edu/media/LEADR_Tutorial_Omeka-Items/1_rip7ls0b).

In Omeka, an Item largely consists of any digital resource(s) and its associated metadata. A digital resource typically refers to any audio, image, or video file(s) which is historically or culturally significant to your project. A digital resource on its own, however, is not incredibly useful without some context. In the case of a photograph, we would want to know things like what the title is, the background description, and who the photographer is. This type of data is referred to as metadata. We can go deeper into metadata later, but just for now think about metadata as the necessary context behind your digital content. The following sections will show you the basics of creating, editing and searching for Items in Omeka.


### *Creating Items*
*For the purpose of this tutorial, we will be using fossils as an example.*

1. Select the **Items** tab from the admin dashboard to access the Browsing Items page. From the Browse Items page, you may browse, add and search for Items.
<img src="img/Items-and-exhibits/itemsandexhibits1.png" width="40%">
2. Click on the **Add an Item** button from the Browse Items page
<img src="img/Items-and-exhibits/itemsandexhibits2.png" width="40%">
3. This will initially bring you to the **Dublin Core** tab where you will fill out fields describing your Item. This tab usually provides the bulk of what makes up an Item. You will want to fill out as much of the Dublin Core tab as possible, especially: **Title**, **Subject**, **Description**, **Source**, and **Publisher**. There is no problem, however, with leaving a field empty when metadata is simply not available.
  - *Note: this tab is called “Dublin Core” because that is the metadata standard that Omeka uses. A metadata standard refers to the use of the same “entities” for the description of data (digital resources in our case). The “Title” field is an example of an “entity”. Use of the same, standardized entities across multiple collections of data makes it easier to search and compare data (digital resources) across multiple collections. Sometimes the websites that you obtain your content from will have options to specifically format the metadata into the metadata standard we are using.*
<img src="img/Items-and-exhibits/itemsandexhibits3.png" width="40%">
4. Once you have added the metadata, click on the Item Type Metadata tab. This tab is usually reserved for describing the type of digital content that you are uploading.
<img src="img/Items-and-exhibits/itemsandexhibits4.png" width="40%">
  - Select **fossil** from the dropdown menu.
  - Fill out as much of the metadata as you can.
5. After you finish entering the Fossil Item Type Metadata, select the Files tab to add a digital resource(s) for your Item.
  - Click on the **Browse…** button to select and download the digital resource(s) into your Omeka Item.
6. The final data-entry step is the application of tags to your Omeka Item. For the purposes of this class, you may add in any relevant subject tags you would like, though they are not necessary. Simply enter in the text for your tags (separated by commas) and press the **Add Tags** button.
7. Now you can add your Item. Before adding your Item, **make sure your item is public** (viewable on the actual website) by checking the **Public** check box under the Add Item button. Finally, Press the **Add Item** button.
<img src="img/Items-and-exhibits/itemsandexhibits5.png" width="40%">
8. h.	This will bring you back to the *Browse Items* page where you will receive a message saying that your Item was successfully added.

#### *Viewing, Editing, and Deleting your Item*
1. You may view the details of, edit or delete an Item at any time by browsing or searching (see next section) for an Item that you have created.
2. Once you have found the location of your Item click on the button for the corresponding action you want to take.
  - The “**Details**”, “**Edit**” and “**Delete**” buttons will be located under your Item’s title.
<img src="img/Items-and-exhibits/itemsandexhibits6.png" width="40%">

#### *Searching for Items*
1. Navigate to the Browse Items page and click the search button.
<img src="img/Items-and-exhibits/itemsandexhibits7.png" width="40%">
2. You may search for an Item using any number of categories, but it will probably be most useful to search by user, using the username you provided.
3. Once you have entered your search criteria, press the *Search for Items* button.
4. Results should appear with any Items matching your search criteria.

## Exhibits
**Watch the video tutorial introduction to Exhibits. It can be found here:** https://mediaspace.msu.edu/media/LEADR+Omeka+Exhibits+Video+Tutorial/1_9cdxrdim

In Omeka, Exhibits combine Items and your textual analysis to create a public, online exhibit. Exhibits are composed of pages, typically with a page that serves as the introduction to a project and additional pages which highlight the Items and component text. An Omeka exhibit may be one or more pages in total, depending on the project. The following sections will show you the basics of creating and editing exhibits in Omeka.

#### *Creating Exhibits*
1. On your dashboard, select **Exhibits** on the left hand menu. 


#### *Advanced Settings for Your Search*
There are several advanced setting options in row 13 to 17 of your TAGS sheet. These functions are summarized below:
- Period: This period allows you to specify how far back into the past you want to scrape tweets for (up to 7 days). Note that your search will automatically search 7 days into the past if left blank.
- Follower Count Filter: You may use this option to specify particular users who have a minimum number of followers.
- Number of Tweets: If you want to collect Tweets for a longer period of time, then you can increase this number. Experience has shown that TAGS usually meets the limit in less than a month if this is not changed.  
- Type: This specifies whether you want to use search terms to scrape tweets or if you want to scrap the favorite tweets or statuses of a particular user.

#### *Scrapping Tweets*
Once you have your search terms and settings in place, follow these steps to scrape Twitter for Tweets:
- Go to the TAGS tab and select either "Run Now!" Or "Update Archive every Hour".
  - If you want a one time dataset, select Run Now!
  - If you want to continually take data, say in preparation for some event, select Update Archive every Hour.
    - Twitter only allows you to scrape Tweets from the past 7 days. So, if you want to analyze tweets for an extended period of time, you will have to do some planning.
    - For instance, if you want to analyze tweets before and after a political event, you could set up TAGS to scrape tweets beforehand. But, be sure to keep an eye on whether or not your TAGS sheet has reached your tweet limit before the event is over. <img src="img/tags/TAGS_10.png" width="90%">
- After running TAGS, tweets that meet your criteria will be found in the Archive tab at the bottom of your Google Sheet. <img src="img/tags/TAGS_11.png" width="90%">

## Downloading Your Data
Once you’ve scrapped some tweets, TAGS will provide you with a Google Sheet containing the actual Tweets, their creator, creation date and other metadata in the Archives section. Follow these steps to download your data:
1. Go to the file tab
2. Select download
3. Choose the format that you want to download your data in and click on it.
  - Excel and .csv formats will work well in Voyant. <img src="img/tags/TAGS_12.png" width="90%">

## FAQ
*How does TAGS work?*
- TAGS works by making requests for tweets (that meet your criteria) to Twitter’s Application Program InterfaceI (API). The API essentially acts as an administrator who decides whether or not to give you the Tweets that you are asking for. This means that Twitter is policing which tweets are sent to you.

*How does Twitter’s API affect my dataset?*
- There are many conditions that the Twitter API will run your request through before getting you your dataset. It is important that you consider how your dataset is made before making analyses. The following two conditions are significant in this regard:
  - The Twitter API will automatically prefer Tweets from more popular and connected users.
  - Twitter only lets you scrape Tweets within the last 6-9 days.

*If TAGS and Twitter give me a curated dataset, why are we using them?*
- While it’s true you are not getting a perfect dataset, that was never a possibility. Certain populations do not use social media and it is up to you to take all these factors into account when explaining your analysis. That being said, TAGS does provide a way to collect HUGE amounts of data from people publicly giving their opinion on issues. Using this data responsibly and correctly is extremely valuable.

*How do I use this data?*
- There are as many purposes for your data as you can imagine. You can examine the actual tweets users have submitted it, where they are from, how the tweets changed over time and so on.
There are numerous resources for learning how to visualize data including Voyant, Excel, R, Python, and Flourish. Voyant is a good option and LEADR  provides a handout.

*How do I collect useful data?*
- Much of this will be trial and error. Different search terms, hashtags and users will all greatly affect what your dataset looks like. Try to think critically about what issue you are looking into and how best to examine it with TAGS.

*My TAGS is not working or I did not get any results and want to do a new search. How do I reset?*
- The easiest way to reset TAGS is to simply create a new sheet. You may have multiple instances of TAGS running, and setting up a new sheet is much easier once you have already gone through the process.

## Assessment
By the end of this tutorial, you should have TAGS and be able to scrape for tweets in a variety of ways. This should provide you tabulated datasets that can be very large. Visualizing this data will be the next step in your analysis.

Keep in mind that how you got the data, and how you choose to visualize it will greatly affect your analysis. There are a number of ways to visualize data, but one way to analyze and visualize the textual data of TAGS is through Voyant. Check out the LEADR tutorial on this subject to learn more.

-----
### Return to [LEADR's Resources list](https://leadr-msu.github.io/)
