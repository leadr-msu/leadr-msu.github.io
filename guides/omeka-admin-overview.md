# Omeka Administrative Overview
Created by Dawson McCall, Brandon Locke, and Autumn Painter

*Last Updated: 12/16/2017*

## Omeka Overview
*This older guide covers an overview of functions that are useful for administrators trying to set up an Omeka website. If you are a student looking for help on your projects, we recommend checking out the Omeka guides on [Items and Exhibits](https://leadr-msu.github.io/guides/omeka-items-and-exhibits.html), [Pages](https://leadr-msu.github.io/guides/omeka-pages.html), [Metadata](https://leadr-msu.github.io/guides/omeka-metadata.html), and [Footnotes](https://leadr-msu.github.io/guides/omeka-footnotes.html).*
* Omeka is a web-publishing platform for the online display and curation of visual collections and exhibitions.
* Great tool for projects utilizing visual images, physical objects, and material culture items.
* Some of the most important Omeka features include: standards-based metadata and web design, data migration tools, exhibit building, curation and organization of material culture items/collections/exhibits, tagging features, and timeline and Google Maps plugins.
* Good overview video for Omeka here - [Omeka Documentation, 2.0 Overview (Video)](https://vimeo.com/55973380)

## Dublin Core & Omeka
* Dublin Core is a metadata schema (set of terms) used as a common set of descriptors for the presentation of online resources (digital and material).
* Omeka uses the Dublin Core metadata schema in order to help organize, describe, and document the content of your Omeka projects.
* Omeka provides a short description of how you can effectively work with the Dublin Core Schema - [Omeka Documentation, Working with Dublin Core](http://omeka.org/codex/Working_with_Dublin_Core)

## Omeka Organizational Schema
* The most important thing to understand about Omeka is the organizational hierarchy for content that Omeka operates from.
* There are three basic hierarchical groupings for organizing your content within Omeka - Items, Collections, and Exhibits. Each of these builds on or pulls from each other depending on your organizational criteria.
* Items are the individual pieces in your collection.
* Collections are groups of items that have some common trait (theme, time period, artist, etc) that is important for the organization of your project.
* Exhibits are essentially the entire project that you are presenting (made up of individual Items that are grouped into Collection).
* IMPORTANT NOTE - The Exhibit feature has to be added with a plugin (it is easy - just follow the steps in the documentation sheet below at #3 of this section).
* Below are some brief descriptions of these organizational groups:
  1. Items - [Omeka Documentation - Managing Items 2.0](http://omeka.org/codex/Managing_Items_2.0)
  2. Collections - [Omeka Documentation - Managing Collections 2.0](http://omeka.org/codex/Managing_Collections_2.0)
  3. Exhibits - [Omeka Documentation - Exhibits, Plugins/Exhibit Builder 2.0](http://omeka.org/codex/Plugins/ExhibitBuilder_2.0)

## Design and Finishing Touches
### Themes
While most really good Omeka projects include heavy CSS and PHP customization, there are several things you can do to make the project look a lot better. The themes give you a number of good jumping-off points. It usually helps to have at least a few items in and an exhibit created before changing themes - otherwise it can be difficult to discern exactly what the project looks like.

To change the theme, click on 'Appearance' at the top of the screen, and you'll go directly to the theme page. You can easily test any of them out by clicking 'Use this theme' and then looking at the public view of the project. Each Omeka install will have all of the themes that are available and have been vetted by the developers of Omeka.

### Configuring a Theme
Each theme will have a 'Configure Theme' button once it is selected. Configurations let you make choices about the look of your site, including adding a logo and homepage text, managing featured elements, and adding footer text. The configuration settings you make are unique to each theme and will be saved with that theme. Not all themes have the same configuration settings.

To configure your theme, click the “Configure Theme” button below the theme graphic to customize your site. While not all themes have the same configuration settings, most will have the following two sections:

**Header and Footer configuration options are:**

* Logo file. You may upload a logo file that will replace the site title in the header of the theme. Recommended maximum width for the logo is 500px.
* Header image. Upload an image file that will display across the top of each of your public website's pages, usually below the navigation bar.
* Background image. Upload an image file that will display, tiled, in the background of each of your site's pages.
* Footer text. An HTML-enabled text box where you can enter text for a site footer to appear on every page.
* Display copyright in footer. Check this box if you wish to display your site’s copyright information in the footer. Site copyright information is found in the General Settings section.
* Use Advanced Site-wide search. Check this box to allow public-side site visitors to search the whole site, including items, collections, and files, and to use boolean methods when searching.

**Homepage configuration options:**

* Display Featured Item. Check this box if you wish to show a featured item on the homepage.
* Display Featured Collection. Check this box if you wish to show a featured collection on the homepage.
* Display Featured Exhibit. Check this box if you wish to show a featured exhibit on the homepage.
* Homepage Recent Items. Choose the number of recent items to be displayed on the homepage. These will appear in the order in which they were mostly recently added to the archive.
* Homepage Text. Add some text to be displayed on your homepage above the Featured Items. This is a good place to add a very short tagline or description of your site.

Save longer explanations for an About page.

Remember to save changes.

### Navigation
You can customize the navigation bar by clicking 'Appearance' at the top of the screen, and then clicking on the 'Navigation' tab. You can rename or remove the default links from the bar, add links to specific Collections, Exhibits, or Simple Pages, or add external links on this screen.

### Changing the default home page
You can change the default home page by clicking 'Appearance' at the top of the screen, and then clicking on the 'Navigation' tab. On the right, there is a dropdown where you can select the default home page. If the page you want to be your home page is not listed, you need to add the link to the navigation list (you can uncheck it so that it does not appear in the menu) and then select that as your home page.

### Adding an Image to the Exhibit Landing Page
* The student will need the image URL
* Then go the the exhibit tab
* Click your exhibit, press edit
* Under “exhibit metadata” go to the description box
* Click the HTML option on the top right menu bar for that box
* It will open a “HTML Source Editor”
* If you would like the image at the bottom of your exhibit description, place the code below underneath the existing text (if you would  like it at the top of the page, place the code before any of the existing text
  * <img src=“YOUR URL" alt="cemetery" style="width: 50%;" />
* Replace YOUR URL with the url of the image between the quotation marks
* You can adjust the width of the image by percentage
* Press Update
* Press Save Changes
* Then View Public Page to check that it worked


## Other Useful Omeka Video Tutorials & Documentation
- [Omeka Documentation - Managing Tags](http://omeka.org/codex/Managing_Tags_2.0)
- [Omeka Documentation - Managing Themes](http://omeka.org/codex/Managing_Themes_2.0)
- [Omeka Documentation - Managing Navigation](http://omeka.org/codex/Managing_Navigation_2.0)

-----
### Return to [LEADR's Resources list](https://leadr-msu.github.io/)
