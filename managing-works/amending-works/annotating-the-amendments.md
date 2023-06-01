# Annotating the amendments

Annotations are how we show readers what happened to a piece of legislation over time. We make an annotation under each change, specifying what the change is and how it came about.

## How to insert an automatically created annotation

1. In Edit mode, place your cursor in the line below the one where the change was made.
2. Click 'Insert | Insert annotation …' and select the appropriate verb (refer to the amending work).
3. Amend the annotation:
   * First, double-check that the amending work is correct — especially when there are multiple amendments at the same date.
   * Replace the section reference (`section 10` in the screenshot below) with the provision that was affected – in this case, `subsection (2)`.
   * Replace `XXX` with the section of the amending work that made this particular change. (If the amending work doesn't have sections, delete all of `section XXX of`.)
4. In our example, the final annotation will read `{{*[subsection (2) substituted by section 8(1)(b) of the {{>/za-playground/act/by-law/2020/practice-3 Amendment By-law, 2020}}]}}` – note it does not start with a capital letter, and there are no spaces between the brackets in the reference to section 8(1)(b).

![Inserting the annotation](<../../.gitbook/assets/image (78).png>)

![The automatically inserted annotation still needs to be edited](<../../.gitbook/assets/image (211) (2).png>)

## How to write an annotation from scratch

Amendments have four elements:

1. The provision of the amended work
2. The verb associated with the amendment
3. The provision of the amending work
4. The actual change.

Annotations reflect the first three elements in the following way:

```
<provision of amended work> <verb>ed by <provision> of <amending work>
```

For example:

```
{{*[subsection (1) deleted by section 12 of Act 3 of 2019]}}
```

or:

```
{{*[definition of "consumer" substituted by section 1(a) of the Electricity Supply Amendment By-law, 2017]}}
```

## Tips

* Wrap annotations in `{{*[annotation markup]}}`, because they are editorial remarks.
* Make the annotation as close to the change as possible.
* To determine the verb, follow what is given in the amending work. \
  (For example, 'altered' seems to be preferred over 'amended' in Nigeria.)
* When the amending work doesn't have an Act number, use its short title.

## Placement of annotations when a new Chapter/Part/Schedule is inserted

* When an entire new Chapter/Part/Schedule is **inserted**, place the annotation at the top, directly underneath the heading.
* Also place an annotation underneath each section in the new Chapter/Part. These annotations are only inserted when the Chapter/Part has been **inserted**, not if it has been **substituted**.
* When a new Schedule is inserted, just the one annotation at the top is necessary.
