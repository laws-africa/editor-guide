---
description: Manage the taxonomies used to group works into collections.
---

# Taxonomies

Taxonomies are used to group works into collections. The platform supports multiple taxonomies and a work can belong to any number of taxonomies.

## About taxonomies

You can think of a taxonomy as a collection of folders called **topics**. The topics form a hierarchy or a tree of options.

A taxonomy topic in the tree has these properties:

* **Name**: the title of the topic
* **Description**: an optional description of the topic
* **Public**: is this topic visible to external users of the platform? Note: This only applies to topics at the top-level of the taxonomy tree.
* **Project**: is this topic used for grouping works into projects within the platform? If this is checked, then this taxonomy will be shown in the project dropdown when editing works.

### Using taxonomies to manage tasks and works

In the Works and Tasks listing views, use the taxonomy topic tree on the left to show only works or tasks that are tagged with certain topics.

<div align="center" data-full-width="false">

<figure><img src="../.gitbook/assets/Works – South Africa – Laws.Africa 2024-09-13 14-51-35.png" alt=""><figcaption></figcaption></figure>

</div>

### Using taxonomies for subject area tags

A useful application of public-facing taxonomies is to tag legislation with subject-area tags, such as "Finance and Money" or "Arts and Culture".

This topics will be available to external users of this information, and helps them to understand what a piece of legislation is about.

For example, a subject area taxonomy tree may look like this:

* Subject areas
  * Arts and Culture
  * Business, Trade and Industry
  * Citizenship
  * Education
  * etc.

The best way to achieve this is:

1. Create a top-level topic in the taxonomy tree called **Subject areas.**
2. Ensure the **public** checkbox for that topic is checked.
3. Add the necessary sub-topics (child topics or sub-folders) underneath the Subject areas topic.&#x20;
4. Tag each work with one or more subject area topics.

### Using taxonomies for project groupings

Taxonomies can be used internally to group works for managing digitisation projects and priorities.

For example, a project taxonomy tree may look like this:

* Projects
  * Priority 1: High priority
    * Recent updates
    * High priority acts
  * Priority 2: Medium priority
    * Regulations for Health and Safety
  * Priority 3: Low priority
    * Repealed and out-dated legislation

The best way to achieve this is:

1. Create a top-level topic in the taxonomy tree called **Projects**
2. Ensure the **public** checkbox is **NOT checked**, so that the projects are not visible to the public.
3. Ensure the **projects** checkbox is checked.
4. Add the necessary sub-topics (child topics or sub-folders) undernetah the Projects topic.
5. Tag each work with a project tag.

## Adding a new taxonomy topic

To add a new taxonomy topic:

1. Open the admin interface
2. Under **Indigo API** click on **Taxonomy Topics**
3. Click **Add Taxonomy Topic**
4. Enter the **Name,** a user-friendly title for the topic
5. Enter the **Description**, a brief description of the topic (optional)
6. If this part of the taxonomy tree must be publicly-visible, check the **Public** checkbox. This only applies to top-level entries of the taxonomy tree.
7. If this part of the taxonomy tree will be used to manage projects, check the **Project** checkbox. This only applies to top-level entries of the taxonomy tree.
8. **Copy from principal work**: when checked, this topic will be copied from a principal work to all works that amend, repeal or commence the principal work. This is useful for ensuring that all works that impact a principal work have this particular topic. In most cases, do not select this option.
9. Use **Position** to choose how to position this taxonomy topic in the tree.
   1. **Child of**: the topic will be a child (sub-topic) of the topic chosen in the **Relative to** box.
   2. **Sibling of**: the topic will be at the same level of the topic chosen in the **Relative to** box.
10. In the **Relative to** box, choose the parent (for **Child of**) or sibling (for **Sibling of**) of the topic.
11. For a new top-level topic, choose **Child of** and **-- root --**.
12. Click **Save**

<figure><img src="../.gitbook/assets/image (233).png" alt=""><figcaption></figcaption></figure>

## Editing a taxonomy topic

To edit an existing taxonomy topic:

1. Open the admin interface
2. Under **Indigo API** click on **Taxonomy Topics**
3. Use the **Search** box, **Expand all** and **Collapse all** buttons to help you find the topic you're looking for
4. Click on the taxonomy to edit it
5. Make your changes
6. To delete a topic, check the **Delete** checkbox
7. Click **Save**

## Deleting a taxonomy topic

Deleting a taxonomy topic will remove it from any works linked to it. To delete a taxonomy topic:

1. Open the admin interface
2. Under **Indigo API** click on **Taxonomies**
3. Use the **Search** box, **Expand all** and **Collapse all** buttons to help you find the topic you're looking for
4. Click on the taxonomy to delete
5. Click **Delete**
