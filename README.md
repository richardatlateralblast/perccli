PERC CLI Notes
==============

Download
--------

Original Linux/EFI tool (noarch rpm in ZIP file):


https://www.dell.com/support/home/en-us/drivers/driversdetails?driverId=PDG3H


Convert to Debian package
-------------------------

```
sudo apt install alien
tar -xpf perccli_7.1-007.0127_linux.tar.gz
cd Linux
sudo alien perccli-007.0127.0000.0000-1.noarch.rpm
```

Install package:

```
sudo dpkg -i perccli_007.0127.0000.0000-2_all.deb
```
