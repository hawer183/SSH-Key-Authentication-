SSH-Key-Authentication<br><br>

SSH Key Authentication between two linux computer<br>

I have two remote hosts:<br>
&emsp;&emsp;  (M): Master host -> 192.168.200.165 (green prompt)<br>
&emsp;&emsp; (S): Slave host  -> 192.168.200.150 (red prompt)<br>

M:<br>
&emsp;&emsp; ssh-keygen -t rsa<br>
  
S:<br>
&emsp;&emsp; cd ~<br>
&emsp;&emsp; mkdir /root/.ssh<br>
  
M:  <br>
&emsp;&emsp; ssh-copy-id -p 23 root@192.168.200.150<br>
&emsp;&emsp; ssh -p 23 root@192.168.200.150<br>
  
