---
title: Activity
nav: true
---

---

# Text Analysis Activity

{% capture text %}
- For exploration, hypothesis generation
    - Playing around with text (even if you don't know what you're doing) can be an effective way to gain a new perspective on the texts you study
- To expand the audience for under-recognized texts
{% endcapture %}
{% include card.md text=text header="Why digital text analysis?" %}

What questions do you want to answer by analyzing your text? 
Whether you have a specific hypothesis in mind or your work is more exploratory, analyzing the frequency of words in your text can be a good place to start. 
The results may confirm your suspicions or yield surprising outputs that lead to further research.

---

## Word Frequency

- **Raw frequency**
    - The number of times a word appears in a text
- **Relative frequency**
    - The number of times a word appears in a text, relative to the size of that text. 
- **Example:** The word "love" might appear 200 times in a 100,000-word book and 200 times in a 50,000-word book. 
The word has the same raw frequency in both books, but the 50,000-word book has a higher relative frequency of the word "love" because there are a fewer number of words in the book.

We can visualize word frequency using [Voyant Tools](https://voyant-tools.org/){:target='_blank' rel='noopener'}. 
Voyant Tools is a modular online tool set for visualizing one or many documents.

---

## Basics of Voyant

- Variety of tools for reading, finding, analyzing and visualizing digital texts
- No installation or login are required, and you can work with texts in a wide variety of formats (plain text, PDF, XML, MS Word, RTF, etc.)
- Best to think of as "exploratory," just one piece of a larger research process and a way to spark questions

{% capture text %}
### Activity: Word Frequency in Thoreau's *Walden*

1. Go to [Voyant Tools](https://voyant-tools.org/){:target='_blank' rel='noopener'}
2. Copy and paste the <a href="https://owikle.github.io/dh-intro/data/walden.txt">text of *Walden*</a>{:target='_blank' rel='noopener'} into the text box on the Voyant Tools home screen
3. After uploading your text, you should see a screen with three tool panels along the top and two tool panels along the bottom:

{% include figure.html img="voyant-interface.jpg" alt="voyant interface" width="75%" %}

"Summary" at the bottom-left and "Cirrus" at the top-left give us the top five most frequent words in the text:

{% include figure.html img="summary.jpg" alt="voyant summary" width="75%" %}

{% include figure.html img="cirrus.jpg" alt="voyant cirrus" width="75%" %}

"Trends" at the top-right allows us to view the relative frequency of the top words in this text as they appear throughout the text. 
Voyant has separated the text into ten equal segments for this visualization.

{% include figure.html img="trends.jpg" alt="voyant trends" width="75%" %}
{% endcapture %}
{% include alert.md text=text color=secondary %}

---

**Tool Interactions**

An essential part of Voyant is that events in one tool can cause changes in other tools (the exact interactions depend on a number of factors, including which tools are visible).

---

**Stopword List**

A stopword is a word (usually a commonly-used word) that an application has been programmed to ignore. 
Usually, stopword lists contain common words such as a, an, the, and, to, from, etc. 

Sometimes, it can be useful to add common words like person names or place names, depending on what your research question is. 
Stopword lists are customizable, allowing the researcher to remove words such as character or place names from the analysis. 

Voyant automatically analyzes your text using a stop word list, but you can delete or edit this list as you see fit.

---

**Stopwords Make a Difference**

Compare the following two screenshots. 
The first uses Voyant's *Auto-detect* stopword setting. 
In this case, it has recognized this text as English, so it is using a standard English stopword list. 
The second uses Voyant's *None* stopword setting.

{% include figure.html img="walden-stoplist.jpg" alt="walden with stoplist" caption="Voyant's Cirrus visualization of Walden with an English stopword list" width="75%" %}

{% include figure.html img="walden-nostoplist.jpg" alt="walden without stoplist" caption="Voyant's Cirrus visualization of Walden without a stopword list" width="75%" %}

If you have your own stopword list, you can upload it instead. 
Or you can simply add words to Voyant's ready-made lists. 
To add or edit stopwords, click on the `options` icon in the top right of the visualization. 
This will produce a dialog box where you can select a list or edit it. 

<div class="text-center">{% include figure.html img="voyant-options.jpg" alt="voyant options tab" caption="Click on the 'options' tab (upper right)" width="75%" %}</div>

{% include figure.html img="stoplist.jpg" alt="voyant stoplist dropdown" caption="Voyant's stoplist options" width="75%" %}

---

**Contexts**

Word counts give us some information about a text, but often we need more context to make sense of how those words are being used. 
The Voyant "contexts" tool shows each occurrence of a word with its surrounding text. 
The tool lets you choose from the text's most frequent words, or you can type a word of your choice into the search box in the lower left-hand corner of the panel. 
Move the "context" slider next to the search box to view more words before and after your search term.

{% include figure.html img="contexts.jpg" alt="voyant-contexts" caption="A search for the contexts of 'heard' in Walden" width="75%" %}

To see how many times words appear in close proximity to each other, you can also view the "Links" feature in the top left-hand panel of the homepage (the same panel where you see "Cirrus"). 

---

**Other Voyant Tools**

Voyant has a robust [documentation](http://docs.voyant-tools.org/tools/){:target='_blank' rel='noopener'}. 
In it, you'll find a lot of tools listed that don't appear on the landing page. 
You can access these tools by hovering your cursor over the grid icon in the upper right-hand corner of each tool box.

---

{% capture text %}
**Exploration Time**

Let's explore a larger set of texts. Using a text corpus of your choice, spend some time exploring various Voyant tools. 

Sample Corpora:
- Your own writing
- The Austen or Shakespeare corpora that Voyant provides
- [Abraham Lincoln State of the Union Addresses]({ '/data/lincoln-addresses.zip' | relative_url })
- [Barack Obama State of the Union Addresses]({ '/data/obama-addresses.zip' | relative_url })
{% endcapture %}
{% include alert.md text=text color=secondary %}

{% capture text %}
**Reflection Time** 
- What insights, if any, do these tools provide?
- Are there patterns or in/consistencies?
    - Do you trust these patterns? Could you verify their accuracy somehow?
- How might your 'read' groups of words?
- What keywords or patterns did you pursue and why?
- What are the values/limitations of 'not reading' this way?
{% endcapture %}
{% include alert.md text=text color=secondary %}

---