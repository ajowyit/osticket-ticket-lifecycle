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
      <img width="1029" alt="Screenshot 2025-06-16 at 6 31 42 PM" src="https://github.com/user-attachments/assets/1b8c58eb-e9e6-4c53-9007-c0053974d1ef" />
    </td>
    <td>
      <img width="1030" alt="Screenshot 2025-06-16 at 6 32 29 PM" src="https://github.com/user-attachments/assets/68ad7256-7374-4aa6-bfd5-20c8ea54d33e" />
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
      <img width="1023" alt="Screenshot 2025-06-16 at 6 34 42 PM" src="https://github.com/user-attachments/assets/0752e322-336d-43b5-ae75-ab8256bff6b4" />
    </td>
    <td>
      <img width="1030" alt="Screenshot 2025-06-16 at 6 37 14 PM" src="https://github.com/user-attachments/assets/b282dfff-c3dc-4c01-9b56-3aa5523ef2ea" />
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
      <img width="1034" alt="Screenshot 2025-06-16 at 6 46 02 PM" src="https://github.com/user-attachments/assets/1c0071f7-54f2-475e-9098-f6cce7edb1af" />
    </td>
    <td>
      <img width="1021" alt="Screenshot 2025-06-16 at 6 51 06 PM" src="https://github.com/user-attachments/assets/9e8a7b16-edf1-4ea7-8143-d28f5cf6d677" />
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
      <img width="962" alt="Screenshot 2025-06-17 at 4 24 29 PM" src="https://github.com/user-attachments/assets/26c818ed-e6ca-4627-8861-3464b233efcb" /> 
    </td>
    <td>
      <img width="866" alt="Screenshot 2025-06-17 at 4 25 51 PM" src="https://github.com/user-attachments/assets/768f2445-83bb-4665-bf6d-07c897d41eee" />
    </td>
  </tr>
</table>

<p>
  - You should see a confirmation that a support ticket request was created.
<p>
  - Next, log in to the Admin/Agent Portal as John Doe. Username: john_doe | Password: Password1 
</p>

<p>
  <img width="890" alt="Screenshot 2025-06-17 at 4 27 13 PM" src="https://github.com/user-attachments/assets/df82fcc7-2a39-48e5-b408-fd318866c461" />
</p>

<p>
  - After we are logged in, make sure to navigate to Tickets -> Open.
</p>
<p>
  - We should be able to see all the open tickets. Find the ticket we just created as Karen. Clikc on it to open it.
</p>
<br/>

<p>
<img width="994" alt="Screenshot 2025-06-17 at 4 33 58 PM" src="https://github.com/user-attachments/assets/55398d73-3691-4a01-8bc7-19219e817fed" />
</p>

<p>
  - Review the ticket details. Based off the issue stated by Karen, this seems like a serious problem.
</p>
<p>
  - In the real world, we might contact Karen via phone, email, or direct message to find out more from her. Let's pretend we spoke with Karen and confirmed that the issue is serious. Next, let's update the SLA, the Help Topic, and assign the ticket to the correct team.
</p>
<br/>

<table>
  <tr>
    <td>
      <img width="998" alt="Screenshot 2025-06-17 at 4 36 09 PM" src="https://github.com/user-attachments/assets/bf2eb644-6210-410e-8170-4853e835b540" />
    </td>
    <td>
      <img width="996" alt="Screenshot 2025-06-17 at 4 36 43 PM" src="https://github.com/user-attachments/assets/17c43ff2-c477-4fb8-91c7-8b2a24087e62" />
    </td>
  </tr>
</table>

<p>
  - Click "Deault SLA". In the pop-up, select Sev-A. Write a comment as to why you are updtaing the SLA Plan to Sev-A. Click "Update".
</p>

<table>
  <tr>
    <td>
      <img width="998" alt="Screenshot 2025-06-17 at 4 37 26 PM" src="https://github.com/user-attachments/assets/6b7dce6f-019f-4e15-94f7-5168fa17319c" />
    </td>
    <td>
      <img width="993" alt="Screenshot 2025-06-17 at 4 41 00 PM" src="https://github.com/user-attachments/assets/9d5f6f1b-08fa-4bbf-8f1a-20f0b54fde6b" />
    </td>
  </tr>
</table>

<p>
  - We should see a confirmation that SLA PLan was updated successfully. Next, click "Help Topic". Use the dropdown to select "Report a Problem / Business Critical Outage". Comment the reason and click "Update".</p>
<p>
  - Making these changes will help our team process the ticket accordingly and effectively.
</p>
<br/>

<table>
  <tr>
    <td>
      <img width="997" alt="Screenshot 2025-06-17 at 4 42 23 PM" src="https://github.com/user-attachments/assets/2be09115-8eda-4741-a64a-ed76c8329e9f" />
    </td>
    <td>
      <img width="988" alt="Screenshot 2025-06-17 at 4 44 48 PM" src="https://github.com/user-attachments/assets/3c38bc23-e206-472d-9796-1dd2ca7b7622" />
    </td>
  </tr>
</table>

<p>
  - You should see a confirmation saying Help Topic updated successfully. Now, click "Unassigned". Assign the ticket to Online Banking. Comment and click "Assign".
</p>

<p>
  <img width="1001" alt="Screenshot 2025-06-17 at 4 53 16 PM" src="https://github.com/user-attachments/assets/4e854207-b36c-4be3-bcee-2e34b134d9b4" />
</p>

<p>
  - You should see a confirmation saying that the ticket was assigned to Online Banking successfully. Review the changes we made and scroll down. 
</p>
<br/>

<p>
<img width="998" alt="Screenshot 2025-06-17 at 5 01 07 PM" src="https://github.com/user-attachments/assets/f18a4822-784a-4de1-b3e7-25d1a99a155d" />
</p>

<p>
  - osTicket keeps a track of all the changes in the Ticket Thread. You should see the reasons you commented here.
</p> 
<p>
  - This helps us keep track of who did what with the ticket and keeps everyone updated. 
</p>
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





