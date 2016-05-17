title: Active Citations
link: http://leadr.msu.edu/resources/active-citations/
author: bijanisa
description: 
post_id: 1183
created: 2016/02/12 17:51:42
created_gmt: 2016/02/12 17:51:42
comment_status: closed
post_name: active-citations
status: publish
post_type: page

# Active Citations

[et_pb_section][et_pb_row][et_pb_column type="4_4"][et_pb_image admin_label="Image" src="http://leadr.msu.edu/wp-content/uploads/2016/02/Screen-Shot-2016-02-12-at-12.39.20-PM.png" show_in_lightbox="off" url_new_window="off" animation="left" /][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Intro" background_layout="light" text_orientation="left"] 

Like any academic project, your webpages need to properly acknowledge your sources. The most straightforward way to do this is to provide a bracketed number ([1]) after the text being cited, and to manually insert the citation at the bottom of your document (1. Your Citation). Unlike a printed document from a static word processor, however, your web citations can easily be made interactive. The examples below offer three different ways of presenting online citations, with increasing complexity.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="1_3"][et_pb_text admin_label="Text" background_layout="light" text_orientation="left"] CLICKABLE FOOTNOTES Rather than using plain text as you would in a word processor, you can take advantage of the interactive dynamics of HTML to make footnotes in your web writing clickable. In order to do this, you will first need to name each of your footnotes in html.  The basic script to accomplish this follows. You will replace “footnote1” with your own information. 
    
    
    <a name="footnote1">
    Footnote 1
    </a>
    

This functions as an anchor tag, not a link. After your footnotes are named, you will need to make the footnote marker (for example: “[1]”) into a tag that refers to the appropriate named section. The basic script to accomplish this uses the # sign, as follows: 
    
    
    <p>Text of cited sentence.
    <a href="#footnote1">[1]</a>
    </p>

    [/et_pb_text][/et_pb_column][et_pb_column type="1_3"][et_pb_text admin_label="Text" background_layout="light" text_orientation="left"] CLICKABLE FOOTNOTES WITH RETURN It is also possible to write HTML that will return your reader to the place in the text where they clicked down to your footnote. The script to accomplish this modifies the HTML in the main text body as well that that surrounding the footnote itself. To do this, you will replace the code you used in the previous example. This first block of code is what you will use in the main text of your writing to link to your footnotes."Text to footnote mark" is your writing to the point where you wish to insert your own footnote mark. You will replace “_ftnref1” with your own information. 
    
    
    <p> Text to footnote mark.
    <a id="_ftnref1" href="#_ftn1">
    [1]
    </a>
    End of your paragraph.
    </p>

  Around the footnotes themselves, you will use this basic script: 
    
    
    <p>
    <a id="_ftn1" href="#_ftnref1">
    [1]
    </a>
    Text of footnote
    </p> 

  [/et_pb_text][/et_pb_column][et_pb_column type="1_3"][et_pb_text admin_label="Text" background_layout="light" text_orientation="left"] ADDING POP OVER DESCRIPTIONS FOR BIBLIOGRAPHIC TEXT This requires an active Javascript Framework, which LEADR staff will construct for you. Be sure to request this before attempting to use the following code. This pop over will appear over a parenthetical citation at the end of a sentence of referenced material. At this point in your writing, insert the following code. You will replace “bibliographic entry” and “Author, p#” with your own information. 
    
    
    <a  href="#" rel="citation"
    data-toggle="popover"
    data-content=“bibliographic entry”>
    (Author, p#).
    </a>.

  [/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_tabs admin_label="Tabs"][et_pb_tab title="APA (American Psychological Association) Style Guide"] This is the preferred citation method for those working in the social and natural sciences, including but not limited to Sociology, Anthropology, Psychology, Political Science, and much more. If a field tends to generate rapid publications and the need to cite by publication date is significant, this is the best tool. All sample citations are drawn from Purdue University's Online Writing Lab: [here](https://owl.english.purdue.edu/owl/section/2/10/). "When using APA format, follow the author-date method of in-text citation. This means that the author's last name and the year of publication for the source should appear in the text, for example, (Jones, 1998), and a complete reference should appear in the reference list at the end of the paper.If you are referring to an idea from another work but **NOT** directly quoting the material, or making reference to an entire book, article or other work, you only have to make reference to the author and year of publication and not the page number in your in-text reference. All sources that are cited in the text must appear in the reference list at the end of the paper." 

##### SINGLE AUTHOR

Last name first, followed by author initials.

Berndt, T. J. (2002). Friendship quality and social development. _Current Directions in Psychological Science, 11_, 7-10.

##### TWO AUTHORS

List by their last names and initials. Use the ampersand instead of "and."

Wegener, D. T., & Petty, R. E. (1994). Mood management across affective states: The hedonic contingency hypothesis. _Journal of Personality and Social Psychology, 66_, 1034-1048.

##### JOURNAL ARTICLE

Online articles follow the same guidelines for printed articles. Include all information the online host makes available, including an issue number in parentheses.

Author, A. A., & Author, B. B. (Date of publication). Title of article. _Title of Online Periodical, volume number_(issue number if available). Retrieved from

http://www.someaddress.com/full/url/

Bernstein, M. (2002). 10 tips on writing the living Web. _A List Apart: For People Who Make Websites, 149_. Retrieved from http://www.alistapart.com/articles/writeliving

Because online materials can potentially change URLs, APA recommends providing a Digital Object Identifier (DOI), when it is available, as opposed to the URL. DOIs are an attempt to provide stable, long-lasting links for online articles. They are unique to their documents and consist of a long alphanumeric code. Many-but not all-publishers will provide an article's DOI on the first page of the document.

Note that some online bibliographies provide an article's DOI but may "hide" the code under a button which may read "Article" or may be an abbreviation of a vendor's name like "CrossRef" or "PubMed." This button will usually lead the user to the full article which will include the DOI. Find DOI's from print publications or ones that go to dead links with CrossRef.org's "DOI Resolver," which is displayed in a central location on their home page.

##### ARTICLE WITH DOI ASSIGNED

Author, A. A., & Author, B. B. (Date of publication). Title of article. _Title of Journal, volume number, _page range. doi:0000000/000000000000 or http://dx.doi.org/10.0000/0000

Brownlie, D. (2007). Toward effective poster presentations: An annotated bibliography. _European Journal of Marketing, 41_, 1245-1283. doi:10.1108/03090560710821161

Wooldridge, M.B., & Shapka, J. (2012). Playing with technology: Mother-toddler interaction scores lower during play with electronic toys. _Journal of Applied Developmental Psychology, 33_(5), 211-218. http://dx.doi.org/10.1016/j.appdev.2012.05.005

##### ARTICLE WITHOUT DOI ASSIGNED