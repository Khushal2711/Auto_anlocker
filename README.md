# Auto_anlocker

Windows
Added a GUI to the Windows release
Added a file to signal the patch being already applied, to avoid reapplying it again with an unkown outcome
Features:

The GUI provides a simple interface for the patch process
The vmware install path will still be retrieved from the registry, but you can change it if you need to
The option to download the tools can be disabled and a custom path where you already have the tools downloaded can be chosen. By default it's set to the tools folder in the current directory
You can also download the tools in the said folder through the Download button
The patch will no longer work more than one time on the same installation, without uninstalling it first. This is done by creating a .unlocker hidden file in the vmware install directory. To force applying the patch you have to delete this file first.
Linux
The shell output now has colors to differentiate between different log levels. Error output is red for signaling non-critical errors raised while patching
Notes:

This release has gone through a bit of refactoring, and I did not test it extensively. If there's something not working as expected please provide a feedback in the Issues section and use the v1.1.4 command line version
Linux build is no more provided. Instead it has to be compiled from scratch
