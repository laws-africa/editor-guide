# Marking up the structure

After working through this section, you should be able to:

* Mark up the top-level structure of a document
* Mark up the hierarchical structure of a document
* Mark up numbered elements
* Mark up nested elements.

## Introduction <a href="#introduction" id="introduction"></a>

The parser relies on indentation to group content and reflect the hierarchical structure of a document.

Keywords introduce a group, and everything that falls into that group is indented below the keyword.

## Top-level structure <a href="#top-level-structure" id="top-level-structure"></a>

At the highest level, a document is broken up into the following blocks:

* `PREFACE`
* `PREAMBLE`
* `BODY`
* `SCHEDULE(s)`

If there is no Preface or Preamble, `BODY` will be assumed until a [Schedule-like block](keyword-reference.md#schedule-like-blocks), after which everything will be in the Schedules.

### Example

```
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

## Hierarchical structure

Within the main body and in Schedules, content is usually grouped under headings.

In legislation, the most common groupings are Chapters, Parts, and Subparts.

Under these (or ungrouped), usually in this order, are sections, subsections, paragraphs, and subparagraphs. Articles are also sometimes used.

All of the above are hierarchical elements, and they all follow the same pattern.

The pattern for hierarchical elements is as follows:

* On a new line, the keyword, e.g. `CHAP` for a Chapter
* On the same line, optionally, a space and a number
* On the same line, optionally, `-` and a heading
* On the next line, optionally, an indent and `SUBHEADING`, followed by a space and the subheading
* Below the main heading, indented, the content of the grouping
* To mark the end of a grouping, unindent the next element or line.

### Tips

* If there is a number and no heading, you don't need to use a `-` .
* If there is no number but there is a heading, you do need to use a `-` to indicate the start of the heading.
* If there is a number and a heading, the `-` should come between the number and the heading.

See the examples below for an illustration, paying close attention to the placement of the `-` .

### Examples

#### Number and no heading

```
CHAP 1

  Content of this Chapter (can be Parts, sections, paragraphs, normal text, etc).
    
```

#### No number, heading

```
SUBPART - Financial reporting

  Content of the (unnumbered) 'Financial reporting' Subpart.
    
```

#### Number and heading

```
PART A - Financial reporting

  Content of Part A.
    
```

#### Subheading

```
PART A - Financial reporting
  SUBHEADING How to do it right
    
  Content of Division A.
    
```

#### More examples

```
CHAP 1 - Title
  SUBHEADING Some more detail
    
  SEC 2. - Heading

    Content of section 2, which falls inside Chapter 1.

  This text will fall inside Chapter 1, but not inside section 2.
        
This text won't fall inside Chapter 1.

SUBPART - Heading with no number

  Content of this (unnumbered) Subpart. Note the dash though.

CHAP 2

  Content of Chapter 2, which doesn't have a heading (or a dash).

```

{% hint style="warning" %}
If the content isn't indented, it won't be captured correctly and the keyword will be captured as text.
{% endhint %}

## Nested elements <a href="#nested-elements" id="nested-elements"></a>

To show that one element falls inside another element in the document hierarchy, indent the whole element.

If the parent element has content of its own, the indented element will line up with that content.

### Example <a href="#example-1" id="example-1"></a>

```
CHAP

  Text in Chapter.

  SEC 1

    SUBSEC (1)
    
      Content of first subsection:
      
      PARA a)
      
        Content of paragraph a:
        
        SUBPARA [i]
        
          Content of subparagraph i;
          
        SUBPARA [ii]
        
          Content of subparagraph ii; and
          
      PARA b)
      
        Content of paragraph b.
        
    SUBSEC (2)
    
      Content of second subsection.
      
  SUBPART A
  
    SEC 2
    
      Content of section 2, which is in Subpart A of the (unnumbered) Chapter.
      
    Free-floating content in Subpart A of the Chapter.
    
This text won't fall inside the Chapter.

