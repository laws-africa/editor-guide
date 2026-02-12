# Tanzania

## Importing the HTML documents

**NB: Use the HTML files to import and for reference when cleaning up the imports.**

HTML files are saved here:<br>

[https://drive.google.com/drive/folders/13Qx11isfHmciPjCQOAhIhNis7vS6H3E1?usp=share\_link](https://drive.google.com/drive/folders/13Qx11isfHmciPjCQOAhIhNis7vS6H3E1?usp=share_link)

## Cleaning up the import - 2002 consolidation

### Things to look out for in Tanzania

#### Importing&#x20;

Import the HTML file whose number corresponds with the Chapter number of the Act. For instance, the HTML file for Arbitration Act (Chapter 15) is numbered "15.html" in the 2002 Consolidation-Principal Acts-HTML files folder.

<figure><img src="../.gitbook/assets/image (290).png" alt=""><figcaption><p>An example of how the Act is referenced in drive is captured in the image below.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (293).png" alt=""><figcaption></figcaption></figure>

When importing Swahili HTML files, the language (Swahili) must be selected as demonstrated in the image captured below.

<figure><img src="../.gitbook/assets/image (292).png" alt=""><figcaption></figcaption></figure>

#### Legislation history

References to legislation history, as highlighted in the image below, must be captured in a single annotation above the LONGTITLE. Each reference should be separated by a semi-colon.

<figure><img src="../.gitbook/assets/image (288).png" alt=""><figcaption><p>An example of how to mark up the text in this image is captured below. </p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (289).png" alt=""><figcaption></figcaption></figure>

#### Footnotes

The asterisks (\*) used to denote the footnotes should be deleted. Only numbers should be retained.

<figure><img src="../.gitbook/assets/image (294).png" alt=""><figcaption><p>An example of how to mark up the text is captured in the image captured below.</p></figcaption></figure>

In view mode

<figure><img src="../.gitbook/assets/image (296).png" alt=""><figcaption></figcaption></figure>

In edit mode

<figure><img src="../.gitbook/assets/image (297).png" alt=""><figcaption></figcaption></figure>

For references in the Schedule heading: change “s.” to “Section”

## Cleaning up import (where Gazettes are available)

### Things to look out for in Tanzania

#### Margin references

The references and date that appear alongside/under the Long Title of the Act must be deleted. The images of the logo that appear in the pdf must be removed. This has already been done in the Word docs, if you see any that have accidently been left in, please remove them.

The margin references in the pdfs have been moved into the body of the Act in the  Word docs. \
These references must be  in `{{*[annotation markup]}}`.

Using the pdf as reference, check that they have been placed correctly by following these instructions:

* if the reference/s appear directly under the section heading in the margin of the pdf they apply to that entire section, so should be positioned right at the end of that section.

![](<../.gitbook/assets/image (127).png>)

* if the reference/s appear alongside a specific subsection, paragraph etc, place them under that subsection, paragraph, etc

![](<../.gitbook/assets/image (244).png>)

* another example

<div align="center"><img src="../.gitbook/assets/image (186).png" alt=""></div>

This is how it will look on the platform, **please take note of how the references are indented**:

In view mode

![](<../.gitbook/assets/image (210).png>)

In edit mode

UPDATE SCREENSHOT

![](<../.gitbook/assets/image (107).png>)



If there is a string of references in one margin note in the pdf, like this:

![](<../.gitbook/assets/image (214).png>)

Please string them together, like this: `{{*[Acts Nos. 2 of 2010 s. 19; 13 of 2017 s. 4]}}`

So, full stop after "No." or "Nos." and spaces between "s." or "ss." and their corresponding numbers. Use a semi-colon to separate the Acts in the list.

Full stop after Ord. and Ords.\
`{{*[Ords. Nos. 45 of 1947 s. 3; 20 of 1958 s.2]}}`

For G.Ns place full stop after the N, like this:\
`{{*[G.N.s Nos. 478 of 1962; 64 of 1966]}}`

Cap. references are inconsistent in pdf - sometimes there is a space between the full stop and the number and sometimes no space. Please insert a space if there isn't one. Also, sometimes Cap has a full stop and sometime not, please give all a full stop after Cap. so that all of the Cap. references look like this:\
`{{*[Cap. 113]}}`

#### Missing spaces

If there are spaces missing in the references in margin notes, please insert them. Example:

![](<../.gitbook/assets/image (181).png>)

Should look like this:\
`{{*[G.N. No. 41 of 1992]}}`

and&#x20;

`{{*[Acts Nos 2 of 2010 s.19 13 of 2017 s.4]}}`

Should look like this: `{{*[Acts Nos. 2 of 2010 s. 19; 13 of 2017 s. 4]}}`

## Subsidiary legislation

**Subsidiary legislation** which sometimes appears after an Act is not to be included in the import of a document, please remove if it is there.<br>
