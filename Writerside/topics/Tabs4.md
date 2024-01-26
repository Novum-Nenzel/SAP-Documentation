# Tabs

<control>General</control>

<img src="Image-7.5.3.png" alt="7.5.3"/>

<table>
    <tr>
    <td>Button</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Edit selections</td>
    <td>Opens the dialog to define the selections manually.</td>
    </tr>
    <tr>
    <td>Get variant selections</td>
    <td>Loads the selections of a variant.</td>
    </tr>
    <tr>
    <td>Get fields</td>
    <td>Opens the dialog to define the fields of the report.</td>
    </tr>
</table>

To limit the output of a report you can select a variant or define a selection. If the manual selections are defined, they overwrite all selections in the variant.

<img src="Image-7.5.3.2.png" alt="7.5.3.2"/>

<table>
    <tr>
    <td>Column</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Sign</td>
    <td>The column “Sing” determines whether the result of the condition is includes or excluded in the result set.</td>
    </tr>
    <tr>
    <td>Selection option</td>
    <td>The column “Select Option” defines an operator.
    <control>EQ</control>(Equals), <control>NE</control>(Not Equals), <control>GT</control>(Greater Than), <control>LT</control>(Less Than), 
    <control>BT</control>(Between), <control>NB</control>(Not Between), <control>CP</control>(Matches Pattern), 
    <control>GR</control>(Greater Than Or Equal To), <control>LE</control>(Less Than Or Equal To), 
    <control>NP</control>(Not Matches Pattern)
    </td>
    </tr>
    <tr>
    <td>Low Value</td>
    <td>This column is designated for the comparison value or the lower interval limitation.</td>
    </tr>
    <tr>
    <td>High Value</td>
    <td>This column is designated for the upper interval limitation. High value only has to be filled in if the “Select option” is “Between” or “Nor Between”.</td>
    </tr>
</table>

<control>Fields dialog</control>

To identify the report fields, the report based on the selected variant or selections needs to be executed. The report output (spool list) is displayed in the "Spool request preview" section.

<img src="image-7.5.3.3.png" alt="7.5.3.3."/>

In the most ABAP reports the output fields are delimited by the pipe symbol “|”. In this case, fields can be defined automatically by clicking the "Generate" button in the "Fields" section.

If automatic field detection is not possible, field name, field length and offset must be defined manually.

<table>
    <tr>
    <td>Option</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Report rows per data row
    </td>
    <td>Concatenates the two or more report rows into a data row. 
    The default value is 1 row.
    </td>
    </tr>
    <tr>
    <td>Skip rows from spool top</td>
    <td>The number of rows to skip at the beginning of the report. This option allows skipping the possible meta information in the header section of the report.</td>
    </tr>
    <tr>
    <td>Skip rows from spool page top</td>
    <td>A spool list of a report contains one or more pages. This option allows you to specify the number of rows to skip at the beginning of the spool page.</td>
    </tr>
    <tr>
    <td>Skip rows from spool page bottom</td>
    <td>The number of rows to skip in the footer section of the spool page.</td>
    </tr>
</table>

<control>Advanced</control>

<img src="Image-7.5.3.4.png" alt="7.5.3.4"/>

<table>
    <tr>
    <td>Option</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Job name</td>
    <td>The name of a background job.</td>
    </tr>
    <tr>
    <td>Time out</td>
    <td>The timeout for waiting for the batch job execution in milliseconds.</td>
    </tr>
    <tr>
    <td>Ignore errors</td>
    <td>Ignore execution errors that occur and log information about the errors.</td>
    </tr>
    <tr>
    <td>Spool page count</td>
    <td>The number of spool pages in a batch.</td>
    </tr>
    <tr>
    <td>Report rows per data row
    </td>
    <td>Concatenates the two or more report rows into a data row. 
    The default value is 1 row.
    </td>
    </tr>
    <tr>
    <td>Skip rows from spool top</td>
    <td>The number of rows to skip at the beginning of the spool.</td>
    </tr>
    <tr>
    <td>Skip rows from spool page top</td>
    <td>The number of rows to skip at the beginning of the spool page.</td>
    </tr>
    <tr>
    <td>Skip rows from spool page bottom</td>
    <td>The number of rows to skip in the footer section of the spool page.</td>
    </tr>
</table>