# Tabs

<b>General</b>

<img src="Image-7.2.3.png" alt="7.2.3.1"/>

The General tab provides the field table, splitted in Characteristics and Key Figures. For each you get the fields Name of  <emphasis>InfoObject</emphasis>, <emphasis>SAP DataType</emphasis> and <emphasis>Description</emphasis>.

By using the button Get Fields you retrieve a list of all fields coming in on the stream. It’s possible to sort or delete fields.

<b>Server Mode</b>

<img src="Image-7.2.3.2.png" alt="7.2.3.2"/>

The Server Mode is considered for bulk loading very large InfoProviders, such as very large DSOs, and provides the currently best performance by exposing a ABAP Remote-RFC Endpoint to the SAP System and triggering a custom function at the SAP System to send the data to the RFC Endpoint (PDI/BA Sever).

Loading data this way allows SAP to maintain pointers and run the extraction process in the same thread ensuring constant performance even with very large tables.

<table>
    <tr>
    <td>Option</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>Run in Server Mode</td>
    <td>If activated, the step runs in Server Mode.</td>
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
    <td>Package size</td>
    <td>Number of rows to get within a batch per call. The default value is 5000.</td>
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