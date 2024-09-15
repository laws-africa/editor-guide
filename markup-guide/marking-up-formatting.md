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

```
On the 15{{^th}} of July 2020 …
```

will look like this in View mode:

![](<../.gitbook/assets/image (58).png>)

## Marking up subscripts <a href="#marking-up-subscripts" id="marking-up-subscripts"></a>

The pattern for marking up subscripts is as follows:

* Before the subscripted text, the opening `{{_`
* The text to be subscripted
* The closing `}}`.

{% hint style="warning" %}
Spaces and any punctuation that are included between `{{_` and `}}` will also be subscripted.
{% endhint %}

### Example

```
The amount of CO{{_2}} in the atmosphere …
```

will look like this in View mode:

![](<../.gitbook/assets/image (87).png>)

## Marking up bold text <a href="#marking-up-subscripts" id="marking-up-subscripts"></a>

The pattern for marking up bold text is as follows:

* Before the bold text, the opening `**`
* The text to be bolded
* The closing `**`.

{% hint style="warning" %}
Spaces and any punctuation that are included between the `**`s will also be bolded.
{% endhint %}

### Example

```
**This whole sentence is bold.**
```

will look like this in View mode:

![](<../.gitbook/assets/image (259).png>)

## Marking up italics text <a href="#marking-up-subscripts" id="marking-up-subscripts"></a>

The pattern for marking up italics text is as follows:

* Before the italics text, the opening `//`
* The text to be italicised
* The closing `//`.

{% hint style="warning" %}
Spaces and any punctuation that are included between the `//`s will also be italicised.
{% endhint %}

### Example

```
Just //this text// is in italics.
```

will look like this in View mode:

![](<../.gitbook/assets/image (196).png>)

## Exercise

Copy the text below and paste it into a practise document, then see the instructions that follow.

```
PARA 12.
  
    On the 12th of July 2020, the amount of CO2 in the atmosphere was bold.
    
    Later that same month is was italics.
    
```

1. Mark up the `th` in the 'the 12th of July' as superscripted.
2. Mark up the `2` in 'CO2' as subscripted.
3. Mark up the word `bold` as bold.
4. Mark up the word `italics` as italics.

When you're done, it should look like this in View mode:

![](<../.gitbook/assets/image (143).png>)

and like this in Edit mode:

![](<../.gitbook/assets/image (31).png>)
