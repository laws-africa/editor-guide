# Bulk imports \(spreadsheet\)

The spreadsheet has the following columns:

<table>
  <thead>
    <tr>
      <th style="text-align:left">Column</th>
      <th style="text-align:left">Description</th>
      <th style="text-align:left">Examples</th>
      <th style="text-align:left">Notes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b>Core details</b>
      </td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left">Used for working out the FRBR URI (unique identifier)
        <br />Most fields are mandatory</td>
    </tr>
    <tr>
      <td style="text-align:left">country</td>
      <td style="text-align:left">2-letter country code</td>
      <td style="text-align:left">ZA for South Africa, KE for Kenya</td>
      <td style="text-align:left">Case insensitive
        <br />Must be the same code as the country you&apos;re in on the platform</td>
    </tr>
    <tr>
      <td style="text-align:left">locality</td>
      <td style="text-align:left">locality code</td>
      <td style="text-align:left">cpt for Cape Town in South Africa</td>
      <td style="text-align:left">Leave blank for national legislation
        <br />Case insensitive
        <br />Must be the same code as the locality you&apos;re in on the platform
        <a
        href="https://en.wikipedia.org/wiki/List_of_municipalities_in_South_Africa">
          <br />
          </a><a href="https://en.wikipedia.org/wiki/List_of_municipalities_in_South_Africa">ZA municipalities on Wikipedia</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">title</td>
      <td style="text-align:left">The short title of the work</td>
      <td style="text-align:left">Criminal Procedure Act</td>
      <td style="text-align:left">May or may not include the year at the end &#x2013; house style decision</td>
    </tr>
    <tr>
      <td style="text-align:left">cap</td>
      <td style="text-align:left">Chapter (Cap.) number</td>
      <td style="text-align:left">12 for Chapter 12</td>
      <td style="text-align:left">Not all countries use Chapter numbers</td>
    </tr>
    <tr>
      <td style="text-align:left">doctype</td>
      <td style="text-align:left">The code for the work&apos;s type</td>
      <td style="text-align:left">act, statement</td>
      <td style="text-align:left">In most places the default is &apos;act&apos;, and this column can be
        ignored</td>
    </tr>
    <tr>
      <td style="text-align:left">subtype</td>
      <td style="text-align:left">The code for the work&apos;s subtype</td>
      <td style="text-align:left">ln for a Legal Notice, by-law for a By-law, p for a Proclamation, si for
        a Statutory Instrument</td>
      <td style="text-align:left">Case insensitive
        <br />Leave blank for Acts</td>
    </tr>
    <tr>
      <td style="text-align:left">actor</td>
      <td style="text-align:left">A code decided on internally for the author of a work</td>
      <td style="text-align:left">mepc</td>
      <td style="text-align:left">
        <p>No spaces allowed</p>
        <p>Can mostly be ignored</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">number</td>
      <td style="text-align:left">The number of the work</td>
      <td style="text-align:left">9 for Act 9 of 2012, 34 for SI 34 of 2012</td>
      <td style="text-align:left">Use words separated by hyphens for works without a number and by-laws</td>
    </tr>
    <tr>
      <td style="text-align:left">year</td>
      <td style="text-align:left">The year of the work</td>
      <td style="text-align:left">2012 for Act 9 of 2012</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Publication details</b>
      </td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left">Used to try and automatically link the relevant Gazette when creating
        the work on the platform</td>
    </tr>
    <tr>
      <td style="text-align:left">publication_name</td>
      <td style="text-align:left">Usually the name of the Gazette</td>
      <td style="text-align:left">Eastern Cape Provincial Gazette</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">publication_number</td>
      <td style="text-align:left">The Gazette number</td>
      <td style="text-align:left">12345 for Gazette 12345 of 1 March 2020</td>
      <td style="text-align:left">Found on front cover of Gazette</td>
    </tr>
    <tr>
      <td style="text-align:left">publication_date</td>
      <td style="text-align:left">The Gazette date</td>
      <td style="text-align:left">2020-03-01 for Gazette 12345 of 1 March 2020</td>
      <td style="text-align:left">Found on front cover of Gazette
        <br />Date format is yyyy-mm-dd
        <br />Typing in e.g. &apos;1 Mar 20&apos; should be automatically formatted
        by the spreadsheet</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Other relevant dates</b>
      </td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left">Date format is yyyy-mm-dd
        <br />Typing in e.g. &apos;1 Mar 20&apos; should be automatically formatted
        by the spreadsheet</td>
    </tr>
    <tr>
      <td style="text-align:left">assent_date</td>
      <td style="text-align:left">The date on which the work was signed by the relevant authority</td>
      <td
      style="text-align:left"></td>
        <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">commencement_date</td>
      <td style="text-align:left">The date on which the work came / will come into force</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">If the work has more than one commencement date, enter the main one here
        <br
        />
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Other info</b>
      </td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">stub</td>
      <td style="text-align:left">Mark this work as a stub, i.e. a work for which the content will not be
        pulled in</td>
      <td style="text-align:left">Commencement notices, amending works, repeal notices (works without substantive
        provisions)</td>
      <td style="text-align:left">Leave empty for principal works</td>
    </tr>
    <tr>
      <td style="text-align:left">taxonomy</td>
      <td style="text-align:left">Optional taxonomy tag/s to be applied to the work, separated by &apos;;&apos;s</td>
      <td
      style="text-align:left">lawsafrica-special:COVID-19 for the Laws.Africa Special Collection titled
        &apos;COVID-19&apos;</td>
        <td style="text-align:left">Choose an item from the dropdown
          <br />The taxonomy must exist on the platform first</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Passive relationships</b>
      </td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left">To select a work&apos;s FRBR URI from the dropdown, start typing its title
        in the cell and the list of options will shrink
        <br />There&apos;s no need to record both sides of a relationship in the spreadsheet;
        use the one that works best for your workflow</td>
    </tr>
    <tr>
      <td style="text-align:left">primary_work</td>
      <td style="text-align:left">The FRBR URI of this work&apos;s parent / primary work</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">Only use for subsidiary legislation (e.g. Regulations / SIs)</td>
    </tr>
    <tr>
      <td style="text-align:left">commenced_by</td>
      <td style="text-align:left">The FRBR URI of a work that commences this work</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">The commencing work will get its own row in the spreadsheet
        <br />Leave blank if the work commences itself (either on publication or at
        another date)</td>
    </tr>
    <tr>
      <td style="text-align:left">commenced_on_date</td>
      <td style="text-align:left">The date on which this work is commenced by the commencing work</td>
      <td
      style="text-align:left"></td>
        <td style="text-align:left">The commencing work will most often commence on publication, but may give
          a different commencement date for the work being commenced</td>
    </tr>
    <tr>
      <td style="text-align:left">amended_by</td>
      <td style="text-align:left">The FRBR URI of a work that amends this work</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">The amending work will get its own row in the spreadsheet</td>
    </tr>
    <tr>
      <td style="text-align:left">amended_on_date</td>
      <td style="text-align:left">The date on which this work is amended by the amending work</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">If nothing is given here, the commencement date of the amending work will
        be used (if it has one)</td>
    </tr>
    <tr>
      <td style="text-align:left">repealed_by</td>
      <td style="text-align:left">The FRBR URI of a work that repeals this work</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">The repealing work will get its own row in the spreadsheet</td>
    </tr>
    <tr>
      <td style="text-align:left">repealed_on_date</td>
      <td style="text-align:left">The date on which this work is repealed by the repealing work</td>
      <td
      style="text-align:left"></td>
        <td style="text-align:left">If nothing is given here, the commencement date of the repealing work
          will be used (if it has one)</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Active relationships</b>
      </td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left">To select a work&apos;s FRBR URI from the dropdown, start typing its title
        in the cell and the list of options will shrink
        <br />There&apos;s no need to record both sides of a relationship in the spreadsheet;
        use the one that works best for your workflow</td>
    </tr>
    <tr>
      <td style="text-align:left">subleg</td>
      <td style="text-align:left">The FRBR URI of this work&apos;s children / subsidiary works, separated
        by &apos;;&apos;s</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">commences</td>
      <td style="text-align:left">The FRBR URI of a work commenced by this work</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">The work being commenced will get its own row in the spreadsheet</td>
    </tr>
    <tr>
      <td style="text-align:left">commences_on_date</td>
      <td style="text-align:left">The date on which that work is commenced by this work</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">
        <p>The commencing work (this work) will most often commence on publication,
          but may give a different commencement date for the work being commenced</p>
        <p>If nothing is given here, the commencement date of this work will be used
          (if it has one)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">amends</td>
      <td style="text-align:left">The FRBR URI of a work amended by this work</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">The amended work will get its own row in the spreadsheet
        <br />If this work amends more than one work, duplicate this work&apos;s row
        as many times as needed, only changing this column (and the next one if
        relevant)</td>
    </tr>
    <tr>
      <td style="text-align:left">amends_on_date</td>
      <td style="text-align:left">The date on which that work is amended by this work</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">If nothing is given here, the commencement date of this work will be used
        (if it has one)</td>
    </tr>
    <tr>
      <td style="text-align:left">repeals</td>
      <td style="text-align:left">The FRBR URI of a work repealed by this work</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">The repealed work will get its own row in the spreadsheet
        <br />If this work repeals more than one work, duplicate this work&apos;s row
        as many times as needed, only changing this column (and the next one if
        relevant)</td>
    </tr>
    <tr>
      <td style="text-align:left">repeals_on_date</td>
      <td style="text-align:left">The date on which that work is repealed by this work</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">If nothing is given here, the commencement date of this work will be used
        (if it has one)</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Housekeeping</b>
      </td>
      <td style="text-align:left">&lt;b&gt;&lt;/b&gt;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Ignore</td>
      <td style="text-align:left">When doing a bulk import, put anything in this column and the importer
        will skip it. Putting a &#x2714; will make the cell green, to show it&apos;s
        been imported. Putting a &quot;?&quot; will make it yellow, to show research
        must still be done. It will be red as long as it&apos;s empty, to show
        it must still be imported.</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">
        <p>If a work already exists and is reimported (&apos;Ignore&apos; is left
          blank), it won&apos;t be overwritten on import and will be shown as a &apos;Duplicate&apos;,
          but the taxonomy and any relationships will be linked if they weren&apos;t
          linked previously</p>
        <p>If any other non-core details were corrected on the platform in the meantime,
          they should be updated on the spreadsheet before it&apos;s reimported</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">frbr_uri</td>
      <td style="text-align:left">A formula in this cell will generate the FRBR URI</td>
      <td style="text-align:left">/akn/za/act/2020/1 for Act 1 of 2020 in South Africa</td>
      <td style="text-align:left">Do not edit this cell
        <br />If it looks wrong, check the core details</td>
    </tr>
    <tr>
      <td style="text-align:left">frbr_uri_title</td>
      <td style="text-align:left">A formula in this cell will generate the FRBR URI followed by the title</td>
      <td
      style="text-align:left">/akn/za/act/2020/1 - Banking Act, 2020 for Act 1 of 2020 in South Africa</td>
        <td
        style="text-align:left">This populates the dropdown lists for all relationships</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Comments etc</b>
      </td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">comments</td>
      <td style="text-align:left">Text from this column and any others you add won&apos;t be imported; use
        them as a record for yourself</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">LINKS ETC (add columns as needed)</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>

