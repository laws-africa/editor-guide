# Keyword reference

## Structural markup

| Keyword                  | Description                                                                  |
| ------------------------ | ---------------------------------------------------------------------------- |
| `PREFACE`                | Introduces the Preface                                                       |
| `PREAMBLE`               | Introduces the Preamble                                                      |
| `BODY`                   | Introduces the main body (can be left out if there's no Preface or Preamble) |
| `CHAP 1 - Heading`       | Introduces a Chapter                                                         |
| `PART A - Heading`       | Introduces a Part                                                            |
| `SUBPART X - Heading`    | Introduces a Subpart                                                         |
| `DIVISION X - Heading`   | Introduces a Division                                                        |
| `SUBDIVISION`            | Introduces a Subdivision                                                     |
| `SEC 1. - Heading`       | Introduces a section                                                         |
| `SUBSEC` (`1) - Heading` | Introduces a subsection                                                      |
| `PARA (a) - Heading`     | Introduces a paragraph                                                       |
| `SUBPARA (i) - Heading`  | Introduces a subparagraph                                                    |
| `ART 1 - Heading`        | Introduces an article                                                        |
| `SCHEDULE`               | Introduces a Schedule (see the full list of Schedule-like blocks below)      |
| `QUOTE{startQuote “}`    | Introduces a quote                                                           |
| `FOOTNOTE`               | Introduces a footnote                                                        |

### Schedule-like blocks

`ANNEXURE`\
`APPENDIX` \
`ATTACHMENT` \
`SCHEDULE`

## Inline markup

| `\`                                    | Escape a special keyword                               |
| -------------------------------------- | ------------------------------------------------------ |
| `LONGTITLE`                            | Introduces the Long title                              |
| `CROSSHEADING`                         | Introduces a Crossheading                              |
| `{{*[annotation]}}`                    | An annotation                                          |
| `{{^superscript}}`                     | Superscripted text                                     |
| `{{_subscript}}`                       | Subscripted text                                       |
| `**bold**`                             | Bold text                                              |
| `//italics//`                          | Italics text                                           |
| `__underline__`                        | Underlined text                                        |
| `{{>https://example.com Linked text}}` | A link                                                 |
| `{{IMG media/logo.png}}`               | An image                                               |
| `{{FOOTNOTE x}}`                       | A footnote reference, with `x` as the reference marker |
| `{{^{{FOOTNOTE x}}}}`                  | A superscripted footnote reference                     |
| `{{+ ins}}`                            | Inserted text                                          |
| `{{- del}}`                            | Deleted text                                           |

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
