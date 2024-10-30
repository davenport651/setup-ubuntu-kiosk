# setup-ubuntu-kiosk
The simple script to setup ubuntu kiosk for desired app.

Just install Ubuntu Server (for e.g. tested on Ubuntu Server 24.04) as minimized installation and copy script to the home folder (via SFTP) give execution permissions and run with "sudo".
The script will make host reboot and autologin in GUI with Remmina app window.

Right click menu of the openbox was purposefully disabled.

Little configuration of the SSH and basic iptables rules applied (can be changed in script).

**Use Ctrl + Alt + F1 to exit Openbox and proceed to tty1**
