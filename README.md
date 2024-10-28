<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Installation Configuration</h1>
This lab is a showcase of configuration and assigning permissions to employee users in osTIcket.<br/>
* This lab is done using a virtual machine in Azure. Here are my <a href="google.com" styl>lab</a> showcases *

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Prerequisites</h2>

- osTicket Installation (my <a href="https://github.com/tonideeprai/osticket-prereqs">guide</a>.)

<h2>URL (optional)</h2>

These will help you go back and forth between diffferent pages quicker.<br>
- Admin/Analyst Login Page:<br>
<a href="http://localhost/osTicket/scp/login.php">http://localhost/osTicket/scp/login.php</a>
- End User osTIcket:<br>
<a href="http://localhost/osTicket">http://localhost/osTicket</a>

<h2>Let's get started!</h2>

<h3>Acknowledge Agent Panel vs Admin Panel</h3>
<p>
After loggin in, notice that you can switch between <b>Admin Panel</b> and <b>Agent Panel</b>

  - **Admin Panel** allows to assign roles and create other users, departmanets, teams, etc.
  - **Agent Panel** is where you will be working as IT help desk in this lab
</p>
<p>
  <img width="90%" alt="Screenshot 2024-10-17 at 8 57 54 AM" src="https://github.com/user-attachments/assets/21745dc6-6242-4a34-b78d-e0cc31c8f321">
  </p>
  <p><b>Configure Supreme Admin <a href="https://docs.osticket.com/en/latest/Admin/Agents/Roles.html">Role</a></b></p>
  <p>Under <b>Admin Panel</b><br>
     Agent -> Roles -> Add New Role -> make a new role called "Supreme Admin" -> assign all of the  permisssions to the role
  </p>
  <p>
    <img width="90%" alt="Screenshot 2024-10-17 at 9 09 25 AM" src="https://github.com/user-attachments/assets/86fc456a-67a3-4b5b-834a-9148a665193d">
<img width="90%" alt="Screenshot 2024-10-17 at 9 10 32 AM" src="https://github.com/user-attachments/assets/2d121ddc-22a7-4808-8cd2-85d86698bcb5">
<img width="90%" alt="Screenshot 2024-10-17 at 9 11 11 AM" src="https://github.com/user-attachments/assets/9cd1d96c-6966-448e-8b23-d8b2a793b283">
<img width="90%" alt="Screenshot 2024-10-17 at 9 14 25 AM" src="https://github.com/user-attachments/assets/f8fe739a-1fb2-42c0-8cfb-46ba51d72a84">
  </p>
  <p><b>Configure Help Desk <a href="https://docs.osticket.com/en/latest/Admin/Agents/Roles.html">Role</a></b></p>
  <p>
    <p>Under <b>Admin Panel</b><br>
     Agent -> Roles -> Add New Role -> make a new role called "Help Desk" -> assign the following permissions to the role
  </p>
<p>
  <img width="90%" alt="Screenshot 2024-10-17 at 9 27 33 AM" src="https://github.com/user-attachments/assets/84e0c9a7-44ae-4821-a53a-08cf6efac590">
<img width="90%" alt="Screenshot 2024-10-18 at 9 30 00 AM" src="https://github.com/user-attachments/assets/c923e055-88c5-4e25-bbb7-26f7f31937ad">
<img width="1512" alt="Screenshot 2024-10-20 at 2 09 28 PM" src="https://github.com/user-attachments/assets/245dbcaa-41e6-4a80-a929-5c9a817b0ed5">
</p>
<p> <b>Configure SysAdmins <a href="https://docs.osticket.com/en/latest/Admin/Agents/Departments.html">Department</a></b></p><br>
<p>Under <b>Admin Panel</b><br>
     Agent -> Departments -> Add New Department -> make a new department called "SysAdmins".
  </p>
  <p>
<img width="90%" alt="Screenshot 2024-10-20 at 2 24 59 PM" src="https://github.com/user-attachments/assets/d4838f59-177a-4898-add4-727aa6427349">
<img width="90%" alt="Screenshot 2024-10-20 at 2 26 21 PM" src="https://github.com/user-attachments/assets/a18cafbc-b1c7-4a57-a0af-b26a32f07dee">
<img width="90%" alt="Screenshot 2024-10-20 at 2 28 34 PM" src="https://github.com/user-attachments/assets/12073503-3f29-4543-ac05-5e61d10c30ba">
  </p>
  <p><b>Configure Online Banking <a href="https://docs.osticket.com/en/latest/Admin/Agents/Teams.html">Team</a></b></p>
  <p>Under <b>Admin Panel</b>
  <p>
    Agents -> Teams -> Add New Team -> name it "Online Banking"
  </p>
  <p>
    <img width="90%" alt="Screenshot 2024-10-20 at 2 34 17 PM" src="https://github.com/user-attachments/assets/cfb3577a-4457-4f5c-b603-5846ddb66d5b">
<img width="90%" alt="Screenshot 2024-10-20 at 2 35 00 PM" src="https://github.com/user-attachments/assets/2de16b9f-92ce-4fbd-b28e-cee65366015a">
<img width="90%" alt="Screenshot 2024-10-20 at 2 36 32 PM" src="https://github.com/user-attachments/assets/f48c19c3-a03a-46c9-a9f2-6d84aa4dcc01">
  </p>
  <p><b>Allow anyone to create tickets</b></p>
  <p>Under <b>Admin Panel</b></p>
  <p>
     Settings -> Users (UNCHECK: unregistered users can create tickets)
   <ul>
     <li>Registration Required: Require registration and login to create tickets</li>
   </ul>
  </p>
  <p>
    <img width="90%" alt="Screenshot 2024-10-20 at 2 40 34 PM" src="https://github.com/user-attachments/assets/c8c03f65-dc00-4110-ac33-5de078aaf89f">
