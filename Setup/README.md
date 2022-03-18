[VirtualBox kernel modules do not match this version of VirtualBox](https://askubuntu.com/questions/837427/virtualbox-kernel-modules-do-not-match-this-version-of-virtualbox)

Exit virtualbox and reinstall it
```
sudo apt remove --purge virtualbox
sudo apt install virtualbox
sudo apt install virtualbox-dkms
```

Copy .ova files to a computer
```
scp cyberadmin@192.168.7.194:/vm/*.ova /vm/.
```

Configure the PC in Cyber Range
1. Install all VMs into /vm
2. Change the properties of /vm
   - read/write by Group and Others

Configure VirtualBox
1. File -> Prefenreces -> Network -> Add
2. Particular VM -> Settings -> USB -> Uncheck it



Chane the network setting of Kali VM to NatNetwork and disable USB too.
