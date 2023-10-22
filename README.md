<h1>Active Directory Home Lab</h1>

<h2>Description</h2>
In this lab, I will walk through how to create an Active Directory home lab environment using Oracle Virtual Box.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Oracle Virtual Box</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>
- <b>Windows Server 2019</b>


<h2>Program walk-through:</h2>

<h3 align="center">
<b>Install Active Directory Domain Services</b>
</h3>

<p align="center">
Add the feature: <br/>
<img src="https://i.imgur.com/BgXqWUu.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Feature done installing:  <br/>
<img src="https://i.imgur.com/KJDm1my.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
</p>

<h3 align="center">
<b>Configuring Post-Deployment</b>
</h3>

<p align="center">
Configure post-deployment:  <br/>
<img src="https://i.imgur.com/QgTXlm0.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Choose a new forest and enter the domain:  <br/>
<img src="https://i.imgur.com/M1wkvl8.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Enter password:  <br/>
<img src="https://i.imgur.com/rUEDvTn.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Uncheck create DNS delegation:  <br/>
<img src="https://i.imgur.com/d8xPG43.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
</p>

<h3 align="center">
<b>Creating Admins Organizational Unit and Adding an Admin User</b>
</h3>

<p align="center">
Choose Organizational Unit from the list:  <br/>
<img src="https://i.imgur.com/kTZ6NP4.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Enter "_ADMINS" as the name:  <br/>
<img src="https://i.imgur.com/tIobtUQ.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />

<p align="center">
Choose User from the list:  <br/>
<img src="https://i.imgur.com/58Z7wdx.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Enter user info:  <br/>
<img src="https://i.imgur.com/dwHS4ve.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Need to add user to domain admins:  <br/>
<img src="https://i.imgur.com/6WGwQTc.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Adding the user to domain admins:  <br/>
<img src="https://i.imgur.com/AWXBhJ3.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
User is now in the admins OU:  <br/>
<img src="https://i.imgur.com/T8eaCK0.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />

<h3 align="center">
<b>Adding Remote Access Feature</b>
</h3>

<p align="center">
Choosing remote access feature:  <br/>
<img src="https://i.imgur.com/xaFFkeE.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Choose routing in role services:  <br/>
<img src="https://i.imgur.com/HmoaikJ.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Feature is now installed:  <br/>
<img src="https://i.imgur.com/ucYGswV.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />

<h3 align="center">
<b>Configuring Routing and Remote Access</b>
</h3>

<p align="center">
Choose configure:  <br/>
<img src="https://i.imgur.com/TGXMemA.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Choose NAT:  <br/>
<img src="https://i.imgur.com/rckayvm.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Choose the internet adapter:  <br/>
<img src="https://i.imgur.com/URbjaNs.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />

<h3 align="center">
<b>Install DHCP Feature</b>
</h3>

<p align="center">
Choose DHCP server:  <br/>
<img src="https://i.imgur.com/mD9rxfE.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Feature is now installed:  <br/>
<img src="https://i.imgur.com/kJ4TS5k.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />

<h3 align="center">
<b>Configure DHCP Server</b>
</h3>

<p align="center">
Choose new scope:  <br/>
<img src="https://i.imgur.com/BvibbM6.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Enter IP address range as name:  <br/>
<img src="https://i.imgur.com/r2LomNE.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Enter IP address range and subnet mask value:  <br/>
<img src="https://i.imgur.com/BgCLWhu.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Set default gateway:  <br/>
<img src="https://i.imgur.com/IWBfp1I.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Verify domain is correct:  <br/>
<img src="https://i.imgur.com/ulIGkWG.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Authorize and refresh DHCP server:  <br/>
<img src="https://i.imgur.com/2DMewZC.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Server is now green (was red before):  <br/>
<img src="https://i.imgur.com/YkLPEtY.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />

<h3 align="center">
<b>Creating User Organizational Unit and Adding Users</b>
</h3>

<p align="center">
Choose Organizational Unit and name it "_USERS":  <br/>
<img src="https://i.imgur.com/ONE5fBh.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Create new user:  <br/>
<img src="https://i.imgur.com/WgsO72v.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Created a few other users:  <br/>
<img src="https://i.imgur.com/l9fW8Gc.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />

<h3 align="center">
<b>Adding Client Computer to Domain</b>
</h3>

<p align="center">
Choose "System" in start menu:  <br/>
<img src="https://i.imgur.com/fLM4ZoB.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Choose "Rename this PC (advanced)":  <br/>
<img src="https://i.imgur.com/3JWdDfJ.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Choose "Change":  <br/>
<img src="https://i.imgur.com/Wh50Vdh.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Enter "CLIENT1" for the name and "mydomain.com" for the domain:  <br/>
<img src="https://i.imgur.com/uq1nvg1.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Verify with admin credentials:  <br/>
<img src="https://i.imgur.com/6nnVQ9e.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Client has been added to the domain:  <br/>
<img src="https://i.imgur.com/ZPWlTGq.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />

<h3 align="center">
<b>Confirm Client has an IP address and is On the Computers List</b>
</h3>

<p align="center">
CLIENT1 has an IP address:  <br/>
<img src="https://i.imgur.com/36t3Vcl.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
CLIENT1 is on the computers list:  <br/>
<img src="https://i.imgur.com/SnhNGtX.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />

<h3 align="center">
<b>Signing in On One of the User Accounts on Client Computert</b>
</h3>

<p align="center">
"jdoe" user is signed in on the client using the "whoami" command:  <br/>
<img src="https://i.imgur.com/G6oPshs.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
