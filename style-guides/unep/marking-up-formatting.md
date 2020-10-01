# Marking up formatting

After working through this section, you should be able to:

* Mark up superscripts
* Mark up subscripts
* Mark up bold
* Mark up italics.

## Marking up superscripts

The pattern for marking up superscripts is as follows:

* Before the superscripted text, the opening `{{^`
* The text to be superscripted
* The closing `}}`.

{% hint style="warning" %}
Spaces and any punctuation that are included between `{{^` and `}}` will also be superscripted.
{% endhint %}

### Example

```text
On the 15{{^th}} of July 2020 …
```

will look like this in View mode:

![](../../.gitbook/assets/image%20%28100%29.png)

## Marking up subscripts <a id="marking-up-subscripts"></a>

The pattern for marking up subscripts is as follows:

* Before the subscripted text, the opening `{{_`
* The text to be subscripted
* The closing `}}`.

{% hint style="warning" %}
Spaces and any punctuation that are included between `{{_` and `}}` will also be subscripted.
{% endhint %}

### Example

```text
The amount of CO{{_2}} in the atmosphere …
```

will look like this in View mode:

![](../../.gitbook/assets/image%20%28117%29.png)

## Marking up bold text <a id="marking-up-subscripts"></a>

The pattern for marking up bold text is as follows:

* Before the bold text, the opening `**`
* The text to be bolded
* The closing `**`.

{% hint style="warning" %}
Spaces and any punctuation that are included between the `**`s will also be bolded.
{% endhint %}

### Example

```text
**This whole sentence is bold.**
```

will look like this in View mode:

![](../../.gitbook/assets/image%20%28105%29.png)

## Marking up italics text <a id="marking-up-subscripts"></a>

The pattern for marking up italics text is as follows:

* Before the italics text, the opening `//`
* The text to be italicised
* The closing `//`.

{% hint style="warning" %}
Spaces and any punctuation that are included between the `//`s will also be italicised.
{% endhint %}

### Example

```text
Just //this text// is in italics.
```

will look like this in View mode:

![](../../.gitbook/assets/image%20%28114%29.png)

## Exercise

Copy the text below and paste it into a practise document, then see the instructions that follow.

```text
PARA 12.
  
    On the 12th of July 2020, the amount of CO2 in the atmosphere was bold.
    
    Later that same month is was italics.
    
```

1. Mark up the `th` in the 'the 12th of July' as superscripted.
2. Mark up the `2` in 'CO2' as subscripted.
3. Mark up the word `bold` as bold.
4. Mark up the word `italics` as italics.

When you're done, it should look like this in View mode:

![](../../.gitbook/assets/image%20%28115%29.png)

and like this in Edit mode:

![](../../.gitbook/assets/image%20%28120%29.png)

