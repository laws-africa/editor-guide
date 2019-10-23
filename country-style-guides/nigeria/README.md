---
description: Style guide for importing and marking up legislation for Nigeria.
---

# Nigeria

## Cleaning up

### Editorial remarks

{% hint style="danger" %}
Do not remove remarks that indicate amendments, such as `[1992 No. 59]`.

Do use \[\[double squares\]\] – `[[1992 No. 59]]`\(the text will go green to show that it's an editorial remark\).
{% endhint %}

![](../../.gitbook/assets/remark-act.png)

Remove remarks that reference Caps and Schedules.

![](../../.gitbook/assets/remarks-cap.png)

### Empty Subsidiary Legislation

Remove the headings for empty subsidiary legislations, including the primary Act's title, if it's included.

![](../../.gitbook/assets/subleg.png)

## Use Sections in Schedules

Prefer to use Sections in Schedules rather than Crossheadings.

{% hint style="info" %}
If a title appears to belong to only one numbered Section, mark it as a Section, not as a Crossheading.
{% endhint %}

![](../../.gitbook/assets/schedule-section-titles.png)

Markup these sections like this:

```text
1. Supplementary provisions as to the Corporation

(1) A member ofthe corporation may at any time ...

(2) If the chairman is appointed to be ...

(3) If the chairman is absent from ...

2. Eligibility for reappointment

A member of the Corporation who ...
```

## Crossheadings

Add a `CROSSHEADING` where the source documents use _italics_ for crossheadings that cover multiple sections.

{% hint style="danger" %}
DO NOT italicise the Crossheading using `//`as the platform will do it for you.
{% endhint %}

![](../../.gitbook/assets/crossheading.png)

## Schedule Titles and Headings

Use Schedule Headings where possible, rather than Crossheadings.  

![](../../.gitbook/assets/schedule-headings.png)

```text
SCHEDULE - Second Schedule (Section 7.)
Assets to be transferred to the Corporation

PARA 1. The interests of the State in fixed and movable property ...

PARA 2. The interests of the State in any land or timber ...
```

{% hint style="info" %}
The Schedule heading comes on the next line immediately after the keyword `SCHEDULE`.
{% endhint %}

{% hint style="info" %}
Use Sentence case for the Schedule title, and put any reference to the referring section in brackets.
{% endhint %}

