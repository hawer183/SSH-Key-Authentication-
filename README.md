 SSH-Key-Authentication
SSH Key Authentication between two linux computer

I have two remote hosts:
  (M): Master host -> 192.168.200.165 (green prompt)
  (S): Slave host  -> 192.168.200.150 (red prompt)

M:
  ssh-keygen -t rsa
  
S:
  cd ~
  mkdir /root/.ssh
  
M:  
  ssh-copy-id -p 23 root@192.168.200.150
  ssh -p 23 root@192.168.200.150
  
