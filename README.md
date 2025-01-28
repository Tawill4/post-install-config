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

- Configure roles within the admin panel
- Configure Departments within the admin panel
- Configure Teams within the admin panel
- Change settings to allow anyone to create tickets / Require registration and login to create tickets
- Create / Configure agents to work tickets
- Assign created agents to different departments that were created
- From within the agent panel, create Users or "employees" that will be creating tickets
- From back within the admin panel, create SLA plans (Sev-A, Sev-B, and Sev-C)
- Assign priority and grace period for SLA plans
- Create Help topics for the Users / Employees to choose when creating a ticket
- Assigning SLA plans to the Help topics.

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/TfdfBWb.jpeg" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Following the installation of osTicket, there are some things I configured to make it resemble an actual workplace HelpDesk. First I went ahead and created a new role named "Supreme Admin", and I gave it all permissions and tasks so it has all access.
</p>
<br />

<p>
<img src="https://i.imgur.com/JpBi8CX.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next I created a new Department called "SysAdmin". Creating departments ensures that tickets are routed efficiently, handled by the right people, and organized in a way that supports the business’s needs. 
</p>
<br />

<p>
<img src="https://i.imgur.com/MYgN0In.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next on the list I created a new team called "Online Banking", this is to route specific tickets relating to the software of an online banking app or website. Similar help topics may get routed here as well.
</p>
<br />
