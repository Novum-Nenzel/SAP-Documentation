# Overview

This document contains the documentation for the steps of the Hitachi Data Connector for SAP. With
them you are able to connect to SAP systems and extract data into Pentaho PDI. The steps are:
<list type="bullet">
    <li>SAP BW/ERP RFC Executor Step</li>
    <li>SAP BW DSO Step</li> 
    <li>SAP ERP Table Input Step</li>
    <li>SAP Query Input Step</li>
    <li>Sap Report Input</li>
    <li>Sap ODP Extractor</li>
</list>
<p>The most universal step is the SAP BW/ERP RFC Executor Step who deals with Remote Function Calls
        (RFC) and provides high functionality. For more special cases the SAP BW DSO Step allows you to work
        with Data Store Objects (DSO). The SAP ERP Table Input Step gives access to the tables of a specified
        database connection. The SAP Query Input Step allows you to extract data from SAP-Queries. Data from
        the SAP system is provided in PDI in various formats, e.g. SAP table equivalent or as a String in JSON
        format.
</p>
<p>
After the explanation of how to install the steps, a description of the individual steps and their
functionalities and options follows.
</p>