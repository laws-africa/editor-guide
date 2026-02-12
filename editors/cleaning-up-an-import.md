# Cleaning up an import

Once you have imported a piece of legislation, it needs to be cleaned up before we publish it.

{% hint style="info" %}
Content and structure is more important than matching exactly what the text looks like in the gazette (presentation).
{% endhint %}

{% content-ref url="../how-tos/documents-and-document-settings/importing-a-document/the-importer.md" %}
[the-importer.md](../how-tos/documents-and-document-settings/importing-a-document/the-importer.md)
{% endcontent-ref %}

{% content-ref url="/broken/pages/-MA7AZ2T7nt0K9rLHnsS" %}
[Broken link](/broken/pages/-MA7AZ2T7nt0K9rLHnsS)
{% endcontent-ref %}

{% hint style="info" %}
Always prefer comparing against the original publication document; only compare against the imported docx when there isn't an original PDF to check against.
{% endhint %}

1. In the imported document, click **Show source** to see the imported file or publication document on the right-hand side of the screen.&#x20;
2. Remove superfluous text: The title, number, year, place, date, etc should all have been captured as metadata already and should show on the automatically generated coverpage (the top of the document in View mode). So those can come out, as well as the Table of Contents, which we also generate automatically (on the left-hand side). Click **Save draft** once this is done.
3. Check the structure: Does the automatically generated Table of Contents reflect all the Chapter / Part / Section headings and numbers that are in the pdf? (Crossheadings are not reflected in the Table of Contents, and should never be used for hierarchical elements.)
   * If there are any differences, investigate and resolve them before doing anything else.
   * Click **Save draft** once this is done.
4. Back to the top: Use the [Preface, Long title and Preamble](../markup-guide/preface-and-preamble.md) keywords as necessary. **Save draft**.
5. Run 'Analysis | References' and 'Analysis | Italicised terms'. This will automatically link references and italicise certain non-English terms. **Save draft**.
6. In general:
   * _Do_ correct OCR (e.g. 0 instead of O) and whitespace (e.g. TheBoard instead of The Board) errors.
   * _Don't_ correct spelling, grammar, punctuation, numbering, or cross-references; rather leave a comment on the document starting with 'note:', e.g. 'note: numbering as in original'. (There's no need to actively look for these types of errors, but it's fine for you to note them when you do notice them.)
   * If text was incorrectly linked or italicised automatically earlier, remove it manually. See [Working with links](../how-tos/mark-up/work-with-links.md) and [Working with italicised terms](../how-tos/mark-up/italicised-terms.md).
   * Save often :)
7. Structure:
   * See [Marking up the structure](../markup-guide/marking-up-the-structure.md).
   * For definitions that contain lists, use the [Numbered lists](../markup-guide/marking-up-the-structure.md#definitions) markup.
   * Make all headings [Sentence case](../style-guides/laws.africa.md#headings): only the first letter of the heading as well as any proper nouns or defined terms should be capitalised.
8. Sections:
   * Check the first and last words of paragraphs against the PDF.
   * Check line breaks: should two paragraphs be joined together, or one paragraph be split into two?
   * Check indents, especially of dangling text after the end of a list of paragraphs.
   * Briefly scan the text for OCR errors – but no need to check word for word.
     * If you notice multiple OCR errors in one document, pause what you're doing and alert the team. The document may need to be re-converted — maybe a whole batch of them!
9. You may also need to insert a [table](../how-tos/mark-up/tables/), insert an [image](../how-tos/document-elements/images.md), or work with [Schedules](../markup-guide/marking-up-schedules-annexes.md).
10. Before submitting the task for review:&#x20;
    * [Resolve all editor warnings](editor-warnings.md).
    * Check the [Reviewer checklist](reviewer-checklist.md).
    * Run 'Analysis | Defined terms'.
    * **Save draft.**
    * Return to the Task page by clicking on "Tasks" which is on the top right of the ribbon at the top of the page.
11. Submitting the task for review:
    * &#x20;On the tasks page there is an "Add a comment" button if you need to alert the reviewer of anything before submitting for review.
    * **Submit for review**.
