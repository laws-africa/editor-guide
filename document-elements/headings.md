# Headings

Chapters and Parts are often used to group sections. Sometimes a Chapter will contain Parts, and sometimes a Part will contain Chapters. Subparts serve the same function, but usually only have a number \(or letter\) and a heading. Crossheadings don't group sections and they never have a number; they are standalone headings.

## How to mark up Chapters

1. Enter Edit mode.
2. On one line, start a Chapter with `Chapter <number> - <heading>`.
3. The heading is optional and should use [Sentence case](../style-guides/laws.africa.md#headings), not ALL CAPS.
4. Use "space hyphen space" between the number and the heading.
5. Put the contents of the Chapter on the following lines.

**Example**

```text
Chapter 2 - Interpretation

2. Terms

The following terms shall be interpreted …
```

## How to mark up Parts

1. Enter Edit mode.
2. On one line, start a Part with `Part <number> - <heading>`.
3. The heading is optional and should use [Sentence case](../style-guides/laws.africa.md#headings), not ALL CAPS.
4. Use "space hyphen space" between the number and the heading.
5. Put the contents of the Part on the following lines.

**Example**

```text
Part 2 - Tariffs

4. Calculating tariffs

Tariffs shall be calculated …
```

## How to mark up Subparts

1. Enter Edit mode.
2. On one line, start a Subpart with `SUBPART <number> - <heading>`.
3. The number and heading are both optional, but you should use at least one.
4. The heading should use [Sentence case](../style-guides/laws.africa.md#headings), not ALL CAPS.
5. Use "space hyphen space" before the heading.
6. Put the contents of the Subpart on the following lines.

**Example**

```text
SUBPART A - Fines

6. Calculating fines

(1) Fines should never …
```

{% hint style="warning" %}
If the Subpart doesn't have a number, you should still use a hyphen before the heading – otherwise the heading will be recorded as the number in the XML.
{% endhint %}

## How to mark up Crossheadings

Only use Crossheadings when no other type of heading or grouping makes sense. This happens most often in Schedules.

1. Enter Edit mode.
2. On one line, mark text as a heading with `CROSSHEADING <the heading>`.
3. The heading should use [Sentence case](../style-guides/laws.africa.md#headings), not ALL CAPS.

**Example**

```text
Regular text.

CROSSHEADING The heading

More regular text.
```

## Exercise

1. In Edit mode, copy and paste the following content into your editor.
2. Correct it so that it looks like the screenshot below in View mode.
   1. Chapter 2 should have the correct heading \(using Sentence case\).
   2. Part 1 should have the correct heading \(also using Sentence case\).
   3. The first Subpart should contain sections 5 and 6.
   4. The second Subpart should contain sections 7 and 8.

```text
2
GENERAL

Part: 1
Municipal Services and Taxes

Services

5. Rubbish removal

Rubbish removal will be …

6. Stormwater drainage

Stormwater should …

Taxes

7. Calculating taxes

Taxes are …

8. Paying taxes

Taxes should …

```

Your goal is to make it look like this:

![](../.gitbook/assets/image%20%2884%29.png)

