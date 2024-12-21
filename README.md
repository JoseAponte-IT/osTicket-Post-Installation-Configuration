<img src="https://i.imgur.com/tUnlhRz.jpeg" height="80%" width="80%" alt="Setting Up in Azure"/>

# Configuring osTicket: Departments, Roles, and Help Topics
This project demonstrates how to configure the osTicket ticketing system by setting up departments, agents, users, roles, permissions, and teams. Additionally, we streamline the ticketing process for both clients and support engineers by configuring help topics. This project showcases a foundational understanding of ticketing systems along with technical proficiency in system configuration, role management, and ticketing system optimization. 🫡

<h1>osTicket: Post-Installation Configuration</h1>


<h2>Tools & Technology Used</h2>

- osTicket: A widely-used open-source ticketing system for customer support.
- Microsoft Azure: Cloud platform for hosting the Windows 10 virtual machine.
- Windows 10 VM: Virtual environment used for hosting and configuring the ticketing system.
- RDP: Remote Desktop Protocol for securely accessing the Azure-hosted VM.

<h2>Key Objectives:</h2>

- Role-Based Configuration: Define and assign roles, permissions, and teams within osTicket, ensuring proper access and     workflow management.
- Department Setup: Organize support operations by creating and configuring departments to handle specific ticket         categories.
- User and Agent Management: Configure user profiles and assign agents to teams to streamline task delegation and         collaboration.
- Help Topics Optimization: Create help topics to simplify the ticket submission process for clients and improve         efficiency for support engineers.
- Remote Access: Use Remote Desktop Protocol (RDP) to securely access and manage the VM.

<h2>Prerequisites</h2>

- Completed the previous lab: osTicket: Prerequisites and Installation
- Microsoft RDP: If on MAC go to APP Store and download Microsoft RDP

# Project Overview
<h2>Step 1: Access Admin Configuration Panel</h2>
<p>Login to osTicket portal as an admin using this link in your Vm http://localhost/osTicket/scp/login.php </p>

- Once logged in, navigate to the Admin Panel by clicking "Admin Panel" located in orange at the top right of the page 

<img src="https://imgur.com/xcM6UZs.png" height="80%" width="80%" alt="Setting Up in Azure"/>

<h2>Step 2: Creating and Configuring an Admin role </h2>

- Navigate to the "Agents" tab and click on "Roles" underneath the "Agents" tab. Enter a role name

<img src="https://i.imgur.com/n3nofNe.png" height="80%" width="80%" alt="Setting Up in Azure"/>

- Navigate to the "Permissions" tab of this role and give this role all permissions in "Tickets", "Tasks", and "Knowledgebase"

- This will be our "Supreme Admin" Role

<img src="https://i.imgur.com/THRJLuc.png" height="80%" width="80%" alt="Setting Up in Azure"/>

<h2>Step 3: Setup Departments </h2>

 - While still in the "Agents" tab, click on "Departments" located just below the "Agents" tab

 - Name the department "System Administrators" and create the Department

<img src="https://i.imgur.com/qOwlzfl.png" height="80%" width="80%" alt="Setting Up in Azure"/>

<h2>Step 4: Setup Teams  </h2>

- Navigates to the "Teams" tab, while still in the "Agents" tab

- Then, name the team "Level II Support" and click create team:  

<img src="https://imgur.com/JuIruUo.png" height="80%" width="80%" alt="Setting Up in Azure"/>

<h2>Step 5: Setup Ticekt permissions  </h2>

- Now lets allow users to create tickets

- Navigate to the "Settings" Tab, now under "Authentication Settings" make sure that "Require registration and login to create tickets" is unchecked

<img src="https://imgur.com/Ht7SvW1.png" height="80%" width="80%" alt="Setting Up in Azure"/>

<h2>Step 6: Create Agents (Support Engineers) </h2>

-  Navigate back to the "Agents" tab and select "Agents" and fill out the name, email, and username

<img src="https://i.imgur.com/FsNvEld.png" height="80%" width="80%" alt="Setting Up in Azure"/>

- Next to the username click "Set Password" set the password

- Uncheck the "Send the agent a password reset email" and "Require password change at next login" options 

<img src="https://i.imgur.com/GpPt8kl.png" height="80%" width="80%" alt="Setting Up in Azure"/>

- On the "Access" tab for this user select the "System Administrators" department and the "Supreme Admin" role created earlier:  <br/>

<img src="https://i.imgur.com/2qKTmwN.png" height="80%" width="80%" alt="Setting Up in Azure"/>

- Under the "Teams" tab select "Level II Support" for this agent

<img src="https://i.imgur.com/STRiujN.png" height="80%" width="80%" alt="Setting Up in Azure"/>

- Create one more agent as done previously, the only difference is in the "Access" tab select "Support" for the department

<img src="https://i.imgur.com/wE8r7rv.png" height="80%" width="80%" alt="Setting Up in Azure"/>

<img src="https://i.imgur.com/ej19YSn.png" height="80%" width="80%" alt="Setting Up in Azure"/>


- Navigate to the "Agent Panel, " next to create a user (the customers) switch to the "Agent Panel" in orange in the top right -> Users -> Add User and put an email and name, then create.


- Repeat and make one more user   

<img src="https://i.imgur.com/1X9dwtB.png" height="80%" width="80%" alt="Setting Up in Azure"/>

<h2>Step 7: Configure SLA  </h2>

- Navigate back to Admin Panel - > Manage -> SLA create three SLAs with different severities, grace periods, and schedules 

<img src="https://i.imgur.com/WnlOPeB.png" height="80%" width="80%" alt="Setting Up in Azure"/>

<img src="https://i.imgur.com/d87knx3.png" height="80%" width="80%" alt="Setting Up in Azure"/>

<img src="https://i.imgur.com/joZz8vM.png" height="80%" width="80%" alt="Setting Up in Azure"/>

<h2>Step 8: Setup Help Topics </h2>

- Under the same "Manage" - > "Help Topics" tab - > create four help topics named, "Business Critical Outage", "Personal Computer Issues", "Equipment Request", and "Password Reset" all with the same settings

<img src="https://i.imgur.com/0cfRoqa.png" height="80%" width="80%" alt="Setting Up in Azure"/>


# 🎉Congratulations

 OsTicket is up and running and fully configured for use 🌝. In the next lab we will create tickets and resolve them as a support engineer. Familarizing ourselves with ticket life cycles, SLA, and GOOD 'OL TROUBLESHOOTING🤓.

<h2>We Have Successfully:</h2>

- Configured a ticketing system by setting up departments, agents, users, roles, permissions, and teams.

- Streamlined the ticket process for both clients and support engineers by creating help topics.

- Hosted and managed the ticketing system using a Microsoft Azure Windows 10 Virtual Machine.

- Accessed the Virtual Machine securely through RDP for seamless configuration and management.

# That Concludes this lab<img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px"/>

In the next and last lab we will learn about ticket lifecycles and how to troubleshoot tickets correctly.
