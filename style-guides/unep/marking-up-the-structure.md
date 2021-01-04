# Marking up the structure

After working through this section, you should be able to:

* Mark up the top-level structure of a document
* Mark up the hierarchical structure of a document
* Mark up numbered elements
* Mark up nested elements.

## Introduction <a id="introduction"></a>

The parser relies on indentation to group content and reflect the hierarchical structure of a document.

Keywords introduce a group, and everything that falls into that group is indented below the keyword.

## Top-level structure <a id="numbered-elements"></a>

At the highest level, a document is broken up into the following blocks:

* `PREFACE`
* `PREAMBLE`
* `BODY`
* `SCHEDULE(s)`

{% hint style="info" %}
In UN documents, we use `PREAMBLE` for text like   
'_The Conference of the Parties,  
Recognizing X,  
Appreciative of Y, etc_'  
before the first paragraph or heading \(see below for an exception\).

We haven't yet found a use for `PREFACE`.

See [https://edit.laws.africa/documents/4863/](https://edit.laws.africa/documents/4863/) for an example of a body that doesn't start at a heading or numbered paragraph.
{% endhint %}

If there is no Preface or Preamble, `BODY` will be assumed until a [Schedule-like block](keyword-reference.md#schedule-like-blocks), after which everything will be in the Schedules.

### Example

```text
PREFACE

    Content of preface.
    
PREAMBLE

    Content of preamble.

BODY

Content of body.

SCHEDULE

    Content of Schedule.

```

{% hint style="info" %}
The content of `BODY` doesn't need to be indented under it, because it's the main block.
{% endhint %}

## Hierarchical structure <a id="numbered-elements"></a>

Within the main body and in Schedules, content is often grouped under headings.

In legislation, the most common groupings are Chapters and Parts. For UN documents, which often don't specify what these headings are called, we use Divisions and Subdivisions.

The pattern for hierarchical elements is as follows:

* On a new line, the keyword, e.g. `DIVISION` for a division
* On the same line, optionally, a space and a number
* On the same line, optionally,  `-`  and a heading
* On the next line, optionally, an indent and `SUBHEADING`, followed by a space and the subheading
* Below the main heading, indented, the content of the grouping
* To mark the end of the grouping, unindent the next element.

### Tips

* If there is a number and no heading, you don't need to use a  `-` .
* If there is no number but there is a heading, you need to use a  `-`  to indicate the start of the heading.
* If there is a number and a heading, the  `-`  should come between the number and the heading.

See the examples below for an illustration, paying close attention to the placement of the  `-` .

### Examples

#### Number and no heading

```text
DIVISION A

    Content of this division (can be Subdivisions, paragraphs, normal text, etc).
    
```

#### No number, heading

```text
DIVISION - Financial reporting

    Content of the (unnumbered) 'Financial reporting' Division.
    
```

#### Number and heading

```text
DIVISION A - Financial reporting

    Content of Division A.
    
```

#### Subheading

```text
DIVISION A - Financial reporting
    SUBHEADING How to do it right
    
    Content of Division A.
    
```

#### More examples

```text
DIVISION 1 - Title
    SUBHEADING Some more detail
    
    PARA 2.
    
        Content of second paragraph, which falls inside Division 1.
        
    This text will fall inside Division 1, but not inside Paragraph 2.
        
This text won't fall inside Division 1.

DIVISION - Heading with no number

    Content of this (unnumbered) division. Note the dash though.
    
DIVISION 2

    Content of Division 2, which doesn't have a heading (or a dash).

```

{% hint style="warning" %}
If the content isn't indented, it won't be captured correctly and the keyword will be captured as text.
{% endhint %}

## Numbered elements <a id="numbered-elements"></a>

The most common grouping of content is numbered paragraphs.

The pattern for all numbered elements is as follows:

* On a new line, the keyword, e.g. `PARA` for paragraph
* On the same line, a space and number
* On the same line, optionally, after the number,  `-`  and a heading
* Below it, indented, the content of the element
* To mark the end of an element, unindent the text.

{% hint style="info" %}
Note the similarity to the markup for hierarchical elements.
{% endhint %}

### Example <a id="example"></a>

```text
PARA 1. - Heading

  Content of first paragraph.
  
This text won't fall inside Paragraph 1.
  
```

{% hint style="warning" %}
If the content of an element is not indented, it won't be captured correctly and the keyword will be captured as text.
{% endhint %}

## Nested elements <a id="nested-elements"></a>

To show that one element falls inside another element in the document hierarchy, indent the whole element.

If the parent element has content of its own, the indented element will line up with that content.

### Example <a id="example-1"></a>

```text
DIVISION

  Text in Division.

  PARA 1.
  
    Contents of first paragraph:
    
    SUBPARA a)
    
      contents of first subparagraph.
      
  SUBDIVISION A
  
    PARA 2.
    
      Contents of second paragraph, which is in Subdivision A of the Division.
      
    Free-floating content in Subdivision A of the Division.
    
This text won't fall inside the Division.

```

{% hint style="info" %}
Nesting can get complicated! Look at the sidebar Table of Contents to help guide you.
{% endhint %}

## Bulleted lists

To mark up a bulleted list, use the bullet as the 'number' of the element.

### Example

```text
      SUBPARA (xxiii)

        Relevant elements of existing instruments and processes, including:

        SUBPARA ▪

          Convention on Biological Diversity;

        SUBPARA ▪

          Bonn Guidelines on Access to Genetic Resources and the Fair and Equitable Sharing of Benefits Arising from their Utilization;
        
        etc.
```

See the [Keyword reference](keyword-reference.md#bullets) for a list of copy/pastable bullets.

## Exercises

### Numbered elements

Copy the text below and paste it into a practise document, then see the instructions that follow.

```text
PARA

1.

Content of first paragraph

2. PARA

List introduction:

SUBPARA a) content of subparagraph a;

SUBPARA b)

content of subparagraph b,

Wrap-up text.

PARA 3. Heading Content of third paragraph.


```

1. Correct the ordering of each numbered element: keyword, then number, then content indented below. Paragraph 3 has a heading.
2. Correct the indentation of each numbered element, paying close attention to nested elements.
3. Ensure the wrap-up text at the end of the second paragraph is indented correctly.

When you're done, it should look like this in View mode:

![](../../.gitbook/assets/image%20%28103%29.png)

and like this in Edit mode:

![](../../.gitbook/assets/image%20%28119%29.png)

### Hierarchical structure

Copy the text below and paste it into a practise document, then see the instructions that follow.

```text
Big heading

Medium heading

Content

Small heading

Content

Medium heading

Content

Big heading

Content

```

1. Mark up the two Big headings with `DIVISION`, and the others with `SUBDIVISION`.
2. Nest the two Medium headings under the first Big heading.
3. Nest the Small heading under the first Medium heading.

When you're done, it should look like this in View mode:

![](../../.gitbook/assets/image%20%28109%29.png)

and like this in Edit mode:

![](../../.gitbook/assets/image%20%28104%29.png)

Note the indentation in the Table of Contents:

![](../../.gitbook/assets/image%20%28111%29.png)

