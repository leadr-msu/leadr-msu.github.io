# Manually Topic Modeling Panama Papers News Coverage
Created by Brandon Locke
<br>*Maintained by [LEADR](http://leadr.msu.edu/) under the direction of Alice Lynn McMichael*

*Last Updated: 12/16/2017*

## Learning Goals
> * Demonstrate in simple language how topic modeling works
> * Gain first-hand experience in locating and recognizing topics within a text
> * Know strategies for analyzing corpora and investigating research questions with Topic Modeling Tool results

## "Panama Papers" News Story
The ["Panama Papers"](https://en.wikipedia.org/wiki/Panama_Papers) were about 12 million leaked documents that shed light upon people around the world who were hiding money in offshore entities through the Panamanian company Mossack Fonseca. The news coverage in the immediate aftermath of the leak tended to focus on a wide range of issues from the technical aspects of a hack to the implications of various world leaders and celebrities who were exposed. In the weeks following the leak, I selected 34 articles about the issue and extracted the text content into text files ([see articles below](#all-articles).)

## Manual Topic Modeling Activity
Prior to class: Read [Brett, Megan R. "Topic Modeling: A Basic Introduction." Journal of Digital Humanities.](http://journalofdigitalhumanities.org/2-1/topic-modeling-a-basic-introduction-by-megan-r-brett/)

[Slides are available here](https://docs.google.com/presentation/d/1bSSdl_B1MVvqS3iNaxLDnKLfehyY9Z9rcPml14r7Tpg/edit?usp=sharing)

Topic Modeling is an algorithm that finds [“a recurring pattern of co-occurring words”](https://twitter.com/footnotesrising/status/264823621799780353) in a corpus of text. This does take overall usage of a word across the entire corpus into consideration, so words used often in many documents will not appear in every topic. So, for example, "Panama" will almost certainly be used at least once in every article — the average is about 6.3 times per article. However, "Panama" will only be included in an article's keywords if it's used a significant amount of times *and* has close usage relationships with other words.

Today you'll skim a few articles and try your best to imitate topic modeling algorithms. Your [assigned articles](#article-assignments) can be found below.

Before you start reading your articles, take a look at [the total word usage for all 34 articles (stop words removed)](https://docs.google.com/spreadsheets/d/1db2Rqx08frhsVMZpjUfepxYtrpu__Ag8mXKCVlDcrNc/edit?usp=sharing). Once you have glanced at the list, read your first article. Write (or type) out words that seem unique to the article. This means words that are used disproportionally more often in your article than in others in the corpus. Remember, you’re only looking at words used, not concepts or themes that you're able to discern from them. You’re imitating a computer algorithm, and algorithms are not particularly smart. Once you've finished your first article, do your second.

> **Do your words seem to make sense as one or more topics, or do they seem to be random?**

## Comparing and Analyzing Results
I used [Topic Modeling Tool (TMT)](https://sourceforge.net/projects/topicmodeltool/), an easy-to-use tool for using [MALLET](https://github.com/mimno/Mallet) for topic modeling. TMT produces a set of CSV files and a set of HTML files with your output. Take a look at [these results with 20 topics](http://brandontlocke.com/panamapapers20topics/). (Remember, these aren't labeled topics, they're clusters of words that likely represent a topic.)

> **Are there any identifiable "topics" here? Are there any "topics" that don't seem to make sense?**

If you click on one of the topics, you'll see the list of documents ordered by how closely each document corresponds with the topic. The number in parentheses is the number of times words in the topic appear in the document. Now click on one of the text files. This will show you the full text of the file, and it will also show the topics that align closely with your topic.

Take a few minutes and explore these results. Click through the network of topics and documents and see if you can find any patterns. Look at the articles you read and see how closely your results matched the TMT results.

Once you've examined the results with 20 topics, take a look at the [same articles run with 40 topics](http://brandontlocke.com/panamapapers40topics/).

> **What differences do you see between 20 topics and 40 topics?**
> **Which set do you think are most useful to you? Why?**

## Article Assignments
* Doc 01 [Doc 01](https://www.wordfence.com/blog/2016/04/panama-papers-wordpress-email-connection/)
* Doc 03 [Doc 03](https://www.wordfence.com/blog/2016/04/mossack-fonseca-breach-vulnerable-slider-revolution/)
* Doc 05 [Doc 05](http://www.theguardian.com/politics/2016/apr/09/david-cameron-to-launch-local-election-campaign-as-panama-papers-row-rumbles-on)
* Doc 07 [Doc 07](http://www.independent.co.uk/news/uk/politics/panama-papers-david-cameron-to-announce-tax-taskforce-to-investigate-revelations-as-he-seeks-to-a6976891.html)
* Doc 10 [Doc 10](http://www.nytimes.com/2016/04/06/world/europe/panama-papers-iceland.html)
* Doc 11 [Doc 11](http://observer.com/2016/04/panama-papers-reveal-clintons-kremlin-connection/)
* Doc 12 [Doc 12](http://www.vox.com/2016/4/5/11370646/panama-papers-iceland-gunnlaugsson-resigned)
* Doc 21 [Doc 21](http://www.politico.com/agenda/story/2016/04/the-panama-papers-where-are-the-americans-000083)
* Doc 22 [Doc 22](http://www.nbcnews.com/storyline/panama-papers/why-are-americans-not-included-panama-papers-n551081)
* Doc 28 [Doc 28](http://www.darkreading.com/vulnerabilities—threats/7-lessons-from-the-panama-papers-leak/d/d-id/1324976)
* Doc 29 [Doc 29](http://www.wired.co.uk/news/archive/2016-04/06/panama-papers-mossack-fonseca-website-security-problems)
* Doc 32 [Doc 32](http://www.nationalreview.com/article/433696/national-security-agency-panama-papers-prove-its-worth?target=author&tid=1022644)
* Doc 34 [Doc 34](https://www.helpnetsecurity.com/2016/04/07/panama-papers-lax-security-practices/)

## All Articles
1. https://www.wordfence.com/blog/2016/04/panama-papers-wordpress-email-connection/
2. http://gizmodo.com/is-this-how-a-hacker-got-the-panama-papers-1769836788
3. https://www.wordfence.com/blog/2016/04/mossack-fonseca-breach-vulnerable-slider-revolution/
4. http://wptavern.com/outdated-and-vulnerable-wordpress-and-drupal-versions-may-have-contributed-to-the-panama-papers-breach
5. http://www.theguardian.com/politics/2016/apr/09/david-cameron-to-launch-local-election-campaign-as-panama-papers-row-rumbles-on
6. http://www.independent.co.uk/news/world/politics/the-not-completely-crazy-theory-that-russia-leaked-the-panama-papers-a6977271.html
7. 	http://www.independent.co.uk/news/uk/politics/panama-papers-david-cameron-to-announce-tax-taskforce-to-investigate-revelations-as-he-seeks-to-a6976891.html
8. http://www.bbc.com/news/world-europe-35975893
9. http://time.com/4283587/these-5-facts-explain-the-massive-political-fallout-from-the-panama-papers/
10. http://www.nytimes.com/2016/04/06/world/europe/panama-papers-iceland.html
11. http://observer.com/2016/04/panama-papers-reveal-clintons-kremlin-connection/
12. http://www.vox.com/2016/4/5/11370646/panama-papers-iceland-gunnlaugsson-resigned
13. http://latino.foxnews.com/latino/news/2016/04/08/americans-lucked-out-in-panama-papers-scandal-founder-didnt-like-taking-us/
14. http://www.nbcnews.com/business/business-news/why-few-americans-panama-papers-lawyer-doesn-t-want-them-n553116
15. http://www.nytimes.com/2016/04/08/world/europe/vladimir-putin-panama-papers-american-plot.html
16. http://www.theguardian.com/commentisfree/2016/apr/07/panama-papers-taxes-universal-basic-income-public-services
17. https://www.rawstory.com/2016/04/heres-why-so-few-americans-appear-in-the-panama-papers/
18. http://www.usatoday.com/story/news/2016/04/06/panama-papers-americans-with-past-financial-crimes/82704788/
19. http://bigstory.ap.org/article/ef45a25e39224a7989894334aa44bfd4/why-few-americans-panama-papers-lawyer-doesnt-want-them
20. http://fusion.net/story/287671/americans-panama-papers-trove/
21. http://www.politico.com/agenda/story/2016/04/the-panama-papers-where-are-the-americans-000083
22. http://www.nbcnews.com/storyline/panama-papers/why-are-americans-not-included-panama-papers-n551081
23. http://fortune.com/2016/04/09/bad-security-panama-papers/
24. http://www.forbes.com/sites/thomasbrewster/2016/04/05/panama-papers-amazon-encryption-epic-leak/#47b5058a1df5
25. http://www.bbc.com/news/world-latin-america-35975503
26. http://www.computerworld.com/article/3052218/security/the-massive-panama-papers-data-leak-explained.html
27. http://www.computerweekly.com/news/450280758/Panama-Papers-revealed-by-graph-database-visualisation-software
28. http://www.darkreading.com/vulnerabilities—threats/7-lessons-from-the-panama-papers-leak/d/d-id/1324976
29. http://www.wired.co.uk/news/archive/2016-04/06/panama-papers-mossack-fonseca-website-security-problems
30. http://www.wired.com/2016/04/security-week-panama-papers-law-firm-seriously-shoddy-security/
31. http://www.wired.com/2016/04/reporters-pulled-off-panama-papers-biggest-leak-whistleblower-history/
32. http://www.nationalreview.com/article/433696/national-security-agency-panama-papers-prove-its-worth?target=author&tid=1022644
33. http://thehackernews.com/2016/04/panama-paper-corruption.html
34. https://www.helpnetsecurity.com/2016/04/07/panama-papers-lax-security-practices/

-----
### Return to [LEADR's Resources list](https://leadr-msu.github.io/)
