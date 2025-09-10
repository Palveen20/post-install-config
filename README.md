<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration Guide</h1>
After successfully installing osTicket on a Windows Server VM in Microsoft Azure, the next step is to configure the system so it can function as a fully operational help desk ticketing solution. This post-install configuration ensures that roles, agents, departments, and service workflows are properly defined, allowing tickets to be routed and resolved efficiently.

This guide walks through the key configuration steps within the Admin Panel of osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Protocol (RDP) – to access the VM
- Internet Information Services (IIS) - to host os Ticket

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users
- Configure SLA
- Configure Help Topics
Each of these steps establishes how osTicket will manage tickets, assign responsibilities, and track response times.




<p align="center">
  <h1>Configure Roles</h1>
</p>



<strong>Navigate to: Admin Panel > Agents > Roles</strong>
<p>
</p>
<p>Roles define the level of access and permissions for support staff. For example, administrators may have full control, while support agents may only have access to assigned tickets.
</p>
<br />
<p>
<img <img width="829" height="473" alt="Screenshot 2025-09-01 181421" src="https://github.com/user-attachments/assets/1ba8bdea-2066-4cf1-b5a6-58c39010c646"/>
</p>
<img width="828" height="583" alt="Screenshot 2025-09-01 181436" src="https://github.com/user-attachments/assets/b0b2772e-f457-4eb5-a99b-ef058687d792"/>

<img width="829" height="464" alt="Screenshot 2025-09-01 181502" src="https://github.com/user-attachments/assets/db0c2b59-7ba9-48dc-91cd-edc17c1c2098"/>

<img width="828" height="340" alt="Screenshot 2025-09-01 181513" src="https://github.com/user-attachments/assets/a53874f3-fd6a-4fe2-8646-80b68185ce9d"/>

<img width="825" height="379" alt="Screenshot 2025-09-01 181524" src="https://github.com/user-attachments/assets/376672b6-6a18-4842-a0dd-584d1ecb0e5d"/>






<p>
</p>
<br />



<p align="center">
  <h1>Configure Departments</h1>
</p>



<strong>Go to: Admin Panel > Agents > Departments</strong>
<p>
Departments allow you to organize ticket assignments by function, such as:
System Administrators
Human Resources
Customer Support
This makes it easier to assign issues to the right group of people.  
</p>
<p>
</p>
<br />
<p>
<img <img width="831" height="555" alt="Screenshot 2025-09-01 181549" src="https://github.com/user-attachments/assets/46e421ac-0841-45c6-af64-c9aff42857ab"/>
</p>
<p>
</p>
<br />






<p align="center">
  <h1>Configure Teams</h1>
</p>



<strong>Path: Admin Panel > Agents > Teams</strong>
<p>
Teams are cross-departmental groups that can be assigned to specific types of tickets.
</p>
<p>Example: Online Banking Team – members from IT and Finance working together to handle customer banking issues.
</p>
<br />




<p align="center">
  <h1>Allow anyone to create a ticket</h1>
</p>



<strong>Admin Panel > Settings > User Settings.</strong>
<p>
Uncheck the option: “Require registration and login to create tickets.”
</p>
<p>This allows both registered users and external customers to open tickets without mandatory logins.
</p>
<br />
<p>
<img <img width="828" height="561" alt="Screenshot 2025-09-01 182137" src="https://github.com/user-attachments/assets/990558ed-a3f9-4040-8831-b478e7113aca"/>
</p>
<p>
</p>
<br />



<p align="center">
  <h1>Configure Agents (Support Staff)</h1>
</p>



<strong>Admin Panel > Agents > Add New.</strong>
<p>
Agents are the help desk staff who will work on tickets.
</p>
<p>
Example entries:
Ben Crawford – Full access to Support Department
</p>
<br />
<p>
<img <img width="951" height="809" alt="Screenshot 2025-09-01 182410" src="https://github.com/user-attachments/assets/524b0adf-9324-4611-8375-f8ef5a95fcc7"/>
</p>
<p>
 Jane Doe – Full access to Support Department
<img width="952" height="813" alt="Screenshot 2025-09-01 182435" src="https://github.com/user-attachments/assets/fa90c704-ff38-4f65-ae63-a8218890e7b0"/>

<img width="957" height="397" alt="Screenshot 2025-09-01 182458" src="https://github.com/user-attachments/assets/1b04352e-afed-45c1-a5ce-13d2e87ffda6"/>



Agents should be assigned to appropriate roles, teams, and departments based on their job function.
</p>
<br />




<p align="center">
  <h1>Configure End Users (customers)</h1>
</p>



<strong>Admin Panel > Users > Add New.</strong>
<p>
End users are the customers who create tickets.
Example:
Karen – Internal user added to the system
</p>
<p>
</p>
<br />
<p>
<img <img width="643" height="389" alt="Screenshot 2025-09-01 182746" src="https://github.com/user-attachments/assets/867e6744-583e-473a-82c0-917d16f72623"/>
</p>

Repeat this process for any additional employees or customers who will be using the system.
<p>
</p>
<br />



<p align="center">
  <h1>Configure SLA (Service Level Agreement)</h1>
</p>



<strong>Admin Panel > Manage > SLA.</strong>
<p>
Sev-A – 1 hour response time, 24/7 coverage (Critical issues)
Sev-B – 4 hours response time, 24/7 coverage (Major issues)
Sev-C – 8 hours response time, business hours only (Low-priority issues)
</p>
<p>
</p>
<br />
<p>
<img <img width="828" height="535" alt="Screenshot 2025-09-01 182806" src="https://github.com/user-attachments/assets/d94ce8f0-bf22-4228-ac13-d19de8970702"/>

<img width="829" height="541" alt="Screenshot 2025-09-01 182818" src="https://github.com/user-attachments/assets/b942ca46-f0fd-40be-b604-6fd84b6ef577"/>

<img width="830" height="526" alt="Screenshot 2025-09-01 182828" src="https://github.com/user-attachments/assets/758a1d52-4a0b-47a2-b941-1792d237f6ee"/>
</p>
<p>
</p>
<br />



<p align="center">
  <h1>Configure Help Topics</h1>
</p>



<strong>Admin Panel > Manage > Help Topics.</strong>
<p>
 Help Topics guide users when submitting tickets, ensuring proper routing. Example topics:
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
</p>
<p>These topics make it easier for users to categorize their requests and for the system to auto-assign tickets to the right department/team.
</p>
<br />
<p>
<img <img width="828" height="548" alt="Screenshot 2025-09-01 182842" src="https://github.com/user-attachments/assets/7d3e5f91-7e28-4ddf-838e-be2ec38328d9"/>

<img width="827" height="549" alt="Screenshot 2025-09-01 182904" src="https://github.com/user-attachments/assets/37b05b06-e059-438c-82fd-878ab50b5967"/>

<img width="829" height="543" alt="Screenshot 2025-09-01 182915" src="https://github.com/user-attachments/assets/72ae8c1d-43c8-4d0d-b892-227af6245087"/>

<img width="833" height="539" alt="Screenshot 2025-09-01 182926" src="https://github.com/user-attachments/assets/f67fd52c-b651-4524-a079-348f9dca46d6" />

</p>
<p>
At this stage, osTicket has been fully configured with roles, departments, teams, agents, end users, SLA policies, and help topics. These post-installation steps are critical for ensuring tickets flow correctly, response times are tracked, and support staff have the right level of access.

With these configurations, your osTicket system is now ready to function as a robust help desk platform, capable of handling both internal IT support requests and external customer service issues efficiently.
</p>
<br />





