# Initial changes to access the Pi cleanly over SSH
 ```
 sudo apt install openssh-server
 sudo apt install sshguard
 sudo nano /etc/ssh/sshd_config
 ```
 within /etc/ssh/sshd_config, look for the line that says X11Forwarding. Make sure this is uncommented and it says yes afterward like: `X11Forwarding yes`
 
 You can check that your configuration by doing trying to start a little GUI on your desktop. To do this, leave your ssh session by typing `exit`
 
 On your main PC install Xming, then start it up. SSH back into the Pi/BBB by using `ssh -X <username>@<ip_address>` and type
 
 ```
sudo apt-get install x11-apps
xeyes
```