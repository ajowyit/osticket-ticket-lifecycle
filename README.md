<p align="center">
<img width="900" alt="Screenshot 2025-04-27 at 7 28 04 PM" src="https://github.com/user-attachments/assets/e350f934-ca85-4e5e-9937-6eae6811f8c5" />

</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial goes over the lifecycle of a ticket in a ticketing system from intake to resolution within osTicket.
<br/>

<h2>⚠️ Prerequisites</h2>

- [Creating Virtual Machines in the Cloud](https://github.com/ajowyit/creating-virtual-machines)
- [osTicket: Prerequisites and Installation](https://github.com/ajowyit/osticket-prereqs)
- [osTicket: Post-Installation Configuration](https://github.com/ajowyit/osticket-post-install-config)

<h2>💻 Environments and Technologies</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Windows App (macOS)
- Internet Information Services (IIS)

<h2>👨‍💻 Operating Systems</h2>

- macOS Sequoia
- Windows 10 (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>♻️ Lifecycle Stages</h2>

<p>
<img width="1030" alt="Screenshot 2025-06-16 at 6 23 49 PM" src="https://github.com/user-attachments/assets/b343a831-d2ef-4f39-89f9-a9fad8be0b24" />
</p>

<p>- Before we get started with creating and working tickets today, there was an issue discovered within osTicket about 30 mintues ago. We had a couple of clients call and ask for an update concerning some Help Desk Tickets they submitted. After several attempts, our Lead Agent was unable to locate the tickets. Then, the Lead Agent submitted a "Test" ticket via the Support Center portal and was unable to locate the "Test" ticket as well. Tickets are being created successfully but our Agents are not able to see them. The Help Desk Manager has exclated the issue to our Admin Team. Lets go solve this issue.    </p>
<p>
  - Go to the Admin / Agent Portal for osTicket. (http://localhost/osTicket/scp/login.php)
</p>
<p>
  - Log in as an Admin. Username: "adminuser" | Password: Password1
</p>
<br/>

<table>
  <tr>
    <td>
      <img width="1000" alt="TL2" src="https://github.com/user-attachments/assets/d8c57ea8-dccc-4035-aa1f-a52999a76c45" />
    </td>
    <td>
      <img width="1000" alt="TL3" src="https://github.com/user-attachments/assets/c3158223-20fb-4fc7-a287-3298f01b23c2" />
    </td>
  </tr>
</table>
<p>- Upon further investigation and working with Osticket Support, we discovered that a recent update caused a bug with a preset Department within osTicket. The bug is causing the tickets to be sent to the Maintenance Department regardless of the configurations. We will delete this department to get operations back to normal while osTicket works on a patch. </p>
<p>
  - From the Admin Panel, click -> Agents -> Departments. 
</p>
<p>
  - Check the box by Manitenance. Click the More dropdown arrow. Click Delete from the dropdown menu.
</p>

<table>
  <tr>
    <td>
      <img width="1000" alt="TL4" src="https://github.com/user-attachments/assets/e520d2a9-1a31-4592-9ef8-1024d6406d63" />
    </td>
    <td>
      <img width="1000" alt="TL5" src="https://github.com/user-attachments/assets/28aab28a-25e8-4176-8a90-96aa0430b7c0" />
    </td>
  </tr>
</table>
<p>
  - Click "Yes, Do it!".
</p>
<p>- The Maintenance Department has successfully been deleted. We had our Agents log out / log back in to osTicket. They are reporting that the tickets are now visible and being routed to the correct Departments. That is a Win! Now, we can get to creating and working tickets. 😎</p>
<br/>

<table>
  <tr>
    <td>
      <img width="1000" alt="TL6" src="https://github.com/user-attachments/assets/6b35cc6e-519d-4ec3-9f75-20c3f655d173" />
    </td>
    <td>
      <img width="1000" alt="TL7" src="https://github.com/user-attachments/assets/52233b24-a17c-47c3-a143-686a130ac711" />
    </td>
  </tr>
</table>
<p>
  - Open the Support Center. In the browser navigate to http://localhost/osTicket.
</p>
<p>-
  Click the blue button that says "Open a New Ticket". Create a ticket as Karen.
</p>
<p>
  - Enter the folllowing - Email Address: karen@lognpacific.com | Full Name: Karen | Help Topic: Report a Problem.
</p>
<p>- Fill out Issue Summary. In the smaller text field for the heading type in, "Entire mobile/online banking system is down". In the larger text field for the summary type in "My employees are reporting that users are not longer able to access the online banking portal. The ones who can occassionally access it, cannot log in.". Scroll down and click "Create Ticket".
</p>

<table>
  <tr>
    <td>
      <img width="1000" alt="TL8" src="https://github.com/user-attachments/assets/15281ad1-cbff-4c2b-8aeb-cc25c23a9acf" />
    </td>
    <td>
      <img width="1000" alt=<"TL9" src="https://github.com/user-attachments/assets/73284ce1-d5dc-4285-a4ca-50c72a8c0f3f" />
    </td>
  </tr>
</table>

<p>- New create is successfully created.
<p>- Now, log in to the Admin / Agent Portal as John Doe. Username: john_doe | Password: Password1 </p>

<p>
<img width="750" alt="TL10" src="https://github.com/user-attachments/assets/49cabd55-cb06-48ba-9f64-3957da5a686a" />
</p>

<p>- Once logged in, click Tickets -> Open.</p>
<p>- This will display all the open tickets. Locate the ticket we just created as Karen and open it.</p>
<br/>

<p>
<img width="750" alt="TL11" src="https://github.com/user-attachments/assets/cea365f7-922e-4e1a-bb9c-8d2edf2af42b" />
</p>

<p>- Take a minute to review the ticket details. Based off the issue stated by Karen, this seems like a serious problem. </p>
<p>- In the real world, we would contact Karen via phone, email, or direct message to find out more. We'll pretend we spoke with Karen and confirmed the issue is serious. Next, we'll update the SLA, the Help Topic, and assign the ticket to the correct team.</p>
<br/>

<table>
  <tr>
    <td>
      <img width="1000" alt="TL13" src="https://github.com/user-attachments/assets/740f2a30-e8c8-479f-a9b3-cdfbd4b6ede4" />
    </td>
    <td>
      <img width="1000" alt=<<img width="745" alt="TL14" src="https://github.com/user-attachments/assets/95062ddf-923b-40e2-89ae-8c100c3d705d" />
    </td>
  </tr>
</table>

<p>- Click "Deault SLA". In the pop-up, Select Sev-A and enter a comment as to why you are updtaing the SLA Plan. Click Update. See Figure 12</p>
<p>- Next, click "Help Topic". Use the dropdown to select "Report a Problem / Business Critical Outage". Comment reason and click Update.</p>
<p>- Making these changes will help our team process the ticket accordingly and effectively.</p>
<br/>

<table>
  <tr>
    <td>
      <img width="1000" alt="TL13" src="https://github.com/user-attachments/assets/740f2a30-e8c8-479f-a9b3-cdfbd4b6ede4" />
    </td>
    <td>
      <img width="1000" alt=<<img width="745" alt="TL14" src="https://github.com/user-attachments/assets/95062ddf-923b-40e2-89ae-8c100c3d705d" />
    </td>
  </tr>
</table>

<p>- Now, click "Unassigned" and assign the ticket to Online Banking. Comment and click Assign.
<p>- Review the changes we made and scroll down. </p>
<br/>

<p>
<img width="750" alt="TL17" src="https://github.com/user-attachments/assets/a0b42e33-c48b-408c-80d5-15b3b64844f5" />
</p>

<p>- osTicket keeps a track record of all the changes in the Ticket Thread.</p> 
<p>- This helps us track who did what with the ticket and keeps everyone updated. </p>
<br/>

<table>
  <tr>
    <td>
      <img width="900" alt="TL18" src="https://github.com/user-attachments/assets/f7b30731-f58a-453e-81dc-01454d65bfd0" />
    </td>
    <td>
      <img width="1000" alt="TL19" src="https://github.com/user-attachments/assets/168d7688-6699-4601-b78a-daa715207d02" />
    </td>
  </tr>
</table>

<p>- Log John out and log in to the Agent Portal as Jane Doe. Username: jane_doe | Password: Password1</p>
<p>- We will work and resolve this ticket as Jan Doe moving forward. </p>
<p>- John assigned the ticket to Online Banking and Jane is on that team. Open the ticket.</p>
<br/>

<p>
<img width="750" alt="TL20" src="https://github.com/user-attachments/assets/8e5c64d8-6f0f-459e-8da7-5c7a36a6183a" />
</p>

<p>- Assign the ticket to Jane to reflect which Agent will be working the ticket. Pretend that Online Banking has more then one Agent.</p> 
<p>- Having the ticket assigned to a specific Agent will help with tracking. </p>
<br/>

<table>
  <tr>
    <td>
      <img width="1000" alt="TL21" src="https://github.com/user-attachments/assets/55c991a0-5edc-46c3-a49d-8146eb9f8902" />
    </td>
    <td>
      <img width="1000" alt="TL22" src="https://github.com/user-attachments/assets/719982a0-e45a-4d58-b908-9a83014025bc" />
    </td>
  </tr>
</table>

<p>- Select "Jane Doe" as Assignee and enter comment of the change. Click Assign.</p>
<p>- Now, look at the "Assigned To" section of the ticket.</p>
<p>- It shows the ticket is assigned to Jane Doe of the Online Banking team.</p>
<br/>

<table>
  <tr>
    <td>
      <img width="1000" alt="TL23" src="https://github.com/user-attachments/assets/58008400-3562-455d-aed2-f3c2050ea108" />
    </td>
    <td>
      <img width="1000" alt="TL24" src="https://github.com/user-attachments/assets/d883f2e7-d0ea-4646-aa38-6c10932b137b" />
    </td>
  </tr>
</table>

<p>- Next, we'll send an update to Karen concerning the ticket she submitted. Click Post Reply. See Figure 22</p>
<p>- Now, lets notify Karen that we determined a cause for the issue, it has been addressed, and online banking is working again. See Figure 23 </p>
<p>- Click Post.</p>
<br/>

<table>
  <tr>
    <td>
      <img width="1000" alt="TL25" src="https://github.com/user-attachments/assets/f3fe340b-626e-4254-9786-d3dca29c44ff" />
    </td>
    <td>
      <img width="1000" alt="TL26" src="https://github.com/user-attachments/assets/a0722cec-a764-467f-a1e7-91549430cd2b" />
    </td>
  </tr>
</table>

<p>- Figure 24 shows us how osTicket records Jane's respones in the Ticket Thread as well.</p>
<p>- Now that the issue has been fixed and the end user has been updated, lets close out the ticket.  </p>
<p>- Click Status and select Resolved.</p>
<br/>

<table>
  <tr>
    <td>
      <img width="900" alt="TL27" src="https://github.com/user-attachments/assets/ff775d52-483e-4c1d-949e-ce018893de56" />
    </td>
    <td>
      <img width="1000" alt="TL28" src="https://github.com/user-attachments/assets/18a9c367-3e2a-4531-9249-708f78f33431" />
    </td>
  </tr>
</table>

<p>- In the pop-up, change the Status to Resolved. Comment the change and click Close.</p>
<p>- Ticket #206084 has been resolved. </p> 
<p>- You have successfully created, worked, and resolved a Help Desk ticket within osTicket! </p>
<br/>

<h2>Conclusion</h2>

<p>This concludes our project. We have successfully navigated through the life cycle of a Help Desk ticket within osTicket. I recommend taking the time to play around in osTicket by creating and working different tickets. Use your imagination and have fun being your own Help Desk! Don't forget to Stop (turn off) the VMs in Azure. As always, Thank You for your time and viewing this Project. We'll see you on the next one! 😎      
</p>
<br/>





