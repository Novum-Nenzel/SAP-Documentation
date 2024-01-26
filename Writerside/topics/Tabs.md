# Tabs

<b>General</b>

<img src="Image-7.1.3.png" alt="7.1.3"/>

The general tab provides options and separate Context Settings.

<table>
    <tr>
    <td>Option</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Source from previous step</td>
    <td>If enabled, the step deals with incoming parameters as rows
    <list type="bullet">
    <li><control> Parameters:</control> Choose the column with the import parameters
    </li>
    <li><control> Table Parameters:</control> Choose the column with the table parameters
    </li>
    </list>
    </td>
    </tr>
    <tr>
    <td>Pass fields to output	
    </td>
    <td>If enabled, the parameters retrieves from the RFC calls get passed to the stream so the following steps can work with them. You can name the fields below: 
        <list type="bullet">
        <li><control> Import Parameters:</control> The import parameter from the SAP database
        </li>
        <li><control> Table Parameters:</control> The table parameter from the SAP database
        </li>
        <li><control> Export Parameters:</control> The export parameter from the SAP database
        </li>
        </list>
    </td>
    </tr>
</table>

<b> BAPIs in a context </b> 

All RFC Executor Steps have to be ordered one after the other as you see in screenshot below. Each step must configure the respective BAPI: set the Import Parameter and, if available, the Table Parameter.

The steps that run within a context have to configure a common context name and mark the checkbox “Run in context”. The last step marks the checkbox “Execute context” as well. The results of the function which you want further to use can selected by the column box “Result from previous function”.

Pass Parameters to stream is deactivated, when “Run in context” is selected and is available again when “Execute in context” is marked.

<img src="Image-7.1.3.2.png" alt="7.1.3.2"/>

<b>Context settings</b> 

<table>
    <tr>
    <td>Context settings</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Run in context</td>
    <td>If enabled, the step run in context</td>
    </tr>
    <tr>
    <td>Execute context</td>
    <td>If enabled, all steps with the same context will be executed.</td>
    </tr>
    <tr>
    <td>Context name</td>
    <td>Name of the SAP context the steps running at.</td>
    </tr>
    <tr>
    <td>Result from previous function</td>
    <td>Select the previous function from which the result comes.</td>
    </tr>
</table>

<b>Fields</b> 

<img src="Image-7.1.3.3.png" alt="7.1.3.3"/>

<table>
    <tr>
    <td>Column</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Field</td>
    <td>The SAP field, sort by Import Parameter, Table Parameter and Export Parameter.</td>
    </tr>
    <tr>
    <td>Type</td>
    <td>SAP data type.</td>
    </tr>
    <tr>
    <td>Value</td>
    <td>The editable value of the field. You can add filter, set import parameter etc.</td>
    </tr>
    <tr>
    <td>Optional</td>
    <td>Shows whether the field is optional.</td>
    </tr>
</table>

<table>
    <tr>
    <td>Button</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Add</td>
    <td>Add rows to a table inside parameter (if parameter is structure). If you want to set values use this button to get the change point.</td>
    </tr>
   <tr>
    <td>Delete</td>
    <td>Remove rows from the parameter table.</td>
    </tr>
</table>