# Initial changes to access the Pi cleanly over SSH
 '''
 sudo apt install openssh-server
 sudo apt install sshguard
 sudo nano /etc/ssh/sshd_config
 '''
 
 Look for the line that says X11Forwarding. Make sure this is uncommented and it says yes afterward like:
 '''
 ...
 X11Forwarding yes
 ...
 '''