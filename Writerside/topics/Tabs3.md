# Tabs

<control>Fields</control>

<img src="Image-7.4.3.png" alt="7.4.3"/>

<table>
    <tr>
    <td>Button</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Get Fields</td>
    <td>Click to retrieve a list of all fields coming in on the stream. It’s possible to sort or delete fields.</td>
    </tr>
    <tr>
    <td>Convert Yes</td>
    <td>Convert Yes	Convert the datatype of every field into Java-Types which are used in PDI.</td>
    </tr>
    <tr>
    <td>Convert No</td>
    <td>The type of any field will be not converted.</td>
    </tr>
</table>

> Note: You can also decide individually for each field how you want to proceed with the conversion by using the dropdown menu.
> 
{style="note"}

<control>Select Options </control>

<img src="Image-7.4.3.2.png" alt="7.4.3.2"/>

<table>
    <tr>
    <td>Button</td>
    <td>Descriotion</td>
    </tr>
    <tr>
    <td>Edit Selections</td>
    <td>Opens the dialog to define the selection for the parameters</td>
    </tr>
</table>

In the "Selection criteria" dialog it is also possible to choose selections to create a variant.

<img src="Image-7.4.3.3.png" alt="7.4.3.3"/>

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

<control>Advanced</control>

<img src="Image-7.4.3.4.png" alt="7.4.3.4"/>

<table>
    <tr>
    <td>Option</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Row limit</td>
    <td>The maximum number of records to be extracted. 0 means unlimited.</td>
    </tr>
    <tr>
    <td>Ignore Errors</td>
    <td>Defines whether an error should be triggered if the query contains no data.</td>
    </tr>
</table>


