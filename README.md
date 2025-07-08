<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles (for grouping permissions)
- Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
- Configure Teams
- Allow anyone to create tickets
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics





After the installation of osTicket, certain configurations need to be made in order for the ticketing system to function effectively. The objectives listed above will be completed in this tutorial.


<h2>Configure Roles (for grouping permissions)</h2>

To begin, the admin username and password that was created in pre-installation will be used to log into osTicket. Once logged on, Roles will be created. Click on “Admin Panel” on the top right corner of the screen then click on the “Agents” tab near the top right. Afterwards, click on “Roles” in the access bar below “Agents”. 

<img src="https://github.com/JosephRC777/post-install-config/blob/c251658b0be857c42e0f065b7baa381614ed74f6/images/osticket%20post%20installation%201.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/post-install-config/blob/c251658b0be857c42e0f065b7baa381614ed74f6/images/osticket%20post%20installation%202.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/post-install-config/blob/c251658b0be857c42e0f065b7baa381614ed74f6/images/osticket%20post%20installation%203.png" width="600" height="400" />



Within this “Roles” section, a “Supreme Admin” role will be created. To create a role, begin by clicking on “Add New Role” on the right side of the screen. 

<img src="https://github.com/JosephRC777/post-install-config/blob/c251658b0be857c42e0f065b7baa381614ed74f6/images/osticket%20post%20installation%204.png" width="600" height="400" />


A “Definition” tab will pop-up. Within this section you can name the role. For this demonstration “Supreme Admin” will be the name for this role. 

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%205.png" width="600" height="400" />


After naming the role, the “Permissions” tab can be clicked to assign the correct permissions to the role.There are 3 sections of permissions, Tickets, Tasks, and knowledgebase.   For the “Supreme Admin” role, all the permissions will be enabled. 

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%206.png" width="600" height="400" />


After permissions have been granted, click on “Add Role” on the bottom of the screen. The role has now been created and can be seen within the “Roles” section. 

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%207.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%208.png" width="600" height="400" />

<h2>Configure Departments</h2> 

Departments will now be configured within osTicket to make ticket assignment easier and more efficient. Return back to the “Admin Panel” and click on “Agents” near the top right. Afterwards, click on “Department” in the access bar below “Agents”. 

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%209.png" width="600" height="400" />



Click on “Add New Department” on the right corner of the screen.

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%2010.png" width="600" height="400" />












A “Settings” screen will pop up. Within this section you can name the department as well as set other settings. For this demonstration, this new department will be named “SysAdmins”. Type in the name in the textbox next to “Name:” All of the other settings for this department will be kept as they are. After naming the department, click on the “Access” tab on the top of the screen. 

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%2011.png" width="600" height="400" />





Nothing will be changed within the “Access” tab for this department. Click on “Create Dept” on the bottom of the screen. The department has been created and can be seen Within the “Departments” section.

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%2012.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%2013.png" width="600" height="400" />




<h2>Configure Teams</h2>

Teams will now be configured within osTicket to make ticket assignment easier and   more efficient. Return back to the “Admin Panel” and click on “Agents” near the top right. Afterwards, click on “Teams” in the access bar below “Agents”. 

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%2014.png" width="600" height="400" />



Click on “Add New Team” on the right corner of the screen.

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%2015.png" width="600" height="400" />


A “Team” section will pop up. Within this section you can name the team as well as configure other settings. For the purposes of this tutorial the team will be named “Online Banking”. After typing the name in the textbox next to “Name”, leave all the other settings the same then click on “Create Team” on the bottom of the screen. The team has been created and can be seen Within the “Teams” section.

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%2016.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%2017.png" width="600" height="400" />



<h2>Allow anyone to create tickets</h2>

Permission to create tickets will be given to everyone without the need of an account. Return back to the “Admin Panel” and click on “Settings” near the top left. Afterwards, click on “Users” in the access bar below “Settings”. 

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%2018.png" width="600" height="400" />




Within this tab, the checkbox next to “Require registration and login to create tickets” needs to be unchecked. This will allow anyone to create tickets without needing to create an account.  Once unchecked, click on “Save Changes” on the bottom of the 
screen. 

<img src="https://github.com/JosephRC777/post-install-config/blob/da67d92ce6678d837cd4444e15787fa067ff9904/images/osticket%20post%20installation%2019.png" width="600" height="400" />


Configure Agents (workers)

New “Agents” will now be added and configured. These accounts will be working and resolving the tickets. To begin, Click on “Admin Panel” on the top right corner of the screen then click on the “Agents” tab near the top right. Afterwards, click on “Add New Agent” in the access bar below “Agents”. 


































