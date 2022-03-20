# Challenges - GitsCTF

## D33ply challenge -- Cryptographie
<img src="images/nta-chal1.png" height="50%" width="70%">



Paste the code into cyberchef gives a binary code :


When we apply the binary decode in cyberchef it's gives the flag: ` `


## FTP Stuck Challenge -- Forensic
<img src="images/nta-chal1.png" height="50%" width="70%">

Nous avons un fichier pcap nommé FORENSIC1.pcap

Nous devons retrouvé la trace d'un fichier uploader pour trouver le flag.

J'ai commencé par filtrer les packets suivant le protocol http. En parcourant les packets obtenus, on trouve un fichier nommé upload.php .

<img src="images/upload.png" height="50%" width="70%">

En suivant le flux tcp on obtient : 

<img src="images/tcpstream.png" height="50%" width="70%">

En évoulant flux par flux on trouve le flag dans le flux du packet n° 29 : `GitsCTF{F4R3NC1$_N3TW0KS}`.

<img src="images/ftpflag.png" height="50%" width="70%">
