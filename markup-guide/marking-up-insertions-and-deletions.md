---
description: >-
  Showing the changes that have been made when one principal work amends
  another.
---

# Marking up insertions and deletions

After working through this section, you should be able to:

* Mark up insertions
* Mark up deletions.

## Marking up insertions

The pattern for marking up insertions is as follows:

* Before the inserted text, the opening `{{+`  (note the space after the `+`)
* The inserted text
* The closing `}}`.

{% hint style="info" %}
If the inserted text starts with a space, simply add a second space after the `+`.
{% endhint %}

### Example

```
  All decisions taken should be reported to the Bureau, the {{+ Open-ended}} Working Group and to the next meeting of the Conference of the Parties.

```

Will look like this in View mode:&#x20;

![](<../.gitbook/assets/image (188).png>)

{% hint style="warning" %}
While `{{+ insertions}}` and `__underlines__` look the same in View mode, they just happen to both be styled with an underline for now.

If the style for insertions is updated to a double underline to set them apart from normal underlines, only `{{+ insertions}}` will be updated.
{% endhint %}

## Marking up deletions

The pattern for marking up deletions is as follows:

* Before the deleted text, the opening `{{-`  (note the space after the `-`)
* The inserted text
* The closing `}}`.

{% hint style="info" %}
If the deleted text starts with a space, simply add a second space after the `-`.
{% endhint %}

### Example

```
  The Secretariat shall {{- consult with}}

```

Will look like this in View mode:&#x20;

![](<../.gitbook/assets/image (192).png>)

## Extra markup

In some jurisdictions, extra markup is included in the original: for example in South Africa, deletions are given \[**in bold and with braces**]. In cases like these:

* Ignore the bold — we could always update the style for deletions to be bold rather than strikethrough.
* Leave in the braces, and include them outside the struckthrough text: `[{{- remove this}}]`.

## Exercise

Copy the text below and paste it into a practise document, then see the instructions that follow.

```
A letter of agreement Memorandum of Understanding has been signed between the secretariat of the Basel Convention and the UNEP/OCHA Environmental Unit, identifying the areas and the methodology for cooperation.

```

1. Mark up `letter of agreement` as an insertion.
2. Mark up `Memorandum of Understanding` as a deletion.&#x20;

When you're done, it should look like this in View mode:

![](<../.gitbook/assets/image (260).png>)

and like this in Edit mode:

```
A {{+ letter of agreement}} {{- Memorandum of Understanding}} has been signed between the secretariat of the Basel Convention and the UNEP/OCHA Environmental Unit, identifying the areas and the methodology for cooperation.

```
