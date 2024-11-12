# osticket-post-install

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

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

<h2>Configuration Steps</h2>

<p>

<h2>Configure Roles (Used for grouping permissions)</h2>


Sign into osTicket and click the "Admin Panel" at the top right to start configuring.
![image](https://github.com/user-attachments/assets/4d55348d-c2b5-46db-8c1a-96f05eec3c93)


Admin Panel > Agents > Roles > "Add new role" > Supreme Admin
<p>Create "Supreme Admin" by clicking "add new role"

  ![image](https://github.com/user-attachments/assets/fd059424-c5a4-4c76-bbd3-a0dff94d4613)

<P>

<h2>Configure Departments (Ticket Visibility, Help Desk, SysAdmins, Networking)</h2>


Admin Panel > Agents > Department > "Add new role" > SysAdmins


![image](https://github.com/user-attachments/assets/31e40c1f-a53f-4997-9f73-d3c85ac2ac0a)

<p>

<h2>Configure Teams</h2>


Admin Panel > Agents > Department > "Add new team" > Online Banking


![image](https://github.com/user-attachments/assets/c78fae84-b8ce-4f58-9854-24be3dff4107)

<p>

<h2>User Ticket Creation</h2>

Before configuring more, we're going to give access to anyone to create tickets such as other users.

In order to do this, go to the user settings and (uncheck : unregistered users can create tickets)
![image](https://github.com/user-attachments/assets/b9733f1d-6898-437f-a828-5b53df5a5349)


<p>
  
</p>

<h2>Configure Agents (Workers)</h2>


Admin Panel > Agents > Add New

For this example, we'll use two names, Jane Doe and John Doe.
We'll add Jane to the SysAdmins Department with supreme access. While John will be apart of the Support Department with a view only access.
![image](https://github.com/user-attachments/assets/9deddf6b-3d24-4c1b-97fd-0ba733027514)


![image](https://github.com/user-attachments/assets/f0fa90e2-92d2-47ac-b59e-9480b3a830b4)


![image](https://github.com/user-attachments/assets/88b8fdf4-05d7-47c2-9688-2eac38164c35)


![image](https://github.com/user-attachments/assets/3d6e1e03-e445-4695-a4cb-a41801bf5a6e)

<p>

Once the steps above are completed, we're going to switch over to the "Agent Panel" at the top right and start to configure some users(customers)

![image](https://github.com/user-attachments/assets/97a5f695-abf5-4d04-8379-5663b8b69b62)

</p>
<h2>Switching to Agent Panel</h2>
In the Agent Panel we're going to proceed and create users Hayden and Karen.
Agent Panel > Users > Add New

![image](https://github.com/user-attachments/assets/90f262cc-dc36-4b2b-b2df-c526c4e2f789)


</p>

<h2>Configure SLA</h2>


After creating users through the Agent Panel, we're going to go back to the Admin Panel and configure SLA's.

Admin Panel > Mange > SLA

1. Sev-A (Grace Period: 1 Hour, 24/7)
![image](https://github.com/user-attachments/assets/1fcbfb14-e8f6-454b-9236-5a21d6dacd66)

2. Sev-B (Grace Period: 4 Hours, 24/7)
![image](https://github.com/user-attachments/assets/e5f86b44-92e2-4b09-b841-0f573fc3226f)

3. Sev-C (Grace Period: 8 Hours, Business Hours)
![image](https://github.com/user-attachments/assets/25629cb1-9257-4804-b078-5cbcbbf661b0)


![image](https://github.com/user-attachments/assets/184e725b-55ce-4707-b730-8f325c4c65a6)

<p>
  
<h2>Configure Help Topics (users create a ticket)</h2>


The final step in this is to configure some help topics for users to choose from when they come across a problem.


Admin Panel > Manage > Help Topics

1. Business Critical Outage
![image](https://github.com/user-attachments/assets/4ff3cef3-18ba-421f-91e9-bf3041882ff7)

2. Personal Computer Issues
![image](https://github.com/user-attachments/assets/eb12ff61-01f7-4bc8-9026-9adab1f0bb03)

3. Equipment Request
![image](https://github.com/user-attachments/assets/44c94385-0477-44ff-9ba4-8457199a2d5d)

4. Password Reset
![image](https://github.com/user-attachments/assets/a1fe0c54-2757-44c5-9aaf-f416b1ac00f8)

5. Other
![image](https://github.com/user-attachments/assets/95282e58-d4d0-42c3-8540-91f87ed83ef0)

</p>

This will conclude this post-installation of osTicket with configurations and managing between and Admin User and an Agent User!
