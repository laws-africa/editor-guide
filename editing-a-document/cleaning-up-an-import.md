---
description: Fixing issues after an import.
---

# Cleaning up an import

Once you have imported a piece of legislation \(usually from a pdf of the gazette in which it was published\), it needs to be cleaned up before we publish it.

{% hint style="info" %}
Content and structure is more important than matching exactly what the text looks like in the gazette
{% endhint %}

1. In the imported document, click **Show source** to see the pdf \(if available\) on the right-hand side of the screen.
2. Check that all the relevant pages of the pdf were imported: Check the start and end of the imported text, and the start and end of the published legislation.
3. Remove superfluous text: The title, number, year, place, date, etc should all have been captured as metadata already and should show on the automatically generated coverpage \(the top of the document in View mode\). So those can come out, as well as the Table of Contents, which we also generate automatically \(on the left-hand side\).
4. Check the structure: Does the automatically generated Table of Contents reflect all the Chapter / Part / Section headings and numbers that are in the pdf?  If there are any differences, investigate and resolve them.
5. Back to the top: Use the [Preface, Long title and Preamble](preface-and-preamble.md) keywords as necessary.
6. Headings
   * Use the [Chapter and Part](chapters.md) keywords as necessary.
   * Make all headings [Sentence case](https://docs.laws.africa/style-guides/south-african-by-laws#what-is-sentence-case): only the first letter of the heading as well as any proper nouns or defined terms are capitalised.
   * Correct OCR \(e.g. 0 instead of O\) and whitespace \(e.g. TheBoard instead of The Board\) errors.
   * Do not correct spelling or grammar mistakes; rather leave a comment on the right-hand side.
   * Do not 'correct' the placement of section numbers if they appear on the next line in the pdf. We mark it up with the number next to the heading so that it is encoded in Akoma Ntoso as 'section number' and 'section title'. We are capturing the _structure_ here, and deal with the _presentation_ separately.
7. Check the text section by section:
   * Check the first and last words of paragraphs against the pdf.
   * Check line breaks: should two paragraphs be joined together, or one paragraph be split into two?
   * Check [indents](indented-lists.md).
   * Briefly scan the text for OCR errors – but no need to check word for word.
   * _Do_ fix OCR errors and whitespace errors.
   * _Don't_ fix spelling, grammar, punctuation, numbering, or cross-references; rather leave a comment starting with 'note:', e.g. 'note: numbering as in original'. \(There's no need to actively look for these types of errors, but it's fine for you to note them if you do notice them.\)
8. You may also need to insert a [table](tables.md), insert an [image](images.md), or work with [Schedules](schedules.md).

