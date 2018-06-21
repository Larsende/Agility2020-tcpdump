tcpdump Switches
~~~~~~~~~~~~~~~~

# tcpdump -D

  To list the available interfaces for packet capture use tcpdump -D

  The 'any' interface will be taken by TMM and made into the interface '0.0'

  .. image:: /_static/tcpdump-d.png

# tcpdump -i

  To capture traffic on a specific interface use tcpdump -i <interface name>. i.e. 'tcpdump -i 0.0'

  When using 0.0 for the interface on a capture make sure to use a capture filter or you will get too much information and may impact performance on the F5.

  .. image:: /_static/tcpdump-i.png

# tcpdump -n

  Use tcpdump -n to disable name resolution of host names

# tcpdump -nn 

  Use tcpdump -nn to disable name resolution of both host names and port names

# tcpdump -X

  Use tcpdump -X to show output including ASCII and hex.  This will making reading screen output easier.

  .. image:: /_static/tcpdump-x.png

# tcpdump -w

  Use tcpdump -w to write the packet capture to a capture file that is readable in an application such as Wireshark.

# tcpdump -s

  Use 'tcpdump -s0' to capture the full data packet.  The number following the 's' indicates the number of bits to capture of each packet.  0 indicates all.
