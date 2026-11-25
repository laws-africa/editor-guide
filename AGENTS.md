# Repository Guidelines

Guidance for coding and documentation agents working in this repository.

## Purpose and Structure

This repository contains the Laws.Africa Editor Guide as GitBook Markdown.
Its audience is editors and reviewers who manage, mark up, and consolidate
legislation on the Laws.Africa platform.

- `README.md`: guide landing page.
- `SUMMARY.md`: published table of contents and navigation order.
- `getting-started/`: lessons, signup, digitisation, and core terminology.
- `editors/`: import cleanup, warnings, review, and sign-off workflows.
- `how-tos/`: task-based instructions, document settings, and bulk operations.
- `managing-works/`: work metadata, commencements, amendments, and bulk imports.
- `markup-guide/`: editor plaintext syntax and keyword reference.
- `style-guides/`: shared Laws.Africa and jurisdiction-specific editorial rules.
- `administration/`: site settings, administrators, places, and taxonomies.
- `.gitbook/assets/`: screenshots, images, and recordings used by the guide.
- `.gitbook/includes/`: reusable content snippets.

Some pages exist outside `SUMMARY.md`, including pages under
`editing-a-document/`, `doing-tasks/`, and `document-elements/`, and alternative
versions of pages under `managing-works/` and `style-guides/`. Start with
`SUMMARY.md` to identify the page readers reach. Check inbound links before
changing similarly named pages; do not assume an unlisted page is unused.

There is no configured local build or automated test suite. Treat the Markdown,
GitBook directives, navigation, and assets as the documentation source.

## Editing Rules

- Keep changes focused on the requested documentation area; preserve unrelated
  working-tree changes and avoid broad formatting churn.
- Update `SUMMARY.md` when adding, moving, renaming, or removing reader pages.
  Preserve its hierarchy unless the task calls for reorganisation.
- When moving a page, update inbound links and its relative links to pages,
  includes, and assets. Preserve existing page paths and heading anchors where
  possible, since they may be linked from the application or other guides.
- Keep this `AGENTS.md` out of `SUMMARY.md`; it is agent guidance.
- Preserve GitBook front matter, directives, HTML figures, captions, and embeds.
- Keep existing screenshots and recordings unless the task requires changing
  them. Do not rename, recompress, or delete assets as incidental cleanup.
- Never add credentials, private implementation details, production extracts,
  or personal information to examples or screenshots.

## Writing and Editorial Standards

- Use clear, direct prose and UK/South African English conventions.
- Explain concepts before relying on terms such as work, expression, point in
  time, commencement, consolidation, and Akoma Ntoso. Follow the terminology in
  `getting-started/terminology-guide.md`.
- Use descriptive headings, numbered steps for ordered procedures, and bullets
  for reference lists. State prerequisites and the expected outcome.
- Match UI labels and explain which page, tab, or editor mode a step uses.
  Verify workflow changes against relevant current code or observed UI; do not
  infer current behaviour solely from an older screenshot.
- Consult `style-guides/laws.africa.md` and the relevant jurisdiction's guide
  before changing editorial examples. Preserve jurisdiction-specific rules and
  distinguish them from general platform behaviour.
- Preserve the meaning of quoted legislation, dates, numbering, amendment
  annotations, and commencement details. Do not silently resolve uncertain
  legal or editorial policy questions by inventing a rule.
- Keep review, sign-off, and publication prerequisites and consequences explicit.
- Wrap new prose at about 100 characters where practical. Do not reflow markup
  examples, tables, URLs, directives, or HTML merely to meet a line limit.

## Markdown and GitBook Conventions

- Use one `#` heading per reader page and keep the navigation title consistent.
  Preserve existing YAML front matter; add descriptions when useful and in
  keeping with nearby pages.
- Preserve paired directives such as `{% hint %}` / `{% endhint %}` and
  `{% content-ref %}` / `{% endcontent-ref %}`, including their attributes.
- Prefer relative links to existing Markdown pages within this guide. Directory
  links should resolve to the intended `README.md`. Use existing heading anchors
  when linking to a section.
- Reference local media from `.gitbook/assets/` relative to the page. Preserve
  exact filename case, spaces, and parentheses; keep angle-bracket destinations
  for filenames containing spaces or parentheses where needed.
- Preserve `<figure>`, `<img>`, and `<figcaption>` markup when editing existing
  media. Give new screenshots useful alternative text or captions.
- Use fenced code blocks for plaintext markup examples. Preserve indentation,
  keywords, escaping, and inline syntax: indentation is meaningful to the editor
  parser. Check `markup-guide/keyword-reference.md` and related examples before
  changing syntax; do not invent keywords or normalise examples as prose.

## Validation

For documentation changes:

1. Check changed relative page, asset, and include links, including filename case
   and heading anchors. Search for inbound references if a page moved.
2. Check `SUMMARY.md` entries and nesting when navigation changes. Do not add
   reusable snippets or agent instructions to reader navigation.
3. Review GitBook directive pairing, front matter, code fences, figures, and
   significant indentation in markup examples.
4. Check procedure order, UI labels, prerequisites, and jurisdiction-specific
   examples. If a GitBook preview is available, inspect affected pages there;
   report any rendering or behaviour verification that was unavailable.
5. Run `git diff --check` and review the scoped diff before finishing. A newly
   created `AGENTS.md` is untracked until added, so inspect it separately too.

Do not introduce a build toolchain or run Django tests for documentation-only
changes. In PR descriptions, summarise the affected pages and validation, and
identify any workflow behaviour that was verified against code or UI.
