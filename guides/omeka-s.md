# Omeka-S Tutorial
Created by Jen Andrella

*Last Updated 12/16/2021*

## Omeka S Overview

On the dashboard, there is a navigation bar on the left and the main work area on the right.  "Manage Resources" provides links and summary accounts for Items, Item Sets, Vocabularies, and Resource Templates. "Manage Sites" lists all sites within the Omeka S installation.  Clicking on the name of a site will direct users to the public view, while clicking on the edit button (pencil icon) will direct users to the editing base.  

## Navigation

On the left-side navigation column, users will see a section heading for "Resources."  This contains all of the tools to build content in Omeka S:
* Items
* Item Sets
* Vocabularies
* Resource Templates

Below these options the user will see the the Administrator system settings to manage all websites on the Omeka S installation, including:
* Users (single or batch-add)
* Modules (plug-ins to extend functionality)
* Jobs
* Settings

## Key Terminology and Concepts

* Item:  A digital representation of a piece of content in which you can attach metadata and upload multiple forms of media.  Items are the building blocks of every Omeka platform, but function a little differently in Omeka S. When users click on the pencil "edit" icon, it will take them to an interface where they will enter metadata information. A new feature is that users will choose which metadata fields they would like to complete based on a list of four different "Properties" that will appear in a side bar on the right side of the screen. Here, users can choose fields from the property lists:
  * Dublin Core (Omeka's standard metadata fields)
  * Bibliographic Ontology
  * Friend of a Friend (Ideal for genealogical projects)
  *Example: Usually a primary or secondary source such as a painting, document, legislation, interview clip, book, newspaper, etc

* Item Set: A group of "Items"  organized around a similar inherent features, like an idea, person, or place.  If multiple Items have the same owner/contributor or archival/museum collection, then creating an Item Set for these objects is an appropriate form of organization. Every Item Set will have its own metadata, and is structured very similarly to "Collections" in Omeka Classic.  The difference is that any Item can appear in one or more Item Sets as users deem necessary.
*Example: The Item Set titled: "William Shakespeare" would include include the Items: ''Romeo and Juliet'', ''Othello'', and "Macbeth."

A new feature of Omeka S is the ability to enter an existing Item or Item Set as the value for a property field.  For example, the Item Set based on "William Shakespeare" can be entered into the "Author" field of an Item. This way, any work with the same author will be connected together.

* Resource Templates: Allows users to create custom sets of metadata properties from any of the categories or a combination of them, and name it. You can then select the resource template when creating an Item or Item Set and it will be added to the metadata form. This feature can simplify the workload when adding a multitude of similar items. This function is similar to "Item Type" in Omeka Classic, but has more flexibility in type-specific metadata.

## Adding and Managing Content

* Create a Website:  On the Admin dashboard, select the "Add Site" button which will open a New Site start-up page with fields to enter the website title and URL slug (or Omeka will generate one automatically). The next tab shows the choices for different themes of appearance. Lastly, the "Item pool" tab is where you can create pools of items between Omeka sites and set specific search settings.

When you are done, click "Add" and your new site will appear on the dashboard ready to upload and manage content.

* Items
To add an item, follow these steps:
1. Go to "Items" under resources and then click the gray button "Add new item."
2. Select a resource template that best applies to the item's type (film, artwork, textual work, a custom template, etc.).  Also select a "class" to claim a metadata type.  
3. Adding a resource template and class will change the kinds of metadata fields available to enter information. To add more fields,     
   skim through the "properties" column on the right side of the page and choose which fields you would like to add to your item's
   metadata information.  Choose properties from "Dublin Core," "Bibliographic Ontology," and "Friend of a Friend" as the user sees
   appropriate for their item.
4. Click the media tab to upload media from your computer, through a URL, HTML, IIIF image, oEmbed, or Youtube.  
5. Select the "Item set" tab to add the item to a pre-created Item set. (i.e.  This is where authors might connect their works to a
   specific donor, artist, creator, etc.).
6. Lastly, click "Add" and the item will appear in the list with the others.  Edit the item at anytime by selecting the pencil icon.

* Item Sets:
To create an item set, follow these steps:
1. Click the "Item Sets" tab from the left navigation column on the dashboard, then click "add new item set."
2. If you have a resource template preference, you may select a specific resource template. Otherwise, select Dublin Core, Bibliographic Ontology, or Friend of a Friend from the right column and enter the metadata information available for the item set.  

* Pages to a Website:
To edit and add new pages to a website, follow these steps:
1. Using the left navigation column on the admin dashboard, you can edit existing pages or "Add new page."
2. Once you add a new page, enter a title and click "add." You will then be directed back to the interface for all pages.  Click the pencil "edit" icon to edit and add content to your page.
3. In the edit interface, notice the selection of content blocks that you can add to the page.  Once you add your content blocks of choice, you can drag them to reposition their order on the page.  
4. Various content blocks allow text, media (items), and mapping features.  
5. Once your a finished with the content, layout and design of your page, click "save."

## Modules

For advanced options, modules (i.e. plug-ins) extend the functionality of Omeka S.These must be downloaded separately to your Omeka S installation.
  * Collecting- Add collecting forms to your sites
  * CSV Import- Import content from a CSV file
  * Custom Vocab- Describe your resources using vocabularies you create
  * Dspace Connector- Connect Omeka S to DSpace repositories
  * Fedora Connector- Connect Omeka S to Fedora 4 repositories
  * File Sideload- Add files that are already on your server to items
  * Folksonomy- Add tages and tagging form to any resource to create uncontrolled vocabularies and tag clouds
  * IIIF Server- Integrates the IIIF specifications and a simple IIp Image Server to allow processing and instant sharing of any sized
    images and media (PDF, audio, 3D, etc.)
  * Mapping- Add location information to your items and sites
  * Metadata Browse- Adds a link to sane results for metadata values
  * Omeka 2 Importer- Import content from an omeka 2 site via its API
  * PDF Embed- Embed PDF files within Omeka S pages
  * Rights Statements- Add a "rights" data type to a property
  * Search- Add search capabilities to Omeka S
  * Sharing- Share and embed content on the web
  * Solr- Add Solr search adapter
  * unAPI- Make your item metadata discoverable using unAPI
  * Universal Viewer- Integrates the Universal Viewer in order to create carousels of virtual books from image files and to display any
    media file (PD, audio, video, 3D, etc.) in a unified player
  * Value Suggest- Describe your resources using auto-suggested values from controlled vocabulary services
  * Zotero Import- Import items and files from Zotero user and group libraries
Please visit the [modules registry and download site](https://omeka.org/s/modules/) to download the module(s) to your Omeka S installation.

-----
### Return to [LEADR's Resources list](https://leadr-msu.github.io/)
