# Rwanda

## Documents for import

Word documents: [https://drive.google.com/drive/folders/1BMk\_kPxg7eEt3HGL-tICcWuwSHPiLGVy?usp=sharing](https://drive.google.com/drive/folders/1BMk\_kPxg7eEt3HGL-tICcWuwSHPiLGVy?usp=sharing)

PDF documents: [https://drive.google.com/drive/folders/1O9iigIOJteEp\_XZ2EoVicpUjG0nU0bcP?usp=sharing](https://drive.google.com/drive/folders/1O9iigIOJteEp\_XZ2EoVicpUjG0nU0bcP?usp=sharing)



## Cleaning up the import

### PDF documents

All PDF documents have 3 languages, Kinyarwanda, English and French. The French and Kinyarwanda text has been removed from the converted word documents, leaving only the English.

### Heading and tables of contents

Please do not import the text that appears at the top of the first page of each document. The table of contents should also not be imported.

<figure><img src="../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Preface and Preamble

The text highlighted in the image below should be marked under the PREFACE.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1).png" alt=""><figcaption><p>Highlighted text should be marked up under the PREFACE.</p></figcaption></figure>

The text highlighted in the image below should be marked under the PREAMBLE.

<figure><img src="../.gitbook/assets/image (2) (1) (1).png" alt=""><figcaption><p>Highlighted text should be marked up under the PREAMBLE.</p></figcaption></figure>

#### PREFACE and PREAMBLE markup example

<pre class="language-html" data-line-numbers data-full-width="true"><code class="lang-html">PREFACE
    **We, KAGAME Paul,**
    President of the Republic;
    
    **THE PARLIAMENT HAS ADOPTED AND WE SANCTION, PROMULGATE THE FOLLOWING LAW AND ORDER IT BE
    PUBLISHED IN THE OFFICIAL GAZETTE OF THE REPUBLIC OF RWANDA**
    
PREAMBLE
    **THE PARLIAMENT:**

    The Chamber of Deputies, in its session of 2 May 2018;
<strong>
</strong><strong>    Pursuant to the Constitution of the Republic of Rwanda of 2003 revised in 2015, especially Articles 64, 69, 70, 88, 91, 106, 120 and 176;
</strong>
<strong>    Having reviewed Law n° 19/2008 of 14/07/2008 on characteristics and ceremonies of the National Anthem as amended to date;
</strong>
    **ADOPTS:**
</code></pre>





### Date and signatories

The date and signatories at the bottom of each document should be excluded from the import.&#x20;

<figure><img src="../.gitbook/assets/image (3) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Elements

Below are some keywords you will encounter in marking up elements, indented correctly.

{% code lineNumbers="true" %}
```html
CHAPTER
    SECTION
        ARTICLE
            ITEMS
                ITEM 1º
                TTEM 2º
                ITEM 3º
```
{% endcode %}



<figure><img src="../.gitbook/assets/image (3) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>
