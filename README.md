# Cyber Range

We created a lot of [video tutorials](https://sites.uml.edu/ccf/education/video-tutorials/) on Cyber Range and refer to them if needed.

UMass Lowell has a virtual Cyber Range, called Cyber Range for brevity. We offer remote access to virtual machines (VMs) hosted over Cyber Range, which is behind a firewall. To access the VMs, a person has to acquire an OpenVPN profile and use OpenVPN to connect to our OpenVPN server. Once connected to the OpenVPN server, a person may access the VMs in a few ways: (i) web access; (ii) Micrsoft Remote Desktop; (iii) SSH (e.g. Putty) if a SSH server runs on the particular VM.

## Install OpenVPN
Access to any VM on Cyber Range requires OpenVPN connection.

1. Download [OpenVPN for Windows](https://openvpn.net/client-connect-vpn-for-windows/), or [OpenVPN for MacOS](https://openvpn.net/client-connect-vpn-for-mac-os/)
2. Click the downloaded file and follow the installation instructions to install OpenVPN 
3. Get an OpenVPN profile (a .ovpn file) from the administrator.
4. Open OpenVPN and go to “Import Profile” 
   - If you are using OpenVPN for the first time, then when you open OpenVPN, it should just be a screen that says “Import Profile”. If this is not what you see, either click the “+” button in the bottom right corner or click the three horizontal bars in the top left corner, then click “Import Profile”
5. Click “File”, then browse your .ovpn file that you downloaded from Dropbox in step 3
6. Click “Add”
7. Now connect to this profile.


## Web access
1. Browse https://xoa.cyberseclab.uml.edu within the browser and log into the virtual Cyber Range with the provided username and password.
2. Within the virtual Cyber Range, i.e. XOA web page, click the Home button to see all (two) virtual machines (VMs) allocated to each student. 
   - Click Filters at the top of the webpage and select *None* if there is no VM listed.


## Micrsoft remote desktop protocol (RDP)
1. Download *Micrsoft Remote Desktop* from Microsoft Store or Apple Store
2. Click on the **+** icon in the top panel to “Add PC”
   - Enter the IP address for the VM you want to connect to in the “PC name” box
   - Click “Add”
   - To connect to the VM over RDP, simply double click on the saved PC and then enter credentials when prompted

If the connection is very slow, you may need to change the resolution of the remote desktop. Here is how to do so:
- Exit your RDP session
- Click on the edit icon on the saved PC to “Edit PC”. You may click **...** for more options.
- Click the “Display” tab
- Under “Resolution”, move the bar so that it says “1280 by 1024” and click “Save”
- Now connect to the VM again, following the steps from earlier

## SSH (e.g. Putty)
You may access the Kali VM and Metasploitable VM through SSH, e.g., [Putty](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html) or the native *ssh* command under MacOS and Linux. Please note Metasploitable does not support RDP.


|Machine       |	SSH Port |	Command Example             |	RDP Support |
|--------------|-----------|------------------------------|-------------|
|Kali          | 	2022	   |ssh kali@192.168.7.144 -p 2022|	Yes         |
|Metasploitable|	22	      |ssh msfadmin@192.168.7.144    |	No          |
|Windows	      |N/A        |	N/A                         |	Yes         |

