# Create and configure a RFC Destination

The following steps describe the settings and configurations:


<list type="decimal">
<li>TCP/IP Connection (RFC destination of type T) must be created
Use SAP transaction sm59 and create a new TCP/IP connection. After naming the connecting as you like, define in the “Technical Settings” tab Program ID (capitals!),<emphasis> Gateway Host</emphasis>  and <emphasis> Gateway service</emphasis>. The Program ID is the name to be called when the step made client requests to this RFC. Make sure the correct Activation Type is set (<emphasis> Registered Server Program</emphasis>).

Besides that communication type must be set to Unicode in the “Unicode” tab. The rest of the settings can remain default.

<img src="Image-5.2.2.1.png"  alt="5.2.2.1"/>
<img src="Image-5.2.2.2.png"  alt="5.2.2.2"/>

Then the Transfer Protocol in the “Special Options” tab must be adapted to
"Classic with tRCF”.
<img src="Image-5.2.2.3.png" alt="5.2.2.3"/>

In the standard SAP system, if tRFC errors occur, a background job is generated to reestablish the connection. To cancel a background job if tRFC errors occur choose from menu Edit-tRFC options.
<img src="Image-5.2.2.4.png" alt="5.2.2.4"/>

In the “Suppress background job if conn.error” field, enter the value X, and then click Continue.
<img src="Image-5.2.2.5.png" alt="5.2.2.5"/>
</li>
<li>
    To allow the registration of external server programs use transaction rz11. Search for Parameter gw/acl_mode and change, if it isn’t, Parameter Value to 0 (instead of default value 1).
</li>
<li>
At this point some file adjustments of the ACL files have to be made, especially of secinfo. This file is used to prevent unauthorized launching of external programs. To access and edit this file, use the gateway monitor (transaction smgw).

From there, go via “Goto -> Expert Functions -> External Security -> Maintenance of ACL Files”.
Here you can check and config the file and add the rule for the Program ID of the destination. You have to create a new line in secinfo file with P (Permit), Program ID of the server (capitals!) and user & host.

<img src="Image-5.2.2.6.png" alt="5.2.2.6"/>
>For more detailed information about the gateway security files see in <a href="https://help.sap.com/saphelp_nw73/helpdata/en/e2/16d0427a2440fc8bfc25e786b8e11c/frameset.htm">SAP Documentation:</a>
>
{style="note"}
</li>
</list>