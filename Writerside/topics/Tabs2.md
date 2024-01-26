# Tabs

<b>General</b>

<img src="Image-7.3.3.png" alt="7.3.3"/>

The General tab provides the field table, a list of the fields from the current table. You can see the Name, the <emphasis> Key field</emphasis> , the <emphasis> SAP-DataType</emphasis> , the <emphasis> PDI-DataType</emphasis> , the  <emphasis> Length</emphasis> and the <emphasis> Description</emphasis> for each field. <emphasis> Convert</emphasis> shows whether the datatype is passed as a string into PDI. Also three Buttons can be found:

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
    <td>Convert Yes</td>
    <td>Convert the data type of every field into Java-Types which are used in PDI.</td>
    </tr>
    <tr>
    <td>Convert No</td>
    <td>The type of any field will be not converted.</td>
    </tr>
</table>

>Note: You can also decide individually for each field how you want to proceed with the conversion by using the dropdown menu.
>
{style="note"}

<control>Advanced</control>

<img src="Image-7.3.3.2.png" alt="7.3.3.2"/>

<table>
    <tr>
    <td>Option</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Batch Size</td>
    <td>Enter the number of rows you want to get within a batch per call. The default value is 5000.</td>
    </tr>
    <tr>
    <td>Load data in parallel?</td>
    <td>If activated, the step uses multithreading to read data from ERP system.</td>
    </tr>
    <tr>
    <td>Row limit</td>
    <td>The maximum number of records to be extracted. 0 is unlimited.</td>
    </tr>
    <tr>
    <td>Skip rows</td>
    <td>The number of rows in the table to ignore prior to extracting the first record. 
    By default, the first row is started (Index 0).
    </td>
    </tr>
</table>

<control>Filter</control>

<img src="Image-7.3.3.3.png" alt="7.3.3.3"/>

The filter tab allows to set a filter on SAP-Database level. The entered query is displayed above and the condition is executed on SAP-System side.

<control>Limitations</control>

Loading very large or wide tables can result in a performance decrease as database pointers cannot be maintained by SAP when running in client RFC mode. For loading very large tables consider using Server Mode.

<control>Server Mode</control>

<img src="Image-7.3.3.4.png" alt="7.3.3.4"/>

The Server Mode is considered for bulk loading very large (100M+) SAP tables and provides the currently best performance by exposing an ABAP Remote-RFC Endpoint to the SAP System and triggering a custom function at the SAP System to send the data to the RFC Endpoint (PDI/BA Sever).

Loading data this way allows SAP to maintain pointers and run the extraction process in the same thread ensuring constant performance even with very large tables.

<table>
    <tr>
    <td>Option</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Run in Server Mode</td>
    <td>If activated, the steps runs in Server Mode. As long as it’s activated the following options from the Advanced tab are no longer available:
    <emphasis> Load data in parallel, Row limit and Skip rows.</emphasis>
    </td>
    </tr>
    <tr>
    <td>RFC Destination</td>
    <td>The Destination where the result will be sent to. Has to be the Destination of the SAP Server.</td>
    </tr>
    <tr>
    <td>Search Destination</td>
    <td>Search for configured transactional RFC (tRFC) destinations on SAP System.</td>
    </tr>
    <tr>
    <td>Program ID</td>
    <td>Program ID for registering and identifying the JCoServer at the gateway.</td>
    </tr>
    <tr>
    <td>Gateway host</td>
    <td>Gateway host on which the server should be registered.</td>
    </tr>
    <tr>
    <td>Gateway service</td>
    <td>Gateway service to be used for registering at the gateway.
    This can either be a symbolic service name or a port number.
    </td>
    </tr>
    <tr>
    <td>Connection Count</td>
    <td>The number of server connections to register at the gateway</td>
    </tr>
    <tr>
    <td>Minimum thread count</td>
    <td>The minimum number of worker threads used by the JCoServer.
    If not set, the number of server connections (the connection count) is used as the minimum number of worker threads.
    </td>
    </tr>
    <tr>
    <td>Maximum thread count</td>
    <td>The maximum number of worker threads used by the JCoServer.
    If not set, the number of server connections (the connection count) is used as the maximum number of worker threads.
    </td>
    </tr>
    <tr>
    <td>Enable connection pooling</td>
    <td>Configuration of connection pooling</td>
    </tr>
    <tr>
    <td>Connection pool capacity</td>
    <td>Maximum number of idle connections kept open by the destination.</td>
    </tr>
    <tr>
    <td>Connection peak limit</td>
    <td>Maximum number of active connections that can be created for a destination simultaneously.</td>
    </tr>
    <tr>
    <td>Connection expiration time</td>
    <td>Time in ms after that a free connections hold internally by the destination can be closed.</td>
    </tr>
    <tr>
    <td>Connection expiration period</td>
    <td>Period in ms after that the destination checks the released connections for expiration.</td>
    </tr>
    <tr>
    <td>Connection timeout</td>
    <td>Max time in ms to wait for a connection, if the max allowed number of connections is allocated by the application.</td>
    </tr>
    <tr>
    <td>Check pooled connections</td>
    <td>If enabled, the pool checks for corrupted connections before they are used by an application.</td>
    </tr>
</table>