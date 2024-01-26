# Tabs

<control> Fields </control>

<img src="Image-7.6.3.png" alt="7.6.3"/>

<table>
    <tr>
    <td>Button</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Get Fields</td>
    <td>Click to retrieve a list of all fields coming in on the stream.</td>
    </tr>
    <tr>
    <td>Edit Selections</td>
    <td>Opens the dialog to define the selection for the fields.</td>
    </tr>
</table>

<img src="Image-7.6.3.2.png" alt="7.6.3.2"/>

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
<control>BT</control>(Between), <control>NB</control>(Not Between),  <control>GR</control>(Greater Than Or Equal To), 
<control>LE</control>(Less Than Or Equal To)
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

<img src="Image-7.6.3.3.png" alt="7.6.3.3"/>

<table>
    <tr>
    <td>Option</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Full</td>
    <td>Extracts all available data.</td>
    </tr>
    <tr>
    <td>Delta</td>
    <td>Extracts delta data if a subscription is available for the subscriber. If no subscription exists for the subscriber, a delta initialization is performed.

This option is only for ODP providers available that support delta extraction.
</td>
    </tr>
    <tr>
    <td>Extract data</td>
    <td>Extract data during delta initialization.</td>
    </tr>
    <tr>
    <td>Reset subscription</td>
    <td>Automatically resets existing delta subscription and creates a new one.</td>
    </tr>
    <tr>
    <td>Package size</td>
    <td>Package size in megabytes. The default value is 50.</td>
    </tr>
    <tr>
    <td>Delta subscription</td>
    <td>Opens the dialog to display details about active subscribers.</td>
    </tr>
</table>

<control>Delta subscriptions dialog </control>

<img src="Image-7.6.3.4.png" alt="7.6.3.4"/>

<table>
    <tr>
    <td>Column</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Subscription</td>
    <td>Subscription name.</td>
    </tr>
    <tr>
    <td>Name</td>
    <td>ODP provider name.</td>
    </tr>
    <tr>
    <td>Context</td>
    <td>ODP provider context.</td>
    </tr>
    <tr>
    <td>Requests</td>
    <td>Number of executed delta requests.</td>
    </tr>
    <tr>
    <td>Last request</td>
    <td>Timestamp of the last request.</td>
    </tr>
</table>
