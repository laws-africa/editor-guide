# Table errors

The 'Broken table' error will tell you what the system thinks the total rows and columns for the table are.

## Incorrect colspan

![](<../../.gitbook/assets/image (218).png>)

In this example, it says '37 rows and 9 columns'.

A quick count of the top row shows a total of 8 columns: the big one on the left and C1 to C7 on the right. A quick scroll through the table confirms that there aren't more columns later on.

![](<../../.gitbook/assets/image (216).png>)

The first two rows look good:&#x20;

The first row includes a header cell that spans two rows, and 7 more cells.

In the second row, we count one cell for the heading from the previous row, and the second cell spans 7 columns.

The third row spans 9 columns, though, and we know there are only 8.&#x20;

So in this case simply replacing the 9 with an 8 will fix the issue.

(It should also be a `TH` and the bold should be removed, but that's for a separate section.)

![](<../../.gitbook/assets/image (217).png>)

Click 'Update', and the error no longer displays:

![](<../../.gitbook/assets/image (207).png>)
