# Challenges - GitsCTF

## D33ply challenge -- Cryptography 
<img src="images/nta-chal1.png" height="50%" width="50%">



Paste the code into cyberchef gives a binary code :


When we apply the binary decode in cyberchef it's gives the flag: ` `


## FTP Stuck Challenge -- Forensic
<img src="images/nta-chal1.png" height="50%" width="50%">

We have a pcap file named FORENSIC1.pcap

We must found an upload file who contain the flag.

I started by filtering using the http protocol. Browsing through the captured packets I found a file named upload.php.
<img src="images/upload.png" height="50%" width="70%">

Following the tcp stream we have:
<img src="images/tcpstrem.png" height="50%" width="70%">

The flag is : `GitsCTF{F4R3NC1$_N3TW0KS}`
