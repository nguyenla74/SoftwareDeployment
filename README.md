# Software Deployment
How to Deploy a Software Using Group Policy

<h2>Utilities Used</h2>

- <b>Group Policy Management (Active Directory)</b>
- <b>Virtual Machines (VirtualBox)</b>
- <b>Server Manager</b>

<h2>Environments Used </h2>

- <b>Windows 10 Pro</b>
- <b>Windows Server 2016</b>

<h2>Step-by-Step Instructions</h2>
<p align="center">
In Windows Server machine, open "Server Manager", then click "Tools" > "Group Policy Management": <br/>
<img src="https://i.imgur.com/BZ7xzsT.png" height="80%" width="80%" alt="Software Deployment"/>
<br />
<br />
In the "Group Policy Management" window, right click on your domain (i.e. "test.local"), select "Create a GPO in this domain, and Link it here..." :  <br/>
<img src="https://i.imgur.com/6gq4njD.png" height="80%" width="80%" alt="Software Deployment"/>
<br />
<br />
Name the GPO (Group Policy Object) (i.e. Skype): <br/>
<img src="https://i.imgur.com/h3KqfVL.png" height="80%" width="80%" alt="Software Deployment"/>
<br />
<br />
Navigate to "Linked Group Policy Objects" tab, right click and select "Edit":  <br/>
<img src="https://i.imgur.com/u6Nhc5D.png" height="80%" width="80%" alt="Software Deployment"/>
<br />
<br />
Select "Computer Configuration":  <br/>
<img src="https://i.imgur.com/mah3rXs.png" height="80%" width="80%" alt="Software Deployment"/>
<br />
<br />
Select "Policies":  <br/>
<img src="https://i.imgur.com/Jahv8LW.png" height="80%" width="80%" alt="Software Deployment"/>
<br />
<br />
Select "Software Settings":  <br/>
<img src="https://i.imgur.com/muAdmoj.png" height="80%" width="80%" alt="Software Deployment"/>
<br />
<br />
Select "Software Installation":  <br/>
<img src="https://i.imgur.com/UA4ovGz.png" height="80%" width="80%" alt="Software Deployment"/>
<br />
<br />
Right click and select "New" > "Package...":  <br/>
<img src="https://i.imgur.com/tCijz9a.png" height="80%" width="80%" alt="Software Deployment"/>
<br />
<br />
Navigate to the file location where you store the MSI file (in this case, Skype MSI file), click "Open":  <br/>
<img src="https://i.imgur.com/4V9iIrd.png" height="80%" width="80%" alt="Software Deployment"/>
<br />
<br />
Select "Assigned" for simplicity, click "OK" :  <br/>
<img src="https://i.imgur.com/DOXFNyQ.png" height="80%" width="80%" alt="Software Deployment"/>
<br />
<br />
Congratulations! Now the software will be installed on target machines after a restart :)  <br/>
<img src="https://i.imgur.com/phVOgpg.png" height="80%" width="80%" alt="Software Deployment"/>
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
