# Marking up footnotes

After working through this section, you should be able to:

* Mark up a footnote reference
* Superscript a footnote reference
* Mark up a footnote's content
* Mark up nested elements inside a footnote
* Mark the end of a footnote.

## Marking up a footnote <a href="#marking-up-a-footnote" id="marking-up-a-footnote"></a>

The pattern for marking up footnotes is as follows:

* In the text where the footnote reference appears, the inline markup `{{FOOTNOTE x}}`, where `x` is the footnote reference marker
* On a new line, the `FOOTNOTE` keyword
* On the same line, a space and the footnote reference marker
* Below it, indented, the content of the footnote
* To mark the end of a footnote, unindent the text.

### Example

```
  PARA 1.

    Content of paragraph 1.{{FOOTNOTE 2}}

    FOOTNOTE 2

      Content of the footnote.

    Next paragraph in paragraph 1.

```

will look like this in View mode:

![](<../.gitbook/assets/image (43).png>)

{% hint style="info" %}
Note the indentation of the text after the end of the quote.
{% endhint %}

{% hint style="warning" %}
If the content of the footnote is not indented, it won't be captured correctly.
{% endhint %}

{% hint style="warning" %}
If the footnote reference marker doesn't match, it won't be captured correctly.
{% endhint %}

## Superscripting a footnote reference

As you will see in [Marking up formatting](marking-up-formatting.md), the way to superscript text is to wrap it in `{{^` and `}}`.

Thus, if your footnote reference reads `{{FOOTNOTE 2}}` as in the above example, and you want it to be superscripted, it should read `{{^{{FOOTNOTE 2}}}}`.

{% hint style="info" %}
Note the two sets of closing `}}`s, one for the superscript markup and one for the footnote reference markup.
{% endhint %}

### Example

```
  PARA 1.

    Content of paragraph 1.{{^{{FOOTNOTE 2}}}}

    FOOTNOTE 2

      Content of the footnote.

    Next paragraph in paragraph 1.

```

will look like this in View mode:

![](<../.gitbook/assets/image (247).png>)

## Marking up nested elements

To mark up nested elements inside a footnote, use the same principles as in [Marking up the structure](marking-up-the-structure.md): Indent the contents of each element under its own keyword, and indent all the elements in the footnote under the `FOOTNOTE` keyword.

### Example

```
  PARA 1.

    Content of paragraph 1.{{^{{FOOTNOTE 2}}}}

    FOOTNOTE 2

      Intro:

      PARA A.

        PARA (i) 
      
          content

        PARA (ii)

          content.

```

will look like this in View mode:

![](<../.gitbook/assets/image (219).png>)

## Exercise

Copy the text below and paste it into a practise document, then see the instructions that follow.

```
PARA 3.

    Content of third paragraph.2

    Content of footnote 2:

    PARA A.

    PARA (i) 
      
    subparagraph (i) inside footnote;

    PARA (ii)

    subparagraph (ii) inside footnote,
    
    Wrap-up text in paragraph A.
    
    Last line of footnote 2.
    
Back into third paragraph.

```

1. Mark up the footnote reference to footnote 2 on line 3.
2. Superscript the same footnote reference.
3. Mark up the footnote that starts on line 5.
4. Correct the indentation of the nested elements in the footnote.
5. Correct the indentation of the text after the end of the footnote.

When you're done, it should look like this in View mode:

![](<../.gitbook/assets/image (184).png>)

and like this in Edit mode:

![](<../.gitbook/assets/image (163).png>)
