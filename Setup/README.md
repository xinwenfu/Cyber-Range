[VirtualBox kernel modules do not match this version of VirtualBox](https://askubuntu.com/questions/837427/virtualbox-kernel-modules-do-not-match-this-version-of-virtualbox)

Exit virtualbox and reinstall it
```
sudo apt remove --purge virtualbox
sudo apt install virtualbox
sudo apt install virtualbox-dkms
```

Configure the PC in Cyber Range
1. Install all VMs into /vm
2. Change the properties of /vm
3. read/write by Group and Others
