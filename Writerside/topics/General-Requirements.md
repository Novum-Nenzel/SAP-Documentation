# General Requirements

>This list provides details about the environment components and versions we support.
>
{style="tip"}
<table>
        <tr>
            <td>System Component</td>
            <td>Description</td>
        </tr>
        <tr>
            <td>Pentaho Data Integration</td>
            <td>Pentaho Data Integration The connector supports PDI Version 7.x., 8.x and higher</td>
        </tr>
        <tr>
            <td>SAP</td>
            <td>The connector supports SAP ERP and SAP BW systems with possibility to connect via RFC (Remote Function
                Call)
            </td>
        </tr>
        <tr>
            <td>Operating System</td>
            <td>see Pentaho Component References</td>
        </tr>
        <tr>
            <td>SAP Java Connector</td>
            <td>Connection to SAP-Systems require the usage of SAP Java Connector. Therefore the following SAP Libraries are necessary:
                <list>
                    <li>
                        sapjco3.jar
                    </li>
                    <li>
                        sapjco3.dll (Windows)
                    </li>
                    <li>
                        libsapjco3.jnilib or libsapjco3.dylib (MacOS)
                    </li>
                    <li>
                        libsapjco3.so (Linux)
                    </li>
            </list>
            <p>
                The supported Operating Systems can be look up in the following SAP Note: SAP JCo 3.0 release and support strategy <a href="https://launchpad.support.sap.com/">(Note 1077727)</a> .
                The SAP JCo is available on the <a href="https://support.sap.com/en/product/connectors.html">Software Downloads Center</a>.
            </p>
            </td>
        </tr>
</table>

<b>
Configuring SAP User-Rights
</b>

In this section you will find some information about configuring SAP-Users to use the different Hitachi Data Connector for SAP types.

To use the Hitachi Data Connector read-rights for the following functions in SAP are needed:

<table>
    <tr>
        <td>Name</td>
        <td>SAP ERP TableInput</td>
        <td>SAP BW/ERP RFC-Executor</td>
        <td>SAP-BW DSOInput</td>
    </tr>
    <tr>
        <td>RFCPING</td>
        <td>X</td>
        <td>X</td>
        <td>X</td>
</tr>
    <tr>       
        <td>RFC_READ_TABLE</td>
        <td>X</td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>VIEW_AUTHORITY_CHECK</td>
        <td>X</td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>DDIF_TABL_GET</td>
        <td>X</td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>DD_TABL_GET</td>
        <td>X</td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>DD_INT_DD03P_ACCUMULATE</td>
        <td>X</td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>DB_GET_INDEXES</td>
        <td>X</td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>PRGN_CHECK_SYSTEM_TYPE</td>
        <td>X</td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>DDIF_FIELDINFO_GET</td>
        <td>X</td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>SCP_GET_LANGUAGE_ID</td>
        <td>X</td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>DD_INT_UPDATE_DDFTX</td>
        <td>X</td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>DDUT_DOMVALUES_GET</td>
        <td>X</td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>RS_EXCEPTION_TO_SYMSG</td>
        <td></td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>RS_EXCEPTION_TO_MESSAGE</td>
        <td></td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>RRSV_SYSTYPE_GET</td>
        <td></td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>RS_EXCEPTION_TEXT_TO_MESSAGE</td>
        <td></td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>RSDG_WORD_WRAP</td>
        <td></td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>TEXT_SPLIT</td>
        <td></td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>RS_EXCEPTION_CLEANUP</td>
        <td></td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>BAPI_ODSO_GETLIST</td>
        <td></td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>GROUP: RSAB</td>
        <td></td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>BAPI_ODSO_GETDETAIL</td>
        <td></td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>GROUP: RSAB</td>
        <td></td>
        <td>X</td>
        <td>X</td>
    </tr>
    <tr>        
        <td>RFC_FUNCTION_SEARCH</td>
        <td></td>
        <td>X</td>
        <td></td>
    </tr>
    <tr>        
        <td>FUNCTION_INCLUDE_CONCATENATE</td>
        <td></td>
        <td>X</td>
        <td></td>
    </tr>
    <tr>        
        <td>FUNCTION_INCLUDE_SPLIT</td>
        <td></td>
        <td>X</td>
        <td></td>
    </tr>
</table>
<!--
<img src="Image-5.1.png" alt="5.1.1" />
<img src="Image.5.1.2.png" alt="5.1.2"/>
<img src="Image.5.1.3.png" alt="5.1.3"/>
<img src="Image.5.1.4.png" alt="5.1.4"/>
<img src="Image.5.1.5.png" alt="5.1.5"/>
<img src="Image.5.1.6.png" alt="5.1.6"/>
-->
The following objects are required at least to use the Report step.

<img src="Image.5.1.7.png" alt="5.1.7"/>
