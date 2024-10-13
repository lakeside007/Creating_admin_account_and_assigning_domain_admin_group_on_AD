# Creating Domain Admin Account on Active Directory




<h2>Description</h2>
This project entails the creation of a domain admin account which would be responsible for most of the configurations for domain users. VirtualBox was used to host the Windows Server 2019 system used for this project and lab. This is a lab environment to practice and not a real work environment, in a real production environment where user accounts are being created, it is advisable to select "user must change password at next logon" to ensure the user does not continue to use default passwords set by an admin. 
<br />



<h2>Environments Used </h2>

- <b>VirtualBox</b>
- <b>Windows Server 2019</b>

<h2>Project walk-through:</h2>

<p align="center">
Select Active Directory and Users to access the domain controller which will be used to create the admin account: <br/>
<img src="https://imgur.com/4Gvqv1O.png" height="80%" width="80%" alt="Accessing domain controller to create admin account"/>
<br />
<br />
Right click on the domain link, select "New" then "Organization Unit" to create an Organization Unit specifically for ADMINS:  <br/>
<img src="https://imgur.com/ymaDhyx.png" height="80%" width="80%" alt="Creating the ADMINS organization unit"/>
<br />
<br />
Create the ADMINS organization unit inside the domain: <br/>
<img src="https://imgur.com/OoFDtnI.png" height="80%" width="80%" alt="ADMINS organization unit created"/>
<br />
<br />
Right click on the ADMINS created organization unit to add domain admin account details like First Name, Last Name and Username then a password to secure the account:  <br/>
<img src="https://imgur.com/5hbCgUP.png" height="80%" width="80%" alt="Creating domain controller"/>
<br />
<br />
Verify details and finish creating the domain admin account:  <br/>
<img src="https://imgur.com/38qsmQw.png" height="80%" width="80%" alt="Finish creating the domain controller."/>
<br />
<br />
Select the admin account, right click then select properties to add the account to the "Domain Admin" group:  <br/>
<img src="https://imgur.com/L2umXBR.png" height="80%" width="80%" alt="Add to Domain Admin group"/>
<br />
<br />
Type in "Domain Admin" as object name then click check names to ensure it becomes underlined, once underlined, it means the object name "Domain Admin" as been selected. Click Ok to complete: <br/>
<img src="https://imgur.com/OwWFEo6.png" height="80%" width="80%" alt="Complete the step of adding the admin account to the Domain Admin group"/>
<br />
<br />
This page displays the admin account now being part of two groups which are the Domain User and Domain Admin group. This gives the admin account the attributes and capabilities of both groups. Once safified with this, click apply and ok to confirm the configuration/setting: <br/>
<img src="https://imgur.com/kZ8EzKE.png" height="80%" width="80%" alt="Confirmation of the groups the admin account is a part of"/>
<br />
<br />
To test and confirm the functionality of the admin account, click the windows button, find the user icon then sign out to logout from the current user and log into the domain using the username and password created for the admin account. In this case, the admin account username is: a-miraclek and password is: *******. Once on the login window, select user then other users, this will pop up a space to input a username and password instead of just the regular password it usually asks for. The admin account will be successfully logged in after this process: <br/>
<img src="https://imgur.com/rhGJ3wG.png" height="80%" width="80%" alt="Logging in the admin account with the username and password"/>
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
