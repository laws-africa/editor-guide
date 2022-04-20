# Cleaning up an import

Once you have imported a piece of legislation, it needs to be cleaned up before we publish it.

{% hint style="info" %}
Content and structure is more important than matching exactly what the text looks like in the gazette (presentation).
{% endhint %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

1. In the imported document, click **Show source** to see the pdf (if available) on the right-hand side of the screen.
2. Remove superfluous text: The title, number, year, place, date, etc should all have been captured as metadata already and should show on the automatically generated coverpage (the top of the document in View mode). So those can come out, as well as the Table of Contents, which we also generate automatically (on the left-hand side). Click **Save draft** once this is done.
3. Check the structure: Does the automatically generated Table of Contents reflect all the Chapter / Part / Section headings and numbers that are in the pdf? (Crossheadings are not reflected in the Table of Contents.)
   * If there are any differences, investigate and resolve them before doing anything else.
   * Click **Save draft** once this is done.
4. Back to the top: Use the [Preface, Long title and Preamble](../markup-guide/preface-and-preamble.md) keywords as necessary. **Save draft**.
5. Run 'Analysis | References' and 'Analysis | Italicised terms'. This will automatically link references and italicise certain non-English terms. **Save draft**.
6. In general:
   * _Do_ correct OCR (e.g. 0 instead of O) and whitespace (e.g. TheBoard instead of The Board) errors.
   * _Don't_ correct spelling, grammar, punctuation, numbering, or cross-references; rather leave a comment starting with 'note:', e.g. 'note: numbering as in original'. (There's no need to actively look for these types of errors, but it's fine for you to note them when you do notice them.)
   * If text was incorrectly linked or italicised automatically earlier, remove it manually. See [Working with links](work-with-links.md) and [Working with italicised terms](italicised-terms.md).
   * Save often :)
7. Structure:
   * See [Marking up the structure](../markup-guide/marking-up-the-structure.md).
   * Make all headings [Sentence case](../style-guides/laws.africa.md#headings): only the first letter of the heading as well as any proper nouns or defined terms should be capitalised.
8. Sections:
   * Check the first and last words of paragraphs against the PDF.
   * Check line breaks: should two paragraphs be joined together, or one paragraph be split into two?
   * Check indents, especially of dangling text after the end of a list of paragraphs.
   * Briefly scan the text for OCR errors – but no need to check word for word.
9. You may also need to insert a [table](tables.md), insert an [image](images.md), or work with [Schedules](../markup-guide/marking-up-schedules-annexes.md).
10. Before submitting the task for review:&#x20;
    * [Resolve all editor warnings](editor-warnings.md).
    * Check the [Reviewer checklist](../reviewing-a-document/reviewer-checklist.md).
    * Run 'Analysis | Defined terms'.
    * **Save draft.**
    * Return to the Task page by clicking on "Tasks" which is on the top right of the ribbon at the top of the page.
11. Submitting the task for review:
    * &#x20;On the tasks page there is an "Add a comment" button if you need to alert the reviewer of anything before submitting for review.
    * **Submit for review**.
