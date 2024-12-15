<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

## osTicket - Post-Install Configuration ##
> This tutorial outlines a post-install configuration demonstration of the open-source help desk ticketing system osTicket.
 - 🔗 Admin & Agent Login Page: `http://localhost/osTicket/scp/login.php`
 - 🔗 End User's osTicket Page: `http://localhost/osTicket` <br />
---

## Video Demonstration ##
### [<img src="https://img.icons8.com/?size=100&id=19318&format=png&color=000000" align="center" width="40" height="40">](https://www.youtube.com/channel/UC9YvuJxKB94ByhwCfZQ_5Kg) [Post Install Configuration](https://youtu.be/7HAPxk8Glic)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b>

<h2>Post-Install Configuration Objectives</h2>

1. Configure Roles ✔️
  - Grouping Permissions
    > Admin Panel -> Agents -> Roles, create 'King Admin' Role
2. Configure Departments ✔️
  - Ticket Visibility, Help Desk vs SysAdmins vs Networking 
    > Admin Panel -> Agents -> Departments, create 'SysAdmins' Department
3. Configure Teams ✔️
  - Pull Agents from different Departments 
    > Admin Panel -> Agents -> Teams, create 'Online Banking' Team
4. Allow all to create a ticket ✔️
    > Admin Panel -> Settings -> User Settings, uncheck 'unregistered users can create tickets' 
5. Configure Agents 'empolyees' & Configure Users 'customers' ✔️
  - Jenny, Department: SysAdmins & Johnny, Department: Support
    > Admin Panel -> Agents -> Add New
  - Ken & Karen
    > Agent Panel -> Users -> Add New
6. Configure SLA ✔️
  - Sev-A, Grace Period: 1 hour, Schedule: 24/7
  - Sev-B, Grace Period: 4 hours, Schedule: 24/7
  - Sev-C, Grace Period: 8 hours, Schedule: 24/7
     > Admin Panel -> Manage -> SLA
7. Configure Help Topics for Users creating tickets ✔️
  - Business Critical Outage
  - Personal Computer Issues
  - Equipment Request
  - Password Reset
  - Other
    > Admin Panel -> Manage -> Help Topics
---
<h2>Configuration Steps</h2>

<img src="https://github.com/user-attachments/assets/cfd86f53-4010-402c-b303-3be1de916df5"/>
<img src="https://github.com/user-attachments/assets/ec547d00-1ec0-4f14-ac52-21e95eaea3aa"/>
<img src="https://github.com/user-attachments/assets/206862d2-0879-42c5-a1dc-ae7cae11c2cd"/> <br />

1️⃣ Configure Roles, Departments, and Teams ⤵️
> 1. To group permissions, sign in to Admin Login Page. Follow path Admin Panel -> Agents -> Roles, click `Add New Agent`. Enter **Name**, **Email**, and check desired permissions on next tab.
> 2. To configure ticket visibility, follow path Admin Panel -> Agents -> Departments, click `Add New Department`. Choose **Parent** department from dropdown, fill out **Name**, and select **Type**. Configure other optional department settings if needed. 
> 3. To assign different Agents to specific teams within department and roles, follow path Admin Panel -> Agents -> Teams,  click `Add New Team`. Enter **Name** and **Status**.
---

<img src="https://github.com/user-attachments/assets/0cb21e98-032a-4a75-8b02-d9b9f47dfd2f" />
<img src="https://github.com/user-attachments/assets/4af933ca-ff06-4936-b95c-932db5e1da0d" /> <br />

2️⃣ Configure User Settings, Agents, and End Users ⤵️
> 1. To allow anyone the ability to create and submit a ticket, follow path Admin Panel -> Settings -> User Settings and ensure `Require registration and login to create tickets` box is unchecked.
> 2. To configure Agents follow path Admin Panel -> Agents -> click `Add Agent`. Enter **Name**, **Email Address**, and **Username**. Click `Set Password`, Uncheck `Send the agent a password reset email` to set Agents password and click `Update`. Assign desired Access, Permissions and/or Teams by clicking in corresponding tabs.
> 3. To configure Users follow path Agent Panel -> Users -> `Add User`. Enter user's **Email** and **Name**.
---

<img src="https://github.com/user-attachments/assets/c7c4b96b-d4c9-4aee-8f80-e1c9d269ffef" /> 
<img src="https://github.com/user-attachments/assets/29bb44dd-0c3a-4fc9-89a1-ab308e9e22e4" /> <br />

3️⃣ Configure Service Level Agreements and Help Topics 🏁
> 1. To create new SLA follow path Admin Panel -> Manage -> SLA, click `Add New SLA Plan`. Enter **Name**, **Grace Period**, and select **Status**.
> 2. To configure Help Topics for users creating tickets follow path Admin Panel -> Manage -> Help Topics, click `Add New Help Topic`. Enter **Topic**, select **Status** and **Type**.
---
