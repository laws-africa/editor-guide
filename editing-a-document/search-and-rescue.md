# Search and rescue

When cleaning up an import, depending on the quality of the scan / consolidation you're working with, you may find things that are consistently wrong. Finding all the instances of a mistake will help you to ensure the quality of the content without worrying that one or two may have slipped through the cracks.

## How to find all instances of 'N' instead of '₦'

1. With the Entire document selected, enter Edit mode.
2. Click **Edit** and then **Find**.
3. Select the first \(`.*`\) and second \(`Aa`\) options above the Search bar.
4. Type `N ?\d` into the Search bar: this will look for capital `N` followed by any number \(`0` to `9`\), with an optional space between. It will take you to the first instance, if there is one.
5. Manually replace the N with ₦.
6. Hit Enter in the Search bar again to go to the next instance.
7. Repeat Steps 5 and 6 until all instances have been fixed.

![](../.gitbook/assets/image%20%2839%29.png)

{% hint style="warning" %}
Don't use 'Edit \| Find next' – this will only find the next instance of `N1` in the example above, rather than using the regular expression `N ?\d`.
{% endhint %}

### Exercise

1. Copy and paste the text below into the editor.
2. Use the instructions given above to fix all instances of N being used instead of ₦.

```text
32. Reconstruction investment allowance

(1) Any person who, without reasonable excuse, fails to comply with this section, shall be guilty of an offence and liable on conviction to a penalty not exceeding N100 plus the amount of tax lost by the granting of the investment allowance made in respect of the expenditure in question.

(2) For the purposes of subsection (1) of this section the minimum tax to be levied and paid shall‐

    (a) if the turnover of the company is ₦500,000 or below and the company has been in business for at least four calendar years be‐

        (i) 0.5 per cent of gross profit; or

        (ii) 0.5 per cent of net assets; or

        (iii) 0.25 per cent of paid‐up capital; or

        (iv) 0.25 per cent of turnover of the company for the year,

        whichever is higher; or

    (b) if the turnover is higher than N500,000, be whatever is payable in paragraph (a) of this subsection plus such additional tax on the amount by which the turn‐over is in excess of ₦500,000 at a rate which shall be 50 per cent of the rate used in paragraph (a) (iv) of this subsection.

(3) In the case of an asset in respect of which an allowance has been granted before the commencement of this sub‐paragraph, an allowance shall be made in respect of the asset for the number of years which, if added to the number of years of assessment for which allowance has already been made, equals the number of years of assessment for which allowance is to be made under the provisions of sub‐paragraph (1) of this paragraph:

Provided that if an allowance has been made for a number of years which is equal to or more than the number of years specified under sub‐paragraph (1) of this paragraph, a single allowance shall be made for an amount which is N10 less than the residue of the qualifying expenditure for the year of assessment in which this sub‐paragraph takes effect.


```

Did you find all three?

