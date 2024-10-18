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

- This lab assumes that you have osTicket installed in your computer and have a login account setup. (My <a href="https://github.com/tonideeprai/osticket-prereqs">guide</a>.)

<h2>URL (optional)</h2>

These will help you go back and forth between diffferent pages quicker.<br>
- Admin/Analyst Login Page:<br>
<a href="http://localhost/osTicket/scp/login.php">http://localhost/osTicket/scp/login.php</a>
- End User osTIcket:<br>
<a href="http://localhost/osTicket">http://localhost/osTicket</a>

<h2>Let's get started!</h2>

<p><b>Acknowledge Agent Panel vs Admin Panel</b></p>
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
    Go to Agent > Roles > Add New Role > make a new role called "Supreme Admin" > assign all of the  permisssions to the role
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
      Go to Agent > Roles > Add New Role > make a new role called "Help Desk". assign the followin permissions to the role
  </p>
<p>
  <img width="90%" alt="Screenshot 2024-10-17 at 9 27 33 AM" src="https://github.com/user-attachments/assets/84e0c9a7-44ae-4821-a53a-08cf6efac590">
<img width="90%" alt="Screenshot 2024-10-18 at 9 30 00 AM" src="https://github.com/user-attachments/assets/c923e055-88c5-4e25-bbb7-26f7f31937ad">

</p>
