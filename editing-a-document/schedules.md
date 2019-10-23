# Schedules

A schedule comes at the end of the main Act. It is a separate from the main content and has a separate heading, subheading and table of contents.

A schedule has a heading, such as 'First Schedule' or sometimes just 'Schedule'. Some schedules also have a subheading, such as 'Laws Amended'.

## How to structure a Schedule

1. Introduce the Schedule with `SCHEDULE -`.
2. Put the schedule heading after the dash, such as `Schedule`, `Schedule 2`, `Third Schedule`.
3. If the schedule has a subheading, put it on the very next line.

{% hint style="warning" %}
Do not use `CROSSHEADING` for the Schedule heading.
{% endhint %}

## Numbered paragraphs in schedules

If the Schedule has numbered sections or numbered paragraphs with heading, mark them up in the same way you would for numbered sections:

```text
2. Heading of the paragraph

Content of the paragraph...
```

 If the Schedule has numbered paragraphs that don't have headings, use the `PARA` keyword instead. 

```text
PARA 2. Content of the paragraph...
```

### How to indent subparagraphs

When a numbered paragraph \(`PARA`\) has numbered subparagraphs, ensure that you indent the subparagraphs so that the system recognises them as a subparagraph, and not as a subsection:

```text
PARA 1.

    (1) This should align nicely.

    (2) As should this.
```

{% hint style="warning" %}
The subparagraph won't be indented correctly if you use the wrong markup.
{% endhint %}

```text
PARA 3. (1) This, on the other hand, will not be correctly indented.

(2) And neither will this.
```

## Articles in schedules

If the Schedule uses numbered Articles and not paragraphs, use the `Article` keyword like you would for a Chapter. 

```text
Article 1 - Heading of the Article

Content of the article...
```

## Exercise

* [ ] Copy and paste the text below into the editor.

```text
Schedule 1: Amendment of laws

1. Heading heading

1.1 Content content content.

1.1.1 Content content content.

1.1.2 Content content content.

1.1.3 Content content content.

1.2 Content content content.

2. Heading heading

Content content content.

Schedule 2
The Agreement
(Section 12)

1. The Agreement is important.

2. The Agreement states-

(a) some interesting things;

(b) some more things.

3. (1) Blah blah blah.

(2) Blah blah blah.

Schedule 3

Some other heading

Article 1. The important thing

Content content content.

Article 2. Another heading

Content content content.


```

* [ ] Click Update.
* [ ] Quick edit Schedule 1:  Fix the title and the heading.
* [ ] Quick edit Schedule 2:  Use `CROSSHEADING` for the section reference; Use `PARA`s;  Update, and fix `PARA` 3 by indenting the subparagraphs.
* [ ] Quick edit Schedule 3:  Fix the heading.



