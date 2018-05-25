4. Install the F5 Wireshark Plugin 
==================================

Wireshark version 2.2.14 is installed on the jumpbox.

You can download the F5 Wireshark plugin from devcentral.f5.com here:  https://devcentral.f5.com/d/wireshark-plugin?lc=1.  In the lab the plugin is already downloaded to C:\F5_Lab\wireshark-plugin.f5ethtrailer.bin.1.11b.

4.1. Start Wireshark by double clicking the shortcut on the desktop.

4.2. Click on Help and then About Wireshark.

4.3. Click on the plugins tab and check to see what directory the plugins are installed to.

4.4. Open the plugin directory in file explorer.

4.5. Copy the F5 wireshark plugin that has been copied to C:\F5_Lab\wireshark-plugin.f5ethtrailer.bin.1.11b.
   
   4.5.1.: The jumpbox client is Windows 32 bit.

   4.5.2.: Open the Win32-2.2.0 folder and copy the f5ethtrailer.dll to the plugin directory determined in step 3.

   4.5.3.: Depending on your OS and Wireshark version, you will need the correct plugin files from the correct folder.

4.6. Shutdwon Wireshark and restart it.

4.7. Click on Help and then About Wireshark.

4.8. Check the plugins tab again and make sure the F5 plugin is installed.

.. image:: ./_static/wireshark-plugin.png
