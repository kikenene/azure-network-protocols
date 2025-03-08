<p align="center">

![active directory](https://github.com/user-attachments/assets/790d6de2-969c-4362-be31-31e0da8dad64)
</p>

<h1>Deploying Active Directory within Virtual Machines and creating Users within them to allow multiple users to login the Directory.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Active Directory
- Powershell ISE

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Windows 2022 Server

<h2>High-Level Steps</h2>

- Deploy Active Directory in Domain Control Server
- Setup Remote Desktop for Client 1 Users
- Open Powershell ISE
- Paste script in Powershell and run it
- Create over 1000 new users
- Login to Client-1 VM as newly created user

<h2>Actions and Observations</h2>

<p>
  
![step 0 created and deployed active directory](https://github.com/user-attachments/assets/eea7bf61-43dd-412b-99fe-d0a07055acea)

</p>
<p>
Created and deployed active directory in the Domain Control Server and created Organizational Units for Employees, Admins and Clients.
</p>
<br />

<p>
  
![step 1 rdp domain users](https://github.com/user-attachments/assets/82950119-1414-4863-96ee-41d495ec5792)

![step 1 rdp add domain users](https://github.com/user-attachments/assets/23a34f0d-9c3a-4cf8-8cee-01b9dfd1ae5f)

</p>
<p>
Opened System and allowed Domain users access to the remote desktop. Being able to log into Client-1 as a regular, non-administrative user.
</p>
<br />

<p>
  
![step 2 copy script](https://github.com/user-attachments/assets/80e3ec85-0b25-4f41-9e6c-6beeb6df7cdb)

![step 2 open powershell ISE](https://github.com/user-attachments/assets/491d4b8f-43a1-416c-aa67-d40f8cb4b29e)

![step 2 paste raw script file in ise](https://github.com/user-attachments/assets/c1659a5a-1496-462b-860a-2015886c2497)

</p>
<p>
Got a github script and copied the script raw. Then, opened up DC-1 server and opened Powershell ISE as an administrator. After that, created a new file and pasted the script into the file.
</p>
<br />

<p>
  
![step 3 run script](https://github.com/user-attachments/assets/0052699c-2328-4452-ac5a-79212ebf06c1)

</p>
<p>
I ran the script and then Powershell started to create over 1000 users into the _EMPLOYEES folder.
</p>
<br />

<p>
  
![step 4 observe new users created in _employee folder active directory](https://github.com/user-attachments/assets/3f346158-ba4f-4b37-91df-1f541c065245)

</p>
<p>
These are the users that are continuously being created by the script inside the _EMPLOYEES folder. 
</p>
<br />

<p>
  
![step 5 login in client 1 as new user created by script](https://github.com/user-attachments/assets/f73df59a-8ca6-42f9-91a5-9a43e5089fde)

![step 5 login as user and observe that it worked](https://github.com/user-attachments/assets/b1a7bf61-623d-49aa-bfd1-0427ec9b97e6)

</p>
<p>
Now users can access the Client-1 Virtual Machine. All the users have the same password. The username is "mydomain.com\user." Ultimately, the login was successful, showcasing the user in the command line and File Explorer.
</p>
<br />
