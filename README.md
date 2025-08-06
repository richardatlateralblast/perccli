PERC CLI Notes
==============

Download
--------

Original Linux/EFI tool (noarch rpm in ZIP file):


https://www.dell.com/support/home/en-us/drivers/driversdetails?driverId=5M4HP


Direct link:


https://dl.dell.com/FOLDER13074167M/1/PERCCLI_7.3208.0_Linux_A01.tar.gz


Documentation
-------------

PERC CLI Guide:

https://dl.dell.com/topicspdf/cli_guide_en-us.pdf


Installing Debian Package
-------------------------

```
tar -xpf PERCCLI_7.3208.0_Linux_A01.tar.gz
sudo dpkg -i PERCCLI_7.3208.0_Linux_A01/Ubuntu/perccli_007.3208.0000.0000_all.deb
```


Setup Alternatives
------------------

```
sudo update-alternatives --install '/usr/bin/perccli' 'perccli' '/opt/MegaRAID/perccli/perccli64' 1
```


Example Output
--------------

```
CLI Version = 007.3208.0000.0000 Feb 20, 2025
Operating system = Linux 6.14.0-27-generic
Status Code = 0
Status = Success
Description = None

Number of Controllers = 1
Host Name = r730p0
Operating System  = Linux 6.14.0-27-generic
StoreLib IT Version = 07.3300.0200.0100
StoreLib IR3 Version = 16.16-0

System Overview :
===============

-------------------------------------------------------------------------
Ctl Model        Ports PDs DGs DNOpt VDs VNOpt BBU sPR DS EHS ASOs Hlth  
-------------------------------------------------------------------------
  0 PERCH730Mini     8  16   3     1   3     1 Opt On  3  N      0 NdAtn 
-------------------------------------------------------------------------

Ctl=Controller Index|DGs=Drive groups|VDs=Virtual drives|Fld=Failed
PDs=Physical drives|DNOpt=Array NotOptimal|VNOpt=VD NotOptimal|Opt=Optimal
Msng=Missing|Dgd=Degraded|NdAtn=Need Attention|Unkwn=Unknown
sPR=Scheduled Patrol Read|DS=DimmerSwitch|EHS=Emergency Spare Drive
Y=Yes|N=No|ASOs=Advanced Software Options|BBU=Battery backup unit/CV
Hlth=Health|Safe=Safe-mode boot|CertProv-Certificate Provision mode
Chrg=Charging | MsngCbl=Cable Failure
```
