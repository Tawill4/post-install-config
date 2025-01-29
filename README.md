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
- Change settings to only allow people with a login to create tickets / Require registration to create tickets
- Create / Configure agents to work tickets
- Assign created agents to different departments that were previously created
- From within the agent panel, create Users or "employees" that will be creating/submitting tickets
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
Next on the list I created a new team called "Online Banking", this is to route specific tickets relating to the software of an online banking app or website.
</p>
<br />

<p>
<img src="https://i.imgur.com/m6R5Vyz.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Then, inside user settings within the admin panel I had to check the box next to "require registration and login to create tickets". This is so we can create users, and logins for the users to simulate what it would look like to create a ticket from an employees POV.
</p>
<br />

<p>
<img src="https://i.imgur.com/FUK2boe.jpeg" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
The next step was to create an Agent (someone to work the tickets), so from within the admin panel I created an agent named "Jane Doe". After creating Jane, I put her into the SysAdmins department to give her the same permissions that I gave SysAdmins earlier in the lab.
</p>
<br />

<p>
<img src="https://i.imgur.com/xX1jvTV.jpeg" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
After Jane Doe, I created another agent named "John Doe", but instead of putting him in the same department I put him into the "Supreme Admin" department with a support role. This way when I create tickets and send them to different departments, I can login to different agents and observe.
</p>
<br />

<p>
<img src="https://i.imgur.com/6q6E6fO.jpeg" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now from the agent panel, I went to users > create, and I created users "Ken", and "Karen". These will be our employees so to speak. They will be able to create and send tickets.
</p>
<br />

<p>
<img src="https://i.imgur.com/KTTwdNq.jpeg" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
With tickets, there needs to be some sort of way to categorize them in regards to priority. In order to do this I created different SLA's (Service Level Agreement). This decides the order / time period the tickets need to be worked in. For example Sev-A would be the most important, Sev-B is below Sev-A, and Sev-C is the lowest level priority. This is usually determined by the importance to the company running / making money.. For instance, if a banks online banking went completely down, that would severely affect the business so it would be Sev-A. The next steps below will be examples of this.
</p>
<br />

<p>
<img src="https://i.imgur.com/XGaF1qO.jpeg" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
I then just needed to configure different help topics for the users to choose from. In this step I created a help topic named "business critical outage". Which if you remember, would be classified a Sev-A SLA, so after creating the topic I assigned it to Sev-A.
</p>
<br />
