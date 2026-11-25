# Marking up formatting

After working through this section, you should be able to:

* Mark up superscripts
* Mark up subscripts
* Mark up bold
* Mark up italics
* Choose text size and alignment using formatting classes.

## Marking up superscripts

The pattern for marking up superscripts is as follows:

* Before the superscripted text, the opening `{{^`
* The text to be superscripted
* The closing `}}`.

{% hint style="warning" %}
Spaces and any punctuation that are included between `{{^` and `}}` will also be superscripted.
{% endhint %}

### Example

```
On the 15{{^th}} of July 2020 …
```

will look like this in View mode:

![](<../.gitbook/assets/image (58).png>)

## Marking up subscripts <a href="#marking-up-subscripts" id="marking-up-subscripts"></a>

The pattern for marking up subscripts is as follows:

* Before the subscripted text, the opening `{{_`
* The text to be subscripted
* The closing `}}`.

{% hint style="warning" %}
Spaces and any punctuation that are included between `{{_` and `}}` will also be subscripted.
{% endhint %}

### Example

```
The amount of CO{{_2}} in the atmosphere …
```

will look like this in View mode:

![](<../.gitbook/assets/image (87).png>)

## Marking up bold text <a href="#marking-up-subscripts" id="marking-up-subscripts"></a>

The pattern for marking up bold text is as follows:

* Before the bold text, the opening `**`
* The text to be bolded
* The closing `**`.

{% hint style="warning" %}
Spaces and any punctuation that are included between the `**`s will also be bolded.
{% endhint %}

### Example

```
**This whole sentence is bold.**
```

will look like this in View mode:

![](<../.gitbook/assets/image (259).png>)

## Marking up italics text <a href="#marking-up-subscripts" id="marking-up-subscripts"></a>

The pattern for marking up italics text is as follows:

* Before the italics text, the opening `//`
* The text to be italicised
* The closing `//`.

{% hint style="warning" %}
Spaces and any punctuation that are included between the `//`s will also be italicised.
{% endhint %}

### Example

```
Just //this text// is in italics.
```

will look like this in View mode:

![](<../.gitbook/assets/image (196).png>)

## Text size and alignment classes

Formatting classes set the text size or alignment of a whole table, an individual cell or a paragraph. You can use the [table editor controls](../how-tos/mark-up/tables/README.md#how-to-edit-a-table) for tables and selected cells. There are no general paragraph size or alignment toolbar controls at present; existing paragraph classes are preserved when editing a table.

In markup, add a full stop and the class name immediately after a keyword. Separate multiple classes with full stops, without spaces. For example, `TABLE.akn--text-small.akn--text-justify` makes the table text Small and justified. See [Marking up tables](marking-up-tables.md#formatting-tables-and-cells) for a complete example.

### Text sizes

| Editor choice | Class | HTML display | PDF output |
| --- | --- | --- | --- |
| Default | No size class | Inherited or publication default | Inherited or publication default |
| Normal | `akn--text-normal` | 100% of normal document size | Normal document size |
| Small | `akn--text-small` | 80% of normal document size | 8 pt |
| Extra small | `akn--text-xsmall` | 70% of normal document size | 7 pt |
| Extra-extra small | `akn--text-xxsmall` | 60% of normal document size | 6 pt |

The normal document size depends on the publication. These classes work in both HTML and PDF, but the two formats use the size scales shown above. Check the PDF when preparing a document for print.

Sizes refer to the document's normal size. They do not shrink repeatedly when nested: a Small cell inside a Small table is still Small. Normal restores the normal document size, even when the surrounding table is Small.

### Text alignment

| Editor choice | Class | Effect |
| --- | --- | --- |
| Default | No alignment class | Follow the inherited or publication alignment |
| Left | `akn--text-left` | Align text to the left |
| Centre | `akn--text-center` | Centre text |
| Right | `akn--text-right` | Align text to the right |
| Justify | `akn--text-justify` | Align text with both sides of the text area |

Use only one size class and one alignment class on each element. A setting on a cell overrides the table's setting; a setting on a paragraph overrides the cell's setting. The table editor replaces conflicting classes from the same group while retaining unrelated classes.

### Cell spacing and borders

* `akn--no-padding` removes cell padding. Apply it to a table to remove padding from all its cells, or to `TH` or `TC` to affect an individual cell. It does not remove borders.
* `akn--no-border` removes borders from a whole table. Apply it to `TABLE`; individual-cell border controls are not supported. Dotted guides in the editor help you see the borderless cells while editing.

These explicit classes do not change the usual formatting of tables without classes. Publication-specific defaults, including those for the [Kenya Annual Supplement](../style-guides/kenya-annual-supplement.md), are documented separately.

## Exercise

Copy the text below and paste it into a practise document, then see the instructions that follow.

```
PARA 12.
  
    On the 12th of July 2020, the amount of CO2 in the atmosphere was bold.
    
    Later that same month is was italics.
    
```

1. Mark up the `th` in the 'the 12th of July' as superscripted.
2. Mark up the `2` in 'CO2' as subscripted.
3. Mark up the word `bold` as bold.
4. Mark up the word `italics` as italics.

When you're done, it should look like this in View mode:

![](<../.gitbook/assets/image (143).png>)

and like this in Edit mode:

![](<../.gitbook/assets/image (31).png>)
