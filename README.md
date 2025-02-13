# setup-ubuntu-kiosk
The simple script to setup ubuntu kiosk for desired app.
The script will make host reboot and autologin in GUI with Java app window.

Right click menu of the openbox was purposefully disabled.

Little configuration of the SSH and basic iptables rules applied (can be changed in script).

**Use Ctrl + Alt + F1 to exit Openbox and proceed to tty1**

 Steps to Install and Configure Ubuntu Server 24.04 as a Java Applet Kiosk:
 1. Install Ubuntu Server 24.04: Use the minimized installation setup and skip adding any additional Snap packages.
 2. Update and Upgrade Packages: Ensure all packages are up-to-date as desired.
 3. Set a Static IP Address: If you plan to access the server via SSH long-term, configure a static IP 
    to prevent issues once the DHCP lease expires.
 4. Copy the Setup Script: Retrieve the machine's IP address, connect via SFTP, and copy the setup_kiosk.sh script to the server.
 5. Run the Setup Script: Grant execute permissions using "chmod +x setup_kiosk.sh", then run the script with "sudo".

 What the Script Configures:
 - Kiosk User Setup: Creates a new user (kiosk-user) configured to auto-login and launch the java application.
 - SSH Settings: Adjusts LoginGraceTime, login attempts, and maximum concurrent sessions for SSH.
 - IPTables Rules: Sets rules to allow outgoing traffic and DNS requests.


![image](https://github.com/user-attachments/assets/17712e9e-c20b-4b25-bf8d-803d6ed6cc2c)
