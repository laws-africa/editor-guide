# Marking up links

After working through this section, you should be able to:

* Mark up a link.

The pattern for marking up links is as follows:

* In the text where the link appears, the opening `{{>`
* Immediately afterwards, the URL of the link
* A space, followed by the text that should appear
* The closing `}}`.

{% hint style="info" %}
If the linked text is the link itself, simply repeat it: once as the URL, and once as the text.
{% endhint %}

{% hint style="warning" %}
The link should never include spaces, and should always start with `https://` or `http://`if it's external.
{% endhint %}

### Examples

#### Text differs from link

> Please visit [our website](https://laws.africa) for more information.

Looks like this in Edit mode:

```
Please visit {{>https://laws.africa our website}} for more information.
```

If you click on the linked text ('our website'), you will be taken to [https://laws.africa](https://laws.africa).

#### Text and link are the same

> Please visit [https://laws.africa](https://laws.africa) for more information.

Looks like this in Edit mode:

```
Please visit {{>https://laws.africa https://laws.africa}} for more information.
```

## Exercise

Copy the text below and paste it into a practise document, then see the instructions that follow.

```
More information at our website.
```

1. Insert the opening `{{>` before 'our website'.
2. Insert the URL `https://laws.africa` immediately after the opening `{{>`, followed by a space.
3. Insert the closing `}}` after 'our website' and before the full stop.

When you're done, it should look like the example above in View mode.

Try clicking on the linked text. Were you directed to [https://laws.africa](https://laws.africa)?

Now replace the text 'our website' with the URL, and see what it looks like.
