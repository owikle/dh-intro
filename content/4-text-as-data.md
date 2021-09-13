---
title: Text as Data
nav: true
---

# Text as Data

Breaking down a text into smaller units of analysis lets us see patterns and approach from different points of entry.

In text analysis (also referred to as text mining), units of analysis tend to be groupings of text (broken up as discrete books, documents, poems, etc.), and words. 
Much of the time spent doing text analysis research is spent preparing text so that these smaller units of analyses can be accessed by the digital tools we use.

## Defining Units of Analysis

{% include figure.html img="chapters.jpg" alt="open books" width="75%" %}

Usually when people analyze text, they are interested in words (i.e. word frequency, order, etc.). 

Therefore, a primary part of preparing your text for research is making sure the words in your corpus are identifiable units of measurement.

## Thinking of Text as a "Bag of Words"

{% capture text %}
- **Structured data**: Data with fixed fields (key/value pairs, relations)
    - Example: spreadsheet of names, phone numbers, dates, zip codes
- **Unstructured data**: No computer-readable structure or relationships between units of analysis
    - Example: un-coded text
{% endcapture %}
<div class="row justify-content-center">{% include card.md text=text header="Structured Data vs. Unstructured Data" %}</div>

In textual research in the digital humanities, usually we are working with unstructured data.

However, most textual content is locked in the printed page, so the first step is to extract the information from digitized images.

## OCR (Optical Character Recognition)

OCR identifies printed or handwritten text characters in digital images of physical documents. 
Once translated by the OCR software, the characters can be recognized as text by the computer, allowing a document's content to be processed and manipulated as data.

{% capture text %}
1. **Digitization** (make high quality scans)
2. **Image preprocessing** (deskew, scale remove borders, high-pass filter)
3. **Layout detection and segmentation** (identify organization and lines of text to pass to OCR)
4. **OCR** (feature extraction)
5. **Text post-processing** (adaptive recognition, lexicons, co-occurrence, noise reduction)

{% endcapture %}
<div class="row justify-content-center">{% include card.md text=text header="Traditional OCR Workflow" %}</div>

{% include figure.html img="ocr2.jpg" alt="ocr" caption="OCR of quality Tiff file" width="100%" %}

***Try it yourself***: [Tesseract](https://github.com/tesseract-ocr/) is an open-source OCR software. 
If you have access to the proprietary [Adobe Acrobat](https://acrobat.adobe.com/us/en/acrobat/how-to/ocr-software-convert-pdf-to-text.html) software, you can use it to extract text as well.

## Where to Find Texts

**Copyright**

Depending on what you're going to do with your texts, you'll need to pay attention to whether or not they are in the public domain. Texts that are no longer under copyright are usually easier to use for analytical research because they have a greater likelihood of already being digitized. 
(Of course, this also has the effect of skewing text research in DH so that it focuses more on older literary works.) 

A good resource to use if you're wondering whether something is under copyright is Cornell University Library's [Copyright Information Center](https://copyright.cornell.edu/publicdomain){:target='_blank'}. 
Currently, most works published before 1925 are in the public domain.

**Digitized Text**

- [Project Gutenberg](https://www.gutenberg.org/){:target='_blank' rel='noopener'}
    - Full text of thousands of free books. Text is usually fairly clean, but often little bibliographic information.
- [Archive.org](https://archive.org/){:target='_blank'}{:target='_blank' rel='noopener'}
    - Full texts and scans of books, lots of different download options from epub to pdf, to plain text.
- [HathiTrust](https://www.hathitrust.org/){:target='_blank'}{:target='_blank' rel='noopener'}
    - Millions of digitized books, public domain and copyrighted. Cleanliness of text varies. More advanced features require institutional membership.

## Text Cleaning

After you've OCRed your text and transferred it to plain text format, you will likely discover errors in your new text file(s). 
OCR is not perfect. 
Especially if you are using older texts, you might encounter problems such as your `s`'s looking like `f`'s:

{% include figure.html img="italian.jpg" alt="italian" caption="The Italian, Ann Radcliffe (1797)" width="100%" %}

{% include figure.html img="italian-text.jpg" alt="italian text" caption="Plain text, after OCR" width="100%" %}

## Getting to Know Your Corpus

{% include figure.html img="picture.jpg" alt="picture frames" width="50%" %}

Text analysis allows us to look at the big picture and explore broad patterns that span large bodies of text. 

*However, this doesn't absolve you from actually having to read some of the text you are analyzing.*

In order to understand the outputs from the algorithms you run on your text, and to be sure that the results you are getting are actually valid, you need to be somewhat familiar with the text you are analyzing.
