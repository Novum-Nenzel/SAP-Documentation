# Installation of transport package

The IT-Novum packages contains some customized functions, programs and types that have to be installed at the SAP system.

ZITN_BASIC Transport Package
<table>
    <tr>
        <td>Function Module</td>
        <td>Description</td>
    </tr>
    <tr>
        <td>Z_ITN_RFC_GET_TCPIP_DEST</td>
        <td>The list of TCP/IP destinations with registered server program.</td>
    </tr>
    <tr>
        <td>Z_ITN_QOUT_HAS_ERROR_QUEUES</td>
        <td>Checks queues with errors that are blocked because of one of the following error messages: SYSFAIL, CPICERR, RETRY, ARETRY, ANORETRY.</td>
    </tr>

</table>

ZITN_BASIC Transport Package
<table>
    <tr>
        <td>Function Module</td>
        <td>Description</td>
    </tr>
    <tr>
        <td>Z_ITN_QRFC_READ_TABLE_JOB</td>
        <td>Starts table data stream in background job.</td>
    </tr>
    <tr>
        <td>Z_ITN_QRFC_READ_TABLE</td>
        <td>Extracts table data via queued RFC.</td>
    </tr>

</table>

ZITN_RSDRI Transport Package
<table>
    <tr>
        <td>Function Module</td>
        <td>Description</td>
    </tr>
    <tr>
        <td>Z_RSDRI_INFOPROV_READ_RFC</td>
        <td>Starts InfoProvider data stream via RFC.</td>
    </tr>
    <tr>
        <td>Z_RSDRI_INFOPROV_READ_SERVICE</td>
        <td>Extracts data from InfoProvider via queued RFC.</td>
    </tr>

</table>

To use BW DSO Input step in server mode the transports ZITN_BASIC and ZITN_RSDRI has to be installed. When reading table data by server mode, ZITN_BASIC and ZITN_SDTI has to be installed.

Therefore unzip the transport package and copy the transport files to the location for the transport files on the SAP system. For the file transfer you can use ftp, FTP client tools like WinSCP or transaction CG3Z.
Then use the SAP transport management system (transaction STMS) to import the transport request.
