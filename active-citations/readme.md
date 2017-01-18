# Active Citations
Prepared by Sara Bijani

Like any academic project, your webpages need to properly acknowledge your sources. The most straightforward way to do this is to provide a bracketed number ([1]) after the text being cited, and to manually insert the citation at the bottom of your document (1. Your Citation). Unlike a printed document from a static word processor, however, your web citations can easily be made interactive. The examples below offer three different ways of presenting online citations, with increasing complexity.

##CLICKABLE FOOTNOTES 
Rather than using plain text as you would in a word processor, you can take advantage of the interactive dynamics of HTML to make footnotes in your web writing clickable. In order to do this, you will first need to name each of your footnotes in html.  The basic script to accomplish this follows. You will replace “footnote1” with your own information. 
    
    
    <a name="footnote1">
    Footnote 1
    </a>
    


This functions as an anchor tag, not a link. After your footnotes are named, you will need to make the footnote marker (for example: “[1]”) into a tag that refers to the appropriate named section. The basic script to accomplish this uses the # sign, as follows: 
    
    
    <p>Text of cited sentence.
    <a href="#footnote1">[1]</a>
    </p>

##CLICKABLE FOOTNOTES WITH RETURN 
It is also possible to write HTML that will return your reader to the place in the text where they clicked down to your footnote. The script to accomplish this modifies the HTML in the main text body as well that that surrounding the footnote itself. To do this, you will replace the code you used in the previous example. This first block of code is what you will use in the main text of your writing to link to your footnotes."Text to footnote mark" is your writing to the point where you wish to insert your own footnote mark. You will replace “_ftnref1” with your own information. 
    
    
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

##ADDING POP OVER DESCRIPTIONS FOR BIBLIOGRAPHIC TEXT 
This requires an active Javascript Framework, which LEADR staff will construct for you. Be sure to request this before attempting to use the following code. This pop over will appear over a parenthetical citation at the end of a sentence of referenced material. At this point in your writing, insert the following code. You will replace “bibliographic entry” and “Author, p#” with your own information. 
    
    
    <a  href="#" rel="citation"
    data-toggle="popover"
    data-content=“bibliographic entry”>
    (Author, p#).
    </a>.

##APA (AMERICAN PSYCHOLOGICAL ASSOCIATION) STYLE TIPS
This is the preferred citation method for those working in the social and natural sciences, including but not limited to Sociology, Anthropology, Psychology, Political Science, and much more. If a field tends to generate rapid publications and the need to cite by publication date is significant, this is the best tool. All sample citations are drawn from Purdue University's Online Writing Lab: [here](https://owl.english.purdue.edu/owl/section/2/10/). "When using APA format, follow the author-date method of in-text citation. This means that the author's last name and the year of publication for the source should appear in the text, for example, (Jones, 1998), and a complete reference should appear in the reference list at the end of the paper.If you are referring to an idea from another work but **NOT** directly quoting the material, or making reference to an entire book, article or other work, you only have to make reference to the author and year of publication and not the page number in your in-text reference. All sources that are cited in the text must appear in the reference list at the end of the paper." 

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

Online scholarly journal articles without a DOI require the URL of the journal home page. Remember that one goal of citations is to provide your readers with enough information to find the article; providing the journal home page aids readers in this process.

Author, A. A., & Author, B. B. (Date of publication). Title of article. Title of Journal, volume number. Retrieved from http://www.journalhomepage.com/full/url/

Kenneth, I. A. (2000). A Buddhist response to the nature of human rights. Journal of Buddhist Ethics, 8. Retrieved from http://www.cac.psu.edu/jbe/twocont.html

##CHICAGO STYLE TIPS

This is the preferred citation method for those working in the field of history. Examples of some of the most commonly used items are listed below. This style is ideal for hard to locate and unique sources, such as those found in archives. All sample citations are drawn verbatim from the Chicago Manual of Style Online, 16th Edition. The full electronic style guide is available through the MSU library: here.

##### BOOK WITH SINGLE AUTHOR OR EDITOR
For a book with a single author, invert the name in the bibliography but not in the notes. Punctuate and capitalize as shown. Note the shortened form in the second note. Note also that actual page numbers cited are usually included in a note but not in a bibliography entry, unless the entry is for a chapter, in which case the page range in which the item appears is included.

Footnote:
1. Michael Pollan, The Omnivore’s Dilemma: A Natural History of Four Meals (New York: Penguin, 2006), 99–100.
18. Pollan, Omnivore’s Dilemma, 3.

Bibliography:
Pollan, Michael. The Omnivore’s Dilemma: A Natural History of Four Meals. New York: Penguin, 2006.

##### BOOK WITH MULTIPLE AUTHORS
For a book with two authors, note that only the first-listed name is inverted in the bibliography entry.

Footnote:
2. Geoffrey C. Ward and Ken Burns, The War: An Intimate History, 1941–1945 (New York: Knopf, 2007), 52.

Bibliography:
Ward, Geoffrey C., and Ken Burns. The War: An Intimate History, 1941–1945. New York: Knopf, 2007.

##### JOURNAL ARTICLE
Citations of journals include the volume and issue number and date of publication. The volume number follows the italicized journal title in roman and with no intervening punctuation. A specific page reference is included in the notes; the page range for an article is included in the bibliography. In the full citation, page numbers are preceded by a colon. If a journal is paginated consecutively across a volume or if the month or season appears with the year, the issue number may be omitted (as in the second and third sets of examples below).

Footnote:
89. Walter Blair, “Americanized Comic Braggarts,” Critical Inquiry 4, no. 2 (1977): 331–32.
111. Blair, “Americanized Comic Braggarts,” 335.

Bibliography:
Blair, Walter. “Americanized Comic Braggarts.” Critical Inquiry 4, no. 2 (1977): 331–49.

##### ARTICLE WITH DOI ASSIGNED

The DOI in the following example indicates that the article was consulted online; it is preferred to a URL (see also 14.5, 14.6). Note that DOI, so capitalized when mentioned in running text, is lowercased and followed by a colon (with no space after) in source citations. Shortened citations for subsequent references to an online source follow the forms for printed books and journals.

Footnote:
1. William J. Novak, “The Myth of the ‘Weak’ American State,” American Historical Review 113 (June 2008): 758, doi:10.1086/ahr.113.3.752.
3. Novak, “Myth,” 770.

Bibliography:
Novak, William J. “The Myth of the ‘Weak’ American State.” American Historical Review 113 (June 2008): 752–72. doi:10.1086/ahr.113.3.752.

##### ARTICLE WITHOUT DOI ASSIGNED

For articles that have not been assigned a DOI (or if the DOI cannot be determined), include a URL. The URL in the following example—consulted through the academic journals archive JSTOR—was listed along with the article as a more stable (and shorter) alternative to the URL that appeared in the browser’s address bar. For access dates (not shown here), see 14.185.

Footnote:
12. Wilfried Karmaus and John F. Riebow, “Storage of Serum in Plastic and Glass Containers May Alter the Serum Concentration of Polychlorinated Biphenyls,” Environmental Health Perspectives 112 (May 2004): 645, http://www.jstor.org/stable/3435987.

Bibliography:
Karmaus, Wilfried, and John F. Riebow. “Storage of Serum in Plastic and Glass Containers May Alter the Serum Concentration of Polychlorinated Biphenyls.” Environmental Health Perspectives 112 (May 2004): 643–47. http://www.jstor.org/stable/3435987.
