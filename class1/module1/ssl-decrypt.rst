11 Decrypting SSL in Wireshark
==============================

Now you need to have your pre-master key file and your capture moved to your local box.  To do this do the following:

11.1. Open Terminal on the Ubuntu Jump Box.

11.2. Run the following commands:

.. code-block:: bash
   :linenos:

   sudo scp root@10.1.1.245:/var/tmp/session.pms /var/tmp/session.pms
   sudo scp root@10.1.1.245:/var/tmp/hackazon.pcap /var/tmp/hackazon.pcap

After each of these commands you will be prompted to accept the SSH keys.  Type yes to continue. Then you will be prompted for the F5 root password.  Type that in as well.
 
11.3. Now open Wireshark.  

11.4. Once Wireshark is open go to Edit/Preferences.

11.5. Expand on the left side, Protocols, then select SSL.

.. image:: /_static/premaster-session.png

11.6. Browse to the pre-master session key file and click on save.

11.7. Open in Wireshark the pcap file you pulled down from the F5 BIG-IP. 

11.8. Right click on one of the SSL packets and select Follow, SSL Stream.

.. image:: /_static/follow-ssl-stream.png

11.9. You will now see unencrypted SSL data in the capture as follows:

.. image:: /_static/ssl-decrypted-data.png
