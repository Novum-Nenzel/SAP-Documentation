# Create and configure an RFC Destination

The following steps describe the settings and configurations:

1. TCP/IP Connection (RFC destination of type T) must be created. Use SAP transaction sm59 and create a new TCP/IP connection. After naming the connection as you like, define in the “Technical Settings” tab Program ID (capitals!), *Gateway Host*, and *Gateway service*. The Program ID is the name to be called when the step makes client requests to this RFC. Make sure the correct Activation Type is set (*Registered Server Program*). Besides that, the communication type must be set to Unicode in the “Unicode” tab. The rest of the settings can remain default.

   ![5.2.2.1](Image-5.2.2.1.png)
   ![5.2.2.2](Image-5.2.2.2.png)

   Then the Transfer Protocol in the “Special Options” tab must be adapted to "Classic with tRCF”.

   ![5.2.2.3](Image-5.2.2.3.png)

   In the standard SAP system, if tRFC errors occur, a background job is generated to reestablish the connection. To cancel a background job if tRFC errors occur, choose from the menu Edit -> tRFC options.

   ![5.2.2.4](Image-5.2.2.4.png)

   In the “Suppress background job if conn.error” field, enter the value X, and then click Continue.

   ![5.2.2.5](Image-5.2.2.5.png)

2. To allow the registration of external server programs, use transaction rz11. Search for Parameter gw/acl_mode and change, if it isn’t, Parameter Value to 0 (instead of default value 1).

3. At this point, some file adjustments of the ACL files have to be made, especially of secinfo. This file is used to prevent unauthorized launching of external programs. To access and edit this file, use the gateway monitor (transaction smgw).

   From there, go via “Goto -> Expert Functions -> External Security -> Maintenance of ACL Files”. Here you can check and config the file and add the rule for the Program ID of the destination. You have to create a new line in secinfo file with P (Permit), Program ID of the server (capitals!) and user & host.

   ![5.2.2.6](Image-5.2.2.6.png)
   >For more detailed information about the gateway security files, see in [SAP Documentation](https://help.sap.com/saphelp_nw73/helpdata/en/e2/16d0427a2440fc8bfc25e786b8e11c/frameset.htm).
   >
   >{style="note"}
