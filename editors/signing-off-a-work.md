# Signing off a work

Signing off a work makes it available on a publishing partner's website (e.g. [lawlibrary.org.za](https://lawlibrary.org.za/)).&#x20;

The purpose of the 'Review and publish changes' task is to make sure that what we have captured on the platform is ready to be seen publicly. This includes the **metadata** and the **content**.

## Picking up a sign-off task

To find sign-off tasks, filter to 'Sign-off' under 'Task type' in any task listing view.

![](<../.gitbook/assets/image (225).png>)

As with any other task, click the task title to go to the task detail page and select yourself under 'Assign to'.

![](<../.gitbook/assets/image (223).png>)

Click 'Review changes' to see the changes that have been lined up for sign-off.

## Before starting the review

Have a look at any open tasks on the work. Presumably the Import task has been done, or the latest amendment has been applied, but are there any other outstanding tasks?&#x20;

You'll need to make a judgement call based on what those tasks might be: can the work go live to the public before an outstanding question is addressed?

For example, if crucial metadata is missing and we've used a placeholder for, say, the Act number and year, this work probably shouldn't be signed off yet. In this case, you can mark the sign-off task as blocked by the other task on the work and move on to the next task for the time being.

But if there's a task open to indicate not all defined terms were captured by the terms finder, this shouldn't block the sign-off.

## Doing the review

![The first part of the sign-off task (metadata)](<../.gitbook/assets/image (207).png>)

In the above example, the work is being published for the first time.

Every new item (in this case all of them) is highlighted in green. Any items that have been removed since the last sign-off will be highlighted in red.

Each of the pieces of metadata should be checked against the original. If all are right and none are missing, check the 'Approve these changes' box, and click 'Next'.

![The next part of the sign-off task (content)](<../.gitbook/assets/image (190).png>)

Check the content against the original, looking especially at the structure of the document.

If a commencements table appears at the top, make sure to check each of those entries as well.&#x20;

* If a provision has been inserted / added by an amendment, this provision will show in the commencements table as "uncommenced". It should be showing as having commenced on the effective date of the amendment, so this needs to be fixed.
* You will have to do this manually, i.e. go to the commencement tab on the work and create a new commencement at the appropriate date by that amending work, then tick the new provisions that have been inserted.
* See here for detailed instructions on how to create a new commencement date: [#insertion-of-new-sections-by-amendment](../managing-works/creating-and-editing-works/working-with-commencements.md#insertion-of-new-sections-by-amendment "mention").

Once the commencement table is complete, go to the "commencements" tab on the work and remove any notes that have been left regarding which provisions commence on the different dates. If the work is a stub, **do not remove** the notes as stubs do not have commencement tables and we need to have that information recorded.

If everything looks good, check the 'Approve these changes' box at the bottom of this page too.



![](<../.gitbook/assets/image (206).png>)

Once all the changes have been approved, the 'Publish changes' button will activate. You should click it to complete the task.

{% hint style="info" %}
Unlike with other tasks, you don't need to approve or close the 'Review and publish changes' task. It automatically closes when you click 'Publish changes'.
{% endhint %}

## What if it's not all good?

The above is the ideal scenario: a final eye over to confirm nothing has slipped through the cracks before the work goes live to the public.

If changes do need to be made, there are two common patterns to follow:

### Make tweaks and publish

* If the **content** needs to change:
  * Edit the document, and click 'Save & publish' when it's ready.
  * Give **feedback** to the editor and reviewer of the Import task by making a comment on the closed task describing the tweaks you made. They should both receive notifications of the comment, but you'e also free to follow up with them.
* If the **metadata** needs to change:
  * Check with the researcher or the project owner before making metadata changes, as they may have more context than you.
  * Once you're on the same page, edit the work or the relevant commencement.
* When you're confident the sign-off task can proceed:
  * **Reload** the page if you still have it open, or 'Publish changes' at the end will fail.
  * Continue with your review.

{% hint style="warning" %}
The part about reloading the page before continuing the review is serious – don't end up having to review the same thing twice!
{% endhint %}

{% content-ref url="../managing-works/creating-and-editing-works/" %}
[creating-and-editing-works](../managing-works/creating-and-editing-works/)
{% endcontent-ref %}

{% content-ref url="../managing-works/creating-and-editing-works/working-with-commencements.md" %}
[working-with-commencements.md](../managing-works/creating-and-editing-works/working-with-commencements.md)
{% endcontent-ref %}

### Placeholder date&#x20;

Sometimes we might get documents that need to be imported that do not have dates. To solve the problem of importing these documents while we look for a date, we use the date **01-01-1600** as a placeholder. When you see a work with this date, **please do not sign it off**. Such a work can only be signed off once the correct date has been found. On encountering such a work, create a task on it detailing that the correct date needs to be found, if such a task does not already exist.&#x20;

### Send back for changes

This should be a rare case, as major changes should be picked up during review. But if the content still needs a lot of work, or the wrong document was imported, for example:

* Reopen the closed Import task, with a comment describing the changes that need to be made.
* Mark the sign-off task as blocked by the now-open Import task.

{% hint style="warning" %}
Once the Import task has been re-approved, the Sign-off task will need to be **unblocked and submitted** before the sign-off is done, since it's a special type of task that only really exists in the 'pending review' state.
{% endhint %}
