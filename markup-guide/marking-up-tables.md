# Marking up tables

After working through this section, you should be able to:

* Mark up a table
* Mark up heading and content cells
* Mark up quoted content in a table cell
* Merge cells horizontally and vertically
* Mark the end of a table.

## Marking up a table <a href="#marking-up-a-footnote" id="marking-up-a-footnote"></a>

The pattern for tables is as follows:

* On a new line, the `TABLE` keyword
* Below it, indented, the `TR` (table row) keyword
* Below it, indented, either the `TH` (table heading) or `TC` (table content) keyword for each cell in the row
* Below each of those, indented, the content of the cell
* To mark the end of a table, unindent the text.

### Example

```
TABLE
    TR
        TH
            Heading 1
        TH
            Heading 2
    TR
        TC
            Content 1
        TC
            Content 2
            
Regular old text.
            
```

will look like this in View mode:

![](<../.gitbook/assets/image (203).png>)

## Marking up quoted content

The pattern for quoted content is as follows:

* On a new line inside a `TH` or `TC` block, the `QUOTE` keyword
* Optionally, `{startQuote “}` immediately after (no space after the keyword)
* Below it, indented, the keyword of the quoted element
* Below that, indented, the content of the quoted element
* To mark the end of the quote, unindent the text.

{% hint style="info" %}
The above is the same logic as for [Marking up the structure](marking-up-the-structure.md), with the addition of the `QUOTE` keyword being the only difference.
{% endhint %}

### Example

```
TABLE
    TR
        TH
            Heading 1

        TH
            Heading 2

    TR
        TC
        
            Something about section 21:

            QUOTE{startQuote “}

                SEC 21 - Head

                    Content of section 21—
                    
                    PARA (a)
                    
                        first paragraph:
                        
                        SUBPARA (i)
                        
                            first subparagraph;
                    
                        SUBPARA (ii)
                        
                            second subparagraph;
                    
                    PARA (b)
                    
                        second paragraph,
                        
                    wrap-up text of section 21.”
                    
            Some more text talking about section 21.


        TC
            Content 2

```

will look like this in View mode:

![](<../.gitbook/assets/image (195).png>)

## Merging cells horizontally

To merge cells horizontally, we use the `colspan` keyword, as follows:

* Immediately after either `TH` or `TC` (no space), `{colspan`&#x20;
* &#x20;The total number of cells to merge horizontally, e.g. `3`
* &#x20;The closing `}`.

### Example

```
TABLE

    TR
        TH{colspan 2}
            Spans both columns
            
    TR
        TC
            First cell's content
        
        TC
            Second cell's content
```

will look like this in View mode:

![](<../.gitbook/assets/image (162).png>)

{% hint style="info" %}
Note how the first row in Edit mode only has one `TH`.
{% endhint %}

## Merging cells vertically

To merge cells vertically, we use the `rowspan` keyword, as follows:

* Immediately after either `TH` or `TC` (no space), `{rowspan`&#x20;
* &#x20;The total number of cells to merge vertically, e.g. `3`
* &#x20;The closing `}`.

### Example

```
TABLE
    TR
        TH
            Heading 1
        TH
            Heading 2
    TR
        TC{rowspan 2}
            Rows 1 and 2, Column 1
        TC
            Row 1, Column 2
    TR
        TC
            Row 2, Column 2
    TR
        TC
            Row 3, Column 1
        TC
            Row 3, Column 2

```

will look like this in View mode:

![](<../.gitbook/assets/image (264).png>)

{% hint style="info" %}
Note how the third row in Edit mode only has one `TC`, which will be in the second column.

If `{rowspan 2}` had been applied to the second column in the second row instead, the third row's one `TC` would be in the first column in View mode, but unchanged in Edit mode.
{% endhint %}

## Exercises

### Structuring a table

Copy the text below and paste it into a practise document, then see the instructions that follow.

```
Big Heading A

Heading 1, Heading 2, Heading 3

Subheading 1, Content 1, Content 2

Content 1, Content 2

```

1. Insert the `TABLE` keyword before row 1, and indent all the rows under it.
2. Insert the `TR` keyword before each row, and indent each row under it.
3. In the first row, insert the `TH` keyword before the Big Heading, have it span all three columns, and indent the text below it.
4. In the second row, insert the `TH` keyword before each Heading, and indent the text below it. You can delete the commas between the Headings.
5. In the third row, use `TH` for the Subheading, and have it span two rows.
6. Use `TC` for the remaining cells. You can delete the commas between them.

When you're done, it should look like this in View mode:

![](<../.gitbook/assets/image (269).png>)

and like this in Edit mode:

![](<../.gitbook/assets/image (70).png>)

### Quoted content

Copy the text below and paste it into a practise document, then see the instructions that follow.

```
TABLE
    TR
        TH{rowspan 2}
            Name of Act being amended

        TC
            Replace section 2 with the following:

            “2. New heading

            (1) New subsection 1.

            (2) New subsection 2.”.

    TR
        TC
            In section 3, replace paragraph (a) with the following:

            “(a) new text;”.

```

1. Insert `QUOTE{startQuote “}` before the start of both quotes (lines 9 and 19).
2. Indent each quote under its keyword.
3. Delete the repeated `“` at the start of each quote.
4. Model the first quote as section 2, including subsections (1) and (2), using the appropriate keywords and indentation.
5. Model the second quote as paragraph (a).

When you're done, it should look like this in View mode:

![](<../.gitbook/assets/image (53).png>)

and like this in Edit mode:

![](<../.gitbook/assets/image (209).png>)
