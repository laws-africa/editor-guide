# Table errors

The 'Broken table' error will tell you what the system thinks the total rows and columns for the table are.

## Incorrect colspan

### Example 1

![](<../../../.gitbook/assets/image (23).png>)

In this example, it says '37 rows and 9 columns'.

A quick count of the top row shows a total of 8 columns: the big one on the left and C1 to C7 on the right. A quick scroll through the table confirms that there aren't more columns later on.

#### Diagnosis

![](<../../../.gitbook/assets/image (78).png>)

The first two rows look good:&#x20;

The first row includes a header cell that spans two rows, and 7 more cells.

In the second row, we count one cell for the heading from the previous row, and the second cell spans 7 columns.

The third row spans 9 columns, though, and we know there are only 8.&#x20;

#### Fixing it

In this case simply replacing the 9 with an 8 will fix the issue.

(It should also be a `TH` and the bold should be removed, but that's for a separate section.)

![](<../../../.gitbook/assets/image (274).png>)

Click 'Update', and the error no longer displays:

![](<../../../.gitbook/assets/image (262).png>)

### Example 2

![](<../../../.gitbook/assets/image (242).png>)

In this example, it says '51 rows and 11 columns'.

From first glance it seems as if the table should have 3 columns (not 11). A quick scroll through the table confirms that there aren't more columns later on.

#### Diagnosis

![](<../../../.gitbook/assets/image (273).png>)

The first two rows look wrong:

The first row has three cells, but the second cell spans 7 columns and the third cell spans 3 columns.&#x20;

In the second row, The second cell spans 10 columns and there is no third cell.

This colspanning repeats throughout the table, but there are never more than three cells in a row.

#### Fixing it

First, it's important to note that some cells in the table legitimately span columns: some span all three columns, and a few span only the second and third column.

In Edit mode, search for `colspan` and either:&#x20;

* Remove the whole of e.g. `{colspan 7}` or `{colspan 3}`, or
* Replace e.g. `{colspan 11}` with `{colspan 3}`,

as appropriate.

{% hint style="info" %}
You can tell which cells legitimately span columns by looking at how many cells there are in that row:&#x20;

* If there's only one cell, it should have `{colspan 3}`, and
* If there's only two cells, one of them should have `{colspan 2}`,

in a 3-column table.
{% endhint %}

Click 'Update', and the error no longer displays:

![](<../../../.gitbook/assets/image (268).png>)
