# Working with links

## How to manually insert a link

1. Enter Edit mode.
2. Wrap the text you want to link in \[square brackets\].
3. Insert the link in \(round brackets\), immediately after the closing square bracket \(no space\).

{% hint style="info" %}
The link \(in round brackets\) should never include spaces, and should always start `https://` or `http://`if it's external.
{% endhint %}

### Example: Text differs from link

> Please visit [our website](https://laws.africa) for more information.

Looks like this in Edit mode:

```text
Please visit [our website](https://laws.africa) for more information.
```

### Example: Text and link are the same

> Please visit [https://laws.africa](https://laws.africa) for more information.

Looks like this in Edit mode:

```text
Please visit [https:\/\/laws.africa](https://laws.africa) for more information.
```

{% hint style="info" %}
The slashes get escaped as`\/\/` in the square brackets only.
{% endhint %}

## How to manually remove a link

1. Enter Edit mode.
2. Delete the opening and closing \[square brackets\] around the linked text.
3. Delete the link and its \(round brackets\).

{% hint style="warning" %}
Don't delete the text inside the square brackets.
{% endhint %}

### Example

To unlink the text in the example above, in Edit mode delete `[`  as well as `](https://laws.africa)`, leaving you with:

```text
Please visit our website for more information.
```

## How to insert an email address link

1. Enter Edit mode.
2. Wrap the text you want to link in \[square brackets\].
3. Insert 'mailto:' and the email address in \(round brackets\), immediately after the closing square bracket.
4. Don't use a space after `mailto:` or between `](`.

### Example: Text differs from link

> Please write us at [this address](mailto:info@laws.africa) for more information.

Looks like this in Edit mode:

```text
Please write us at [this address](mailto:info@laws.africa) for more information.
```

### Example: Text and link are the same

> Please write us at [info@laws.africa](mailto:info@laws.africa) for more information.

Looks like this in Edit mode:

```text
Please write us at [info@laws.africa](mailto:info@laws.africa) for more information.
```

