Install the F5 Wireshark Plugin by doing the following
======================================================

Wireshark version 2.2.14 is installed on the jumpbox.

1. Start Wireshark by double clicking the shortcut on the desktop.
2. Click on Help and then About Wireshark.
3. Click on the plugins tab and check to see what directory the plugins are installed to.
4. Open the plugin directory in file explorer.
5. Copy the F5 wireshark plugin that has been copied to C:\F5_Lab\wireshark-plugin.f5ethtrailer.bin.1.11b from: https://devcentral.f5.com/d/wireshark-plugin?lc=1.
   A. The jumpbox client is Windows 32 bit.
   B. Open the Win32-2.2.0 folder and copy the f5ethtrailer.dll to the plugin directory determined in step 3.
   C. Depending on your OS and Wireshark version, you will need the correct plugin files from the correct folder.
6. Shutdwon Wireshark and restart it.
7. Click on Help and then About Wireshark.
8. Check the plugins tab again and make sure the F5 plugin is installed.