<img width="90%" alt="Screenshot 2024-10-20 at 2 46 36 PM" src="https://github.com/user-attachments/assets/38f6373a-b48a-4f2d-abff-40f4f98d9982">
  </p>
  <p><b>Configure <a href="https://docs.osticket.com/en/latest/Admin/Agents/Agents.html">Agents (workers)</b></p>
  <p>Under <b>Admin Panel</b></p>
  <p>
    Agent -> Add New Agent
    <ul>
    <li>Jane Doe (Dept: SysAdmins, Role: Supreme Admin, Team: Online Banking)</li>
    <li>Alex Blues (Dept: Support, Role: Help Desk, Team: no team (he'll be an IT help desk support)</li>
   </ul>
  </p>
  <p>
    <img width="90%" alt="Screenshot 2024-10-20 at 2 50 31 PM" src="https://github.com/user-attachments/assets/77629dba-4a75-4374-9e95-409a5c7b7837">
    <img width="90%" alt="Screenshot 2024-10-20 at 4 31 11 PM" src="https://github.com/user-attachments/assets/0a4995e0-e244-45e0-aad9-a3174a4bbba0">
<img width="90%" alt="Screenshot 2024-10-20 at 2 54 34 PM" src="https://github.com/user-attachments/assets/19401671-2942-4389-9d9f-eec3ec5d9055">
<img width="90%" alt="Screenshot 2024-10-20 at 3 17 55 PM" src="https://github.com/user-attachments/assets/44e24887-3d5f-4684-88c3-d653d7ba95c0">
<img width="90%" alt="Screenshot 2024-10-20 at 4 25 46 PM" src="https://github.com/user-attachments/assets/39555124-035c-41a6-b7c6-7e3bb6767df2">
<img width="90%" alt="Screenshot 2024-10-20 at 4 38 22 PM" src="https://github.com/user-attachments/assets/ba087fdb-4980-48e1-bf11-64d2c3e3be64">
  </p>
  <p><b>Configure <a href="https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html">Users (customers)</a></b></p>
  <p>Under <b>Agent Panel</b></p>
  <p>
    Users -> Add User
    <ul>
      <li>Sarah</li>
      <li>Coby</li>
    </ul>
  </p>
  <p>
    <img width="90%" alt="Screenshot 2024-10-20 at 4 41 39 PM" src="https://github.com/user-attachments/assets/029d4a31-563e-4e00-a824-bfaf8925e854">
  <img width="90%" alt="Screenshot 2024-10-20 at 4 43 26 PM" src="https://github.com/user-attachments/assets/c2835ad8-da53-4dd4-bbda-5411c6f4a4c7">
  <img width="90%" alt="Screenshot 2024-10-20 at 4 45 12 PM" src="https://github.com/user-attachments/assets/0e0ff70c-e1fe-4523-88bd-9ad22f147fbc">
  </p>
  <p><b>Configure <a href="https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html">SLA</a></b></p>
  <p>Under <b>Admin Panel</b></p>
  <p>
    Manage -> SLA -> Add New SLA Plan
    <ul>
      <li>Sev-A (Grace Period: 1 hour, Schedule: 24/7)</li>
      <li>Sev-B (Grace Period: 4 hours, Schedule: 24/7)</li>
      <li>Sev-C (Grace Period: 8 hours, Business Hours)</li>
    </ul>
  </p>
  <p>
    <img width="90%" alt="Screenshot 2024-10-20 at 4 52 34 PM" src="https://github.com/user-attachments/assets/9a228c45-38c9-4ba5-8ed3-fcbb94fdc83f">
    <img width="90%" alt="Screenshot 2024-10-20 at 4 56 01 PM" src="https://github.com/user-attachments/assets/101e623d-3871-40a7-984e-c7678b79eeda">
    <img width="90%" alt="Screenshot 2024-10-20 at 5 01 11 PM" src="https://github.com/user-attachments/assets/9a50e214-787c-4345-9891-838e2343ac60">
  </p>
  <p><b>Configure <a href="https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html">Help Topics</a> (For when users create a ticket)</b></p>
  <p>Under <b>Admin Panel</b></p>
  <p>
    Manage -> Help Topics -> Add New Help Topic
    <ul>
      <li>Business Critical Outage (Parent Topic: Report a Problem)</li>
      <li>Personal Computer Issues (Parent Topic: Report a Problem)</li>
      <li>Equipment Request (Parent Topic: General Inquiry)</li>
      <li>Password Reset (Parent Topic: Report a Problem/ Access Issue</li>
      <li>Other (Parent Topic: General Inquiry</li>
    </ul>
  </p>
  <p>
    <img width="90%" alt="Screenshot 2024-10-20 at 5 17 47 PM" src="https://github.com/user-attachments/assets/0bc8c27d-7418-444b-b95a-2fe99457edb1">
    <img width="90%" alt="Screenshot 2024-10-20 at 5 20 36 PM" src="https://github.com/user-attachments/assets/d44b32ef-1078-4242-97d2-6c802d4e17ae">
    <img width="90%" alt="Screenshot 2024-10-20 at 5 26 26 PM" src="https://github.com/user-attachments/assets/6858c3b7-0e9a-45a8-92c2-3c95ef707c14">
  </p>
