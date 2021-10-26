# Keyword reference

## Structural markup

| Keyword       | Description                                                                                                                    |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| `PREFACE`     | Introduces the Preface                                                                                                         |
| `PREAMBLE`    | Introduces the Preamble                                                                                                        |
| `BODY`        | Introduces the main body (can be left out if there's no Preface or Preamble)                                                   |
| `SCHEDULE`    | Introduces a Schedule (see the full list of Schedule-like blocks below)                                                        |
| `DIVISION`    | Introduces a group of numbered paragraphs; number and heading both optional                                                    |
| `SUBDIVISION` | Introduces a group of numbered paragraphs inside a division (or inside a subdivision); number and heading both optional        |
| `PARA`        | Introduces a (usually numbered) paragraph; may also optionally have a heading                                                  |
| `SUBPARA`     | Introduces a (usually numbered) subparagraph inside a paragraph (or inside a subparagraph); may also optionally have a heading |
| `FOOTNOTE`    | Introduces a footnote                                                                                                          |

### Schedule-like blocks

`ANNEXURE`\
`APPENDIX` \
`ATTACHMENT` \
`SCHEDULE`

### Bullets

|   |                                                                                                             |
| - | ----------------------------------------------------------------------------------------------------------- |
| • | Filled circle                                                                                               |
| ◦ | Empty circle                                                                                                |
| ▪ | Filled square                                                                                               |
| ▫ | Empty square                                                                                                |
| ‑ | Short dash (non-breaking hyphen, doesn't get picked up as a `-` (the separation between number and heading) |
| — | Long dash                                                                                                   |

## Table markup

| Keyword                  | Description                                                                                                        |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `TABLE`                  | Introduces a table                                                                                                 |
| `TR`                     | Introduces a table row                                                                                             |
| `TH`                     | Introduces a table heading cell                                                                                    |
| `TC`                     | Introduces a table content cell                                                                                    |
| `{colspan 5}`            | After `TH` or `TC`, gives 5 as the total number of columns this cell will occupy                                   |
| `{rowspan 5}`            | After `TH` or `TC`, gives 5 as the total number of rows this cell will occupy                                      |
| `{colspan 2\|rowspan 3}` | After `TH` or `TC`, gives 2 as the total number of columns and 3 as the total number of rows this cell will occupy |

## Inline markup

| Symbol                                 | Description                                            |
| -------------------------------------- | ------------------------------------------------------ |
| `{{FOOTNOTE x}}`                       | A footnote reference, with `x` as the reference marker |
| `{{^{{FOOTNOTE x}}}}`                  | A superscripted footnote reference                     |
| `{{>https://example.com Linked text}}` | A link                                                 |
| `{{^text to be superscripted}}`        | Superscripted text                                     |
| `{{_text to be subscripted}}`          | Subscripted text                                       |
| `**text to be bolded**`                | Bold text                                              |
| `//text to be italicised//`            | Italics text                                           |
