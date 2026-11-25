# Kenya Annual Supplement

This page describes the typography and form layout used in Kenya Law Annual Supplement PDFs. These are specific publication rules; they are not the defaults for every Indigo publication.

For the shared table editor controls and markup, see [Working with tables](../how-tos/mark-up/tables/README.md) and [Marking up tables](../markup-guide/marking-up-tables.md).

## Normal text and table sizes

Normal text is **10 pt in principal legislation** and **9 pt in subsidiary legislation**. This depends on whether the work is subsidiary legislation, rather than whether it is an amending work.

Table text inherits its size from the surrounding content unless a size is explicitly chosen. Ordinary table cells use justified text by default, including tables within forms. An explicit alignment on a table, cell or paragraph takes precedence.

| Editor choice | Class | Principal legislation | Subsidiary legislation |
| --- | --- | --- | --- |
| Default | No size class | Inherit the surrounding size | Inherit the surrounding size |
| Normal | `akn--text-normal` | 10 pt | 9 pt |
| Small | `akn--text-small` | 8 pt | 8 pt |
| Extra small | `akn--text-xsmall` | 7 pt | 7 pt |
| Extra-extra small | `akn--text-xxsmall` | 6 pt | 6 pt |

Use **Normal** to restore the normal document size inside smaller content. Use **Default** to follow the surrounding size. A cell or paragraph can override its table's size or alignment. Size reductions do not compound when the same class is repeated on nested content.

### Wide tables and older documents

Tables are no longer automatically reduced in size because they have more than five columns. Choose a size explicitly when a wide table needs smaller text, and check the resulting PDF for wrapping and page breaks.

Older automatically reduced tables have been given `akn--text-xsmall` to retain their intended size. The old `fontsize` attribute has also been replaced with supported size classes. Do not add `fontsize` in new markup; use the editor's size choices or the classes above.

The replacement of old size overrides used these rules:

| Old `fontsize` value | Principal legislation | Subsidiary legislation |
| --- | --- | --- |
| 6 | Extra-extra small | Extra-extra small |
| 9, 9.2 or 9.5 | Small | Normal |
| 10 | Normal | Normal |

The table editor may mention legacy PDF sizing used by other publications. In the updated Annual Supplement renderer, Default simply follows the surrounding size; it does not trigger shrinking based on the number of columns.

## Declaring a form

Add the class **`akn--form`** to the element that contains the form. This tells the Annual Supplement PDF to start the form at the normal left text edge and avoid ordinary first-line indentation in its unnumbered text. The renderer no longer guesses that content is a form from its internal structure.

Choose the wrapper that matches the content:

| Markup | Use it for |
| --- | --- |
| `TABLE.akn--form` | A form contained in a single table |
| `BLOCKS.akn--form` | A group of unnumbered paragraphs, tables or block lists |
| `SCHEDULE.akn--form` | A whole Schedule that is a form, including formal numbered paragraphs |

For a form in a table:

```
TABLE.akn--form.akn--no-border
    TR
        TC
            Name:
        TC
            ........................................
```

For a group of unnumbered paragraphs:

```
BLOCKS.akn--form
    Name: ........................................

    Address: .....................................
```

For a whole Schedule containing numbered paragraphs:

```
SCHEDULE.akn--form Schedule
    SUBHEADING Application form

    PARA 1.
        Name: ....................................

    PARA 2.
        Address: .................................
```

Keep numbered structure as numbered structure. `BLOCKS` is for block content and cannot contain formal `PARA` or `SECTION` hierarchy. Use a marked Schedule when the whole Schedule is a form containing that hierarchy; do not flatten numbered paragraphs to fit them into a `BLOCKS` wrapper. If only part of a Schedule is a form with formal numbered hierarchy that needs its own wrapper, ask for markup guidance rather than changing its structure.

The form class adjusts indentation only. It does not choose text size, alignment, padding or borders. Add those classes separately as needed. Numbered items and their continuation paragraphs retain their usual indentation, and long forms can continue over page breaks. Schedule headings and references retain their usual layout. Narrow tables keep their width but align with the form's left edge.

Review existing forms and add the class to the appropriate supported wrapper; they are not marked automatically. Check the exported PDF after changing form markup.
