# Step and License Installation for PDI

<p>Requirements for the installation of the steps are:</p>
<list>
    <li>
    Any combination of (sap-tableinput-x.jar, sap-rfcexecutor-x.jar, sap-dsoinput-x.jar,
    sap-queryinput-x.jar, sap-reportinput-x.jar, sap-odp-extractor-x.jar)
    </li>
    <li>
    sap-shared-x.jar
    </li>
    <li>
    sap-server-x.jar
    </li>
    <li>
    license-manager-x.jar
    </li>
    </list>

<p>Additionally you need the sapjco3 libraries and for the license installation you also need the l4j license files.</p>

<list type="decimal">
<li>
    Go to the path of your Pentaho installation into the directory:
    <code-block lang="bash">
    …/design-tools/data-integration/plugins
    </code-block>
</li>
<li>
For every step jar archive (sap-tableinput-x.jar and sap-dsoinput-x.jar) you have to create a subdirectory with the following substructure:
<img src="Image-4.1.png" alt="4.1.1" width="200"/>
For every step jar archive (sap-rfcexecutor-x.jar, sap-queryinput-x.jar, sap-reportinput-x.jar and sap-odp-extractor-x.jar) you have to create a subdirectory with the following substructure:
<img src="Image-4.1.2.png" alt="4.1.2" width="200"/>
</li>
<li>
After you have created the structure, you need to copy the corresponding files to the correct location. These files are affected: sap-shared-x.jar, sap-server-x.jar, license-manager-x.jar, the sapjco3 libraries and the l4j license files.

For example, you have to copy the sap-dsoinput-x.jar into: 
<code-block lang="bash">…/sap_dsoinput</code-block>

For Linux or MacOS, instead of the sapjco3.dll you have to use the libsapjco3.so (Linux) or the libsapjco3.jnilib or libsapjco3.dylib (MacOS).

</li>
</list>


