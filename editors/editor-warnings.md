# Resolving editor warnings

## Steps

1. Check the Table of Contents on the the left-hand side for warnings.
2. Go to the provision to see where exactly the warning is coming from.
3. Edit the provision to resolve the warning; the warning will no longer be there after you Update.
4. Don't forget to save! :)

## Tips

* _Do_ fix OCR errors and whitespace errors.
* _Don't_ fix spelling, grammar, punctuation, or numbering errors; rather [make a comment](../how-tos/document-elements/making-comments.md) or [insert an editorial note](../how-tos/document-elements/inserting-editorial-notes.md).

## Examples

### All-caps headings

![](<../.gitbook/assets/image (249).png>)

Solution: Make the heading/s [Sentence case](../style-guides/laws.africa.md#headings).

### Empty body

![](<../.gitbook/assets/image (101).png>)

Solution: Remove the 'Schedule' introduction (keyword, heading, and subheading), and make sure the body of the document starts after the `BODY` keyword.

### Empty section

![](<../.gitbook/assets/image (172).png>)

Potential solutions:

* Move the content of the section under the heading, if it's a section.
* Use the `PARA` keyword, if it's a numbered paragraph in a Schedule or Annexure.
* insert a `\` before the number so that it gets treated as normal text, if it's a numbered list in the main body.
* Delete the number and heading, if it's in the Arrangement of Sections from the original.

### Duplicate section numbers

![](<../.gitbook/assets/image (24).png>)

Solution: Check the section numbers in the original. If that's how they are, [insert an editorial note](../how-tos/document-elements/inserting-editorial-notes.md).

### Other duplicates

![](<../.gitbook/assets/image (277).png>)

Solution: Check the numbers in the original. If that's how they are, [insert an editorial note](../how-tos/document-elements/inserting-editorial-notes.md).

### Numbers don't follow

![](<../.gitbook/assets/image (118).png>)

Solution:&#x20;

* First check that the previous element wasn't sucked into the one before it (in this example, see if subsection (3) is at the end of subsection (2)).
* Check the numbers in the original. If that's how they are, [insert an editorial note](../how-tos/document-elements/inserting-editorial-notes.md).

### Only one element

![](<../.gitbook/assets/image (46).png>)

Solution:&#x20;

* First check that the subsequent element wasn't sucked into this one (in this example, see if subsection (2) is at the end of subsection (1)).
* Check the numbers in the original. If that's how they are, [make a comment](../how-tos/document-elements/making-comments.md) ('note: as in original').
  * This way, if someone else sees the document and the warning, they'll know you've already checked it.

### (l) or (I) instead of (1)

![](<../.gitbook/assets/image (239).png>)

Solution: These should usually be changed to (1). If in doubt, make a comment to ask for feedback from a reviewer.

### Broken word

![](<../.gitbook/assets/image (275).png>)

Solution: These should usually be joined into one word ('responsible' in this case). If in doubt, make a comment to ask for feedback from a reviewer.

### Space before punctuation

![](<../.gitbook/assets/image (81).png>)

Solution: Find and remove the space. (You may need to use the 'Search' function in Edit view to find it.)

If there should be a space before punctuation for some reason, [make a comment](../how-tos/document-elements/making-comments.md) explaining why it isn't an error.

### Space missing after punctuation

![](<../.gitbook/assets/image (98).png>)

Solution: Insert the missing space.

If there shouldn't be a space for some reason, [make a comment](../how-tos/document-elements/making-comments.md) explaining why it isn't an error.

### Broken link

![](<../.gitbook/assets/image (157).png>)

Solution: See [Working with links](../how-tos/mark-up/work-with-links.md).

### Image missing attachment

![](<../.gitbook/assets/image (37).png>)

Solution: Make sure the name for the file given in Edit view has a corresponding attachment on the document.

### m2

![](<../.gitbook/assets/image (129).png>)

Solution: Superscript the 2: `300m2` → `300m{{^2}}`, or make a comment if it shouldn't be superscripted.
