---
description: Style guide for importing and marking up legislation for Nigeria.
---

# Nigeria

## Cleaning up

### Editorial remarks

{% hint style="danger" %}
Do not remove remarks that indicate amendments, such as `[1992 No. 59]`.
{% endhint %}

![](../.gitbook/assets/remark-act.png)

{% hint style="info" %}
Do use double squares around editorial remarks in Edit mode: `[[1992 No. 59.]]`  
This will show up as italics, single square brackets in View mode: _\[1992 No. 59.\]_
{% endhint %}

Remove remarks that reference Caps and Schedules.

![](../.gitbook/assets/remarks-cap.png)

### Subsidiary legislation

Remove any subsidiary legislation after the Act, including if it says 'No subsidiary legislation'. Delete the name of the Act as well. 

![](../.gitbook/assets/subleg.png)



![](../.gitbook/assets/image%20%289%29.png)

{% hint style="info" %}
The document should end with the last Schedule to the main Act, or with the last section of the main Act if it has no Schedules.
{% endhint %}

## Use Sections in Schedules

Prefer to use Sections in Schedules rather than Crossheadings.

{% hint style="info" %}
If a title appears to belong to only one numbered Section, mark it as a Section, not as a Crossheading.
{% endhint %}

![](../.gitbook/assets/schedule-section-titles.png)

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

![](../.gitbook/assets/crossheading.png)



