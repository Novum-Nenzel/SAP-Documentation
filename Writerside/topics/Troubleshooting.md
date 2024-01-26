# Troubleshooting

Below you can find a few possible issues that may arise when installing the steps and their solutions.

<b>The sapjco Library cannot be loaded</b>

Perhaps the sapjco3 library will not be loaded and you will get this or a similar error:

<code-block lang="bash">java.lang.UnsatisfiedLinkError: no sapjco3 in java.library.path</code-block>: 
In this case the sapjco3.jar is unable to find the sapjco3 JNI library (.dll | .so | .jnilib | .dylib). The JNI library file has to reside in the same directory as the sapjco3.jar. Or in a platform dependent sub-directory relative to the sapjco3.jar. Please refer to the SAP documentation for "Configuration and Requirements" in the "Runtime initialization" section.

<b>Linux Issues</b>

Using a Linux OS can lead to problems when assigning permissions. Make sure the steps have the same user rights as the other plugins. Pentaho creates its own user (pentaho).

If the Pentaho server starts, but you are not allowed to access the user console or connect to the repository, check if the localhost is enabled in firewall and proxy if you use it.
