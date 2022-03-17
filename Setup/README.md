[VirtualBox kernel modules do not match this version of VirtualBox](https://askubuntu.com/questions/837427/virtualbox-kernel-modules-do-not-match-this-version-of-virtualbox)

Exit virtualbox and reinstall it
```
sudo apt remove --purge virtualbox
sudo apt install virtualbox
sudo apt install virtualbox-dkms
```

Install all VMs into /vm
Change the properties of /vm
read/write by Group and Others
