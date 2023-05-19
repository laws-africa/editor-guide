---
description: This page describes how the importer is expected to work.
---

# The importer

If it’s _not_ doing some of the things described in this document, it’s a **bug** and we need to know about it.

If it _should_ be doing anything that’s not described in this document, it’s a missing **feature** and we also need to know about it.

## Main elements

These should all be recognised:

* Chapter
* Part
* Subpart
* Article
* Section
* Subsection
* Paragraph
* Subparagraph
* Items
  * These should only be in the definitions sections
  * There should be no paragraphs or subparagraphs in the definitions section
* Annexure, Appendix, Attachment, Schedule

### For all recognised elements

The following should be picked up:

* Keyword (e.g. CHAP, PART, SEC)
* Number
* Heading

{% hint style="info" %}
There should be a ‘ - ’ between the number and the heading.
{% endhint %}

### For Annexures, Appendixes, Attachments, and Schedules

* There should be no dash before the heading.
* The subheading should be picked up as well.

## Indentation

### Indentation of elements

The importer will do its best to place e.g. Parts inside Chapters, sections inside Parts, subsections inside sections, etc.

It won’t always get the top level 100% right, especially where:

* The Table of Contents / Arrangement of Sections wasn’t removed from the Word document before import
* There are variations in the internal structure, e.g. the first Chapter contains Parts but the next one doesn’t (that should actually be fine but something like that)

So the top-level structure should still always be checked first.

### Indentation within elements

```
Some intro text:
(a)	first para; and
(b)	second para,
except something that applies to both previous paragraphs.
```

In cases like this, the importer will do its best to unindent that last piece of text to the correct level — within the containing element if there is one, but not within the final (sub)element.

However, human intervention will always be required here as simply looking at the shape without reading the words or understanding the context will never be enough to tell the importer where that text should go.

Editors should check for:

* False positives: where the importer has unindented text that should actually be part of the final element. Sometimes an element legitimately contains two or more paragraphs of text, like in places where provisos always go on the next line.
* Missed matches: where the importer has failed to unindent the final element, or has put it in the next element or as a standalone paragraph. This is especially common in the definitions section, where the ‘exception’ text should be indented under ‘ITEMS’ but not under the final ‘ITEM’.

## Other elements

### Annotations

When a standalone paragraph begins with a \[ and ends with a ], the importer will automatically apply the annotation mark-up.

### Tables

Tables should import cleanly, including ‘colspan’s and ‘rowspan’s (where cells are merged horizontally or vertically).

### Arrangement of Sections / Table of Contents

The importer does not try to remove this. It’s risky to remove text from a document without any human oversight, so the best would be for these to be removed manually from Word documents before they’re imported.

### Preface and Preamble

The importer assumes that the Body of the document starts at the first element — be it a Chapter, Part, section, paragraph, etc. If it has a keyword (with rare exceptions, which the importer ignores), it’s in the body.

The importer then looks for the word ‘Preamble’ in the pre-body text of the document, and puts everything from ‘Preamble’ onwards and before the body into the Preamble. This currently only works on English documents.

Then, whether or not it found a Preamble, it puts everything before the body into the Preface.

You’ll notice that in documents where the Arrangement of Sections / Table of Contents hasn’t been removed, everything before that goes into a Preface and then the AoS starts in the BODY: That’s because it thinks that the first item in the AoS is a numbered paragraph, and those don’t go into the Preface.