```

{% hint style="info" %}
Nesting can get complicated! Look at the table of contents to help guide you, or collapse an element to hide its content.
{% endhint %}

{% hint style="info" %}
Note that the numbers of the elements above don't rules about needing a stop, round brackets, etc: anything given after the keyword and before `-` will be accepted as the number of that element.
{% endhint %}

## Bulleted lists

The pattern for bulleted lists is as follows:

* On a new line, the keyword `BULLETS`&#x20;
* Below the keyword, indented, `*` followed by the content of each bullet
* To mark the end of the bulleted list, unindent the next element.

{% hint style="info" %}
If a bullet has more than one paragraph, maintain the indentation so the text lines up, otherwise a `*` will automatically be added at the start of the next line.
{% endhint %}

### Example

```
      SUBPARA (xxiii)

        Relevant elements of existing instruments and processes, including:

        BULLETS
          * Convention on Biological Diversity;
          * Bonn Guidelines on Access to Genetic Resources and the Fair and Equitable Sharing of Benefits Arising from their Utilization;
            Second line of this bullet;
          * Third bullet.
        
        This text will go back into subparagraph (xxiii).
```

### Nested bullets

```
PARA 1.

  //Decides// to amend Annex II to the Basel Convention on the Control of Transboundary Movements of Hazardous Wastes and Their Disposal by adding the following entry:

  TABLE
    TR
      TC

      TC
        Plastic waste with the exception of the following:

        BULLETS
          * Plastic waste that is hazardous waste
          * Plastic waste listed below:

            BULLETS
              * Plastic waste …, including but not limited to the following polymers:

                BULLETS
                  * Polyethylene (PE)
                  * Polypropylene (PP)

              * Plastic waste …, including but not limited to the following resins:

                BULLETS
                  * Urea formaldehyde resins
                  * Phenol formaldehyde resins

              * Plastic waste … one of the following fluorinated polymers:

                BULLETS
                  * Perfluoroethylene/propylene (FEP)
                  * Perfluoroalkoxy alkanes:

                    BULLETS
                      * Tetrafluoroethylene/perfluoroalkyl vinyl ether (PFA)
                      * Tetrafluoroethylene/perfluoromethyl vinyl ether (MFA)

                  * Polyvinylfluoride (PVF)
                  * Polyvinylidenefluoride (PVDF)

          * Mixtures of plastic waste.



```

## Numbered lists

{% hint style="warning" %}
Do not use this markup for numbered elements like paragraphs or subparagraphs. Only use it for numbered lists in defined terms, the Preface, or tables.
{% endhint %}

The pattern for numbered lists is as follows:

* On a new line, the keyword `ITEMS`&#x20;
* Below the keyword, indented, the keyword `ITEM`&#x20;
* Below the second keyword, indented, the content of the item
* To mark the end of the numbered list, unindent the next element.

### Examples

#### Definitions

```
SEC 1. - Definitions

  Unless stated otherwise in this Act:
  
  "bread" means one loaf of bread;

  ITEMS
    "pigeon" means:
    
    ITEM (a)
      a city pigeon; or

    ITEM (b)
      a country pigeon,

    but not a pigeon that has been bred in captivity;
    
  "another term" means something else.


```

#### Preface

```
PREFACE

  Some introductory text:

  ITEMS
    ITEM a
      First numbered item,

      Second paragraph of first item;

    ITEM b.
      Second numbered item.

  This text will be in the preface, but no longer part of the list.


```

### Nested items

Repeat the pattern, with the nested `ITEMS` keyword inside the `ITEM` in which it appears.

```
ITEMS
  "possessions"—

  ITEM (a)
    means property of any kind, nature or description, whether movable or immovable; and

  ITEM (b)
    ITEMS
      includes —

      ITEM (i)
        any cash in a bank account or bank deposit; and

      ITEM (ii)
        any currency, whether or not the currency is legal tender …,
        
      but does not include …, [applies to list in item (b) only]
      
  and "possession" is the singular of "possessions"; [applies to outer list]


```

## Exercises

### Hierarchical structure 1

Copy the text below and paste it into a practise document, then see the instructions that follow.

```
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

![](<../.gitbook/assets/image (103).png>)

and like this in Edit mode:

![](<../.gitbook/assets/image (119).png>)

### Hierarchical structure 2

Copy the text below and paste it into a practise document, then see the instructions that follow.

```
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

1. Mark up the two Big headings with `DIVISION`, and the others with `SUBDIVISION`. You can use `CHAP` and `PART` if you prefer.
2. Nest the two Medium headings under the first Big heading.
3. Nest the Small heading under the first Medium heading.

When you're done, it should look like this in View mode:

![](<../.gitbook/assets/image (109).png>)

and like this in Edit mode:

![](<../.gitbook/assets/image (104).png>)

Note the indentation in the Table of Contents:

![](<../.gitbook/assets/image (111).png>)
