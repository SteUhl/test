---
title: "Using the Bibliography"
teaching: 0
exercises: 1
---

::: questions 

- What is the bibliography feature in Quarto?
- How do you use and expand the bibliography and citations?
- How do you implement footnotes?
  
:::

::: objectives

- Learn the basics of citations and footnotes in Quarto.
- Create and expand your own bibliography and implement it in your document.

:::

One of the most important aspects of scientific publishing is the inclusion and organisation of sources,. citations and footnotes. These are all included in Quarto, which offers an integrated menu to organize and implement Citation from a variety of different sources.

::: callout

For this part of the lesson, we will switch from Source Mode to Visual Mode, in order to offer you an easier to understand guide on how to use these.

:::

## Footnotes:

Footnotes offer an easy way to add useful information or literature to your text. 
They can be implemented into your Quarto document by using the Insert -> Footnotes option in the Visual Mode of Quarto.
<img style="float: right;" src="https://pad.zdv.net/uploads/824de089-c707-4076-bd50-3c2c8fe24fe6.png">


Once selected you can add your information to the text box that appeared in the bottom of your screen.
![](https://pad.zdv.net/uploads/f69b9028-a0a5-4a94-b84e-b8d52cfdc40d.png)

## Citations

In a similar vein to footnotes, you can also directly add citations to your document. This can be done through the Insert window of the Visual Mode:
![](https://pad.zdv.net/uploads/563f1c2c-4aab-4a60-84b5-222be982b5f3.png)

Doing so will accomplish two things: It will open a new window called "Insert citation", and it will create a new file called "references.bib" in your working folder.
![](https://pad.zdv.net/uploads/f0b75353-7f33-47b4-8fa5-d8e9c426e3d3.png)

This new file will contain your newly created bibliography, which can now be filled in a variety of ways.
The easiest to do are the four already integrated options of either searching for a publication through their DOI (a unique number given to all published articles and books) or by searching through the databases of Crossref, Datacite or Pubmed.
Simply add relevant information such as the DOI, Title or name of the author n the search bar and see what you can find there. In the best case your needed citation is already part of one of these databases.
![](https://pad.zdv.net/uploads/cd890f7b-1d12-4520-b29c-b3dbc5a34fb4.png)
If you found your publication, you can use the + button on the right to quickly add it to your bibliography.

Should you not be able to find something through these integrated means, you can simply add it manually. 
In order to do this, you need to open your newly created references.bib file with a text editor of your choice. This can also be done in Visual studio code.
![](https://pad.zdv.net/uploads/8d54b57f-26b4-4351-bd46-c2dd7b9bfecd.png)

In this file you will find all your already added references in form of code chunks.
The citation function uses a format called Bibtex, which is used by a variety of databases. 
It is in part made up of a reference name, signified by a @, which is used internally as a unique signifier of this specific reference. Following this are the reference name, which will be shown in your Quarto document when using the citation function, and a variety of information inside {} brackets. These contain the relevant metadata of the publication.

You can now simply add further objects to your list of references by either manually typing in additional sources, or by copy and pasting the relevant BibTex chunks from other websites. Many Websites used to publish academic texts, such as Jstor, or libraries offer the download oft txt files containing the relevant BibTex Chunks as part of their own citation functions.
Here is an example using Jstor:
![](https://pad.zdv.net/uploads/5e1e52c0-b40b-4217-8b7a-5fea18bd0d23.png)

And here is how it looks when added to your reference.bib file:
![](https://pad.zdv.net/uploads/d1dae321-6e50-413c-8d6b-4a9ba28a432e.png)


Once you have added the new code chunk to you refernces.bb file, you can save and return to your "Insert Citation" window.
Here you will now find your newly added reference as part of you bibliography:
![](https://pad.zdv.net/uploads/562e323b-2d6f-44f1-be83-9c12500b6e8d.png)

Now you can simply click on the different references in order to insert them into your work. This will create a reference in the following format: [@testtes2019] in source mode.
The rendered Document will have the Authors name and the publication date in brackets in its place.
Using the reference feature will also create a reference index at the bottom of your rendered document. This index will contain a full bibliographical list of all used refences, using the information contained in the reference.bib file.
The result could look something like this:
![](https://pad.zdv.net/uploads/ac0a8052-eab4-4bb9-8a88-6fd106b1c310.png)

::: challenge
### Exercise
Use the **References** and **Footnote** features to enrich your document with citations.  
Create and fill out a bibliography, then render your document one last time.
:::