Within the “Add New Agent” section, there are 4 tabs where information can be added. Under the “accounting” tab the following information can be added; Name, email address, phone number, mobile number and username. For this tutorial demonstration the agents “Jane” and “John” will be created. In the text box next to “Name:”, type in the agent's first and last name and in the textbox next to “Email Address:” type in the email address that the agent will use to work within osTicket. 


































Under the “Authentication” section, there is a textbox next to “Username:”. In this textbox, the user name of the agent will be typed in. 







































Click on “Set Password” next to the username textbox. 






































Within this “Set Agent Password”  screen, uncheck the checkbox next to “Send the 
agent a password reset email”. 


















Once clicked, two empty textboxes will pop up. The password for this account can now be typed in and confirmed. There is an option to have the user change their password at the next login on the bottom left. For this tutorial, this checkbox will remain uncheked. Afterwards, click on “Set” in the bottom right hand corner.  
















Once completed, the window will close and the “Account” tab will show up again. The “Status and Settings” section will be left as is for this tutorial. Click on the “Access” tab next to “Account”. 





































Within the “Access” tab, the department and role can be set up per agent. The created agent “Jane” will be a part of the “SysAdmins” and her role will be “Supreme Admin”. The “Permissions” section will be left as is for this tutorial. Click on the “Teams” tab next to “Permissions”. 




































Within the “Teams” tab, the agents can be assigned to teams. Any ticket that gets assigned to the designated team can be seen and worked on by any agent that is in that team. Agent “Jane” will be assigned to the “Online Banking” team. After the team has been assigned, click on “Create” on the bottom of the screen. 





















If everything was done correctly, “Jane” will now appear under the agents section. 














All of the above steps can now be followed to create new agents. The agent “John” will be created following all of the above steps. 

Configure Users (customers)

Users will now be created within osTicket. Click on “Agent Panel” on the top right corner of the screen then click on the “Users” tab near the top right. Afterwards, click on “Add User” in the access bar below “Users”. 
































A “Lookup or create a user” screen will pop-up. Within this screen, you can set an email address, type in a full name and provide a phone number for a user account. For this tutorial the user “ken” will be created. Type in an email the user will use in the textbox next to “Email Address:”. In the textbox next to “Full Name:” type in the user's full name. The phone number section will be left blank. After all the fields have been filled, click on “Add User” on the bottom right hand corner of the screen. 



















The user will now appear under the ”Users” section within osTicket.















Configure SLA

SLAs will now be configured. SLAs are formal agreements that define the expected response and resolution times for support tickets. This is based on their priority and the severity of the ticket. To begin, Click on “Admin Panel” on the top right corner of the screen then click on the “Manage” tab near the middle of the screen. Afterwards, click on “SLA” in the access bar below “Manage”. 



















Click on “Add New SLA Plan” on the right hand corner of the screen. 













Within this screen, you can name SLAs, determine whether it will be active or disabled, provide a grace period and a schedule. For this tutorial the following SLAs will be created with the appropriate grace period and schedule:

	Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)

In the textbox next to “Name”, type in the name of the SLA. All of the above SLAs will be active. In the textbox next to “Grace Period”, type in the number of hours that the ticket needs to be resolved within. In the schedule dropdown menu, select the appropriate time frame when this ticket would be resolved. After all of these fields have been filled, click on “Add Plan” on the bottom of the screen. 














































Now that these SLAs have been created, tickets can be given a proper priority for completion.



Configure Help Topics

Help topics will now be configured. Help topics will help in further categorizing tickets and filtering them to make sure they are resolved efficiently. To begin, To begin, Click on “Admin Panel” on the top right corner of the screen then click on the “Manage” tab near the middle of the screen. Afterwards, click on “Help Topics” in the access bar below “Manage”. 









Click on “Add New Help Topic” on the right hand corner of the screen



















Within this section, you can name help topics, select the status for the help topics (for this tutorial all of the topics will be active), determine whether these topics will be public or private, and select a parent topic that it can be under. For this tutorial the following help topics will be created. 

Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other


In the textbox next to “Topic”, type in the name of the help topic. All of the above help topics will have their status as active, they will also have the type be public. In the “Parent Topic” dropdown menu, select the appropriate parent topic where the created topic would be under. After all of these fields have been filled, click on “Add Topic” on the bottom of the screen. 











































































































Now that the help topics have been created, everything that is needed to operate osTicket and resolve ticket requests is up and ready to go. This concludes this tutorial. 

