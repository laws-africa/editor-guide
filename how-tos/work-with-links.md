# Working with links

## How to manually insert a link

See [Marking up links](../markup-guide/marking-up-links.md).

## How to manually remove a link

The aim is to delete the link markup as well as the link itself, while keeping the linked text.

1. Enter Edit mode.
2. Delete the opening `{{>` and the closing `}}` around the linked text (the markup).
3. Delete the link itself.

{% hint style="warning" %}
Don't delete the text immediately after the link.
{% endhint %}

### Example

```
Please visit {{>https://laws.africa our website}} for more information.
```

To unlink the text 'our website', delete `{{>https://laws.africa`  and `}}`, leaving you with:

```
Please visit our website for more information.
```

{% hint style="info" %}
Make sure to get the space immediately after the link, as it's part of the markup.
{% endhint %}

## How to insert an email address link

1. Enter Edit mode.
2. Insert `{{>mailto:info@laws.africa` before the text you want to link.
3. Insert `}}` after the text you want to link.

### Examples

#### Text differs from link

> Please write us at [this address](mailto:info@laws.africa) for more information.

Looks like this in Edit mode:

```
Please write us at {{>mailto:info@laws.africa this address}} for more information.
```

#### Text and link are the same

> Please write us at [info@laws.africa](mailto:info@laws.africa) for more information.

Looks like this in Edit mode:

```
Please write us at {{>mailto:info@laws.africa info@laws.africa}} for more information.
```
