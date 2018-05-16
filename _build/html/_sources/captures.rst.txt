5. Taking a Capture from the F5
===============================

Let's take the information we have gathered so far and take a packet capture from the F5.  

5.1. Start Putty and launch the bigip1 SSH session.

5.2. Login as root user.

5.3. List the destination address of the virtual on the F5 using the following command:
     
   5.3.1. tmsh list ltm virtual hackazon.f5demo.com_https_vs destination

5.4. Now take the destination address and compose a tcpdump command to track the traffic coming to this virtual server:

     5.4.1. tcpdump -nni 0.0:nnn -s0 -w/var/tmp/hackazon.pcap host 10.1.10.201

5.5. After starting the capture, start Chrome and click on the Hackazon bookmark.  Browse around the site following a couple links.  Next go to the address bar and type in: "https://hackazon.f5demo.com:8080".  Then stop the capture in the putty session by using 'Ctrl+c'.

5.6. Now start WinSCP from the quick launch bar.

5.7. Select the F5-LTM and click on Login.

5.8. On the right side of WinSCP browse to /shared/tmp/ and move the hackazon.pcap file to the My Documents folder on your pc on the left.  

5.9. Now open Wireshark and open the hackazon.pcap file you just copied from the F5. 
