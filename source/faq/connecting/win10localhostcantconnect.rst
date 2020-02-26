Can't connect to localhost Win10 server with Minecraft Win10 Edition
""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

This issue occurs due to loopback restrictions on Windows 10 UWP apps. To lift this restriction, launch Windows PowerShell as an administrator and run the following:

.. code-block:: sh

    CheckNetIsolation LoopbackExempt -a -n="Microsoft.MinecraftUWP_8wekyb3d8bbwe"
    
    or setup new device via win+r>hdwwiz.exe>manual setup>network adapter>microsoft>loopback adapter Microsoft KM--TEST
