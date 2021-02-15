---
title: SciSpy - intelligent search
subtitle: Use machine learning to find related terms in scientific papers
date: '2016-10-10'
thumb_image: images/Screenshot_2021-02-07 https scispy github io.png
thumb_image_alt: 'White, black, and red shoe sole'
image: images/Screenshot_2021-02-07 https scispy github io.png
image_alt: 'White, black, and red shoe sole'
template: project
---
The vast and growing number of publications in all disciplines of science cannot be comprehended by a single human researcher. As a
consequence, researchers have to specialize in narrow subdisciplines, which makes it challenging to uncover scientific connections beyond the
own field of research.

### The Problem

As an interdisciplinary scientist. even finding the right word to search for is not easy if you are unfamiliar with a new topic or field. When reading a paper, searching for relevant sections using CTRL+F is too dumb. Searching for "feeding" won't show potentially relevant sections like "nutrition".

### The Goal

A smart search engine that facilitates finding semantically similar terms and reduces search time instead of guessing terms for CTRL+F

### The Team

Without the help of my genious friends and lots of free time this idea would have not been possible

*   Joanna Kaczanowska: Problem

*   Christoph Götz: Conception, data and model

*   James Dommisse: AWS EC2 backend and [Flask frontend magic](https://flask.palletsprojects.com/en/1.1.x/)

*   Johannes Schuh: Search visualization Javascript magic

### The Result

*   Used [Scrapy](https://scrapy.org/) to download 100k+ scientific papers from Pubmed et al

*   Vectorized the topics using [Gensim](https://radimrehurek.com/gensim/) (word2vec)

*   Website to copy text to form, search field for string. Will automatically calculate semantic distance to searchterm and highligh semantically similar terms

### Lessons Learned

Thinking of words in terms of vectors and semantic meaning as distance between vectors was a fun excersise. Meaning of scientific fields are formed by \*bubbles \*of words  that partially overlap with other fields (think *fat* used in nutrition, detergents and organic chemistry in very different contexts). New evolving fields are budding off existing bubbles until they come completely distinct from its original semantic home. This process of knowledge creation was fascinating but - as always - not really novel and just the beginning:

While researching this topic I talked to researchers in the quantum physics group of Zeilinger. [Markus Krenn](https://scholar.google.at/citations?user=jzG7GC8AAAAJ\&hl=en) worked on an even cooler project namely predicting future research trends in a pretty similar manner. [His work was finally published in PNAS](https://www.pnas.org/content/117/4/1910.short) in 2020.

> Using network theoretical tools, we can suggest personalized, out-of-the-box ideas by identifying pairs of concepts, which have unique and extremal semantic network properties.

Thats such a cool concept! Predicting your future ideas based on the knowledge that is already somewhere around you. This substantiates the fact, that most big discoveries are often discovered by multiple people simulataneously (e.g. Evolution or Mendeleian inheritance). If the basic knowledge is available and people spend enough time and energy on connecting the dots, the dots will be connected.

What started out as a simple tool for vectorizing words ended up in learning about fundamental vectors in culturual evolution. You never know :D
