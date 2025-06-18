<p align="center">
<img width="972" alt="Screenshot 2025-06-17 at 6 17 20 PM" src="https://github.com/user-attachments/assets/a01d23ba-2073-4ea3-ab0a-71597fd1bd8e" />
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

<p>
  - We have discovered an issuenwithin osTicket about 30 mintues ago! A few clients called and asked for an update concerning some Help Desk Tickets they submitted. After many attempts, our Lead Agent was unable to locate the tickets. Afterwards, the Lead Agent submitted a "Test" ticket via the Support Center portal and was unable to locate the "Test" ticket as well! Tickets are being created successfully but our Agents are unable to see them. The Help Desk Manager has exclated the issue to our Admin Team. Lets go solve this issue!    
</p>
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
<p>
  - Upon further investigation, we discovered that a recent update caused a bug with a preset Department within osTicket. The bug is causing the tickets to be sent to the Maintenance Department regardless of the configurations. We will delete this department to get operations back to normal while osTicket works on a patch! 
</p>
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
<p>
  - The Maintenance Department has successfully been deleted! We had our Agents log out and log back in to osTicket. They are reporting that the tickets are now visible and being routed to the correct Departments! Awesome! Now, we can get to creating and working tickets!
</p>
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
<p>
  - Click the blue button that says "Open a New Ticket". Create a ticket as Karen.
</p>
<p>
  - Enter the folllowing - Email Address: karen@lognpacific.com | Full Name: Karen | Help Topic: Report a Problem.
</p>
<p>
  - Fill out Issue Summary. In the smaller text field for the heading type in, "Entire mobile/online banking system is down". In the larger text field for the summary type in "My employees are reporting that users are not longer able to access the online banking portal. The ones who can occassionally access it, cannot log in.". Scroll down and click "Create Ticket".
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
     <img width="1002" alt="Screenshot 2025-06-17 at 5 33 19 PM" src="https://github.com/user-attachments/assets/5d7a8373-4a9f-406d-addb-0289cc628450" />
    </td>
    <td>
      <img width="998" alt="Screenshot 2025-06-17 at 5 34 34 PM" src="https://github.com/user-attachments/assets/5a7b9f50-cb15-44ff-951c-2e7489b893a3" />
    </td>
  </tr>
</table>

<p>
  - Log out of John Dow and log in to the portal as Jane Doe. Username: jane_doe | Password: Password1
</p>
<p>
  - We are going to work and resolve this ticket as Jane Doe moving forward. 
</p>
<p>
  - John assigned the ticket to Online Banking.Jane is on that team. Open the ticket by clicking on the subject.
</p>
<br/>

<table>
  <tr>
    <td>
     <img width="998" alt="Screenshot 2025-06-17 at 5 36 23 PM" src="https://github.com/user-attachments/assets/3c4738f5-8f91-4db5-abe1-9dde22715325" />
    </td>
    <td>
      <img width="1000" alt="Screenshot 2025-06-17 at 5 37 13 PM" src="https://github.com/user-attachments/assets/68759718-bad7-4d4b-8ebc-f5e6508a369d" />
    </td>
  </tr>
</table>

<p>
  - Assign the ticket to Jane to reflect which Agent will be working the ticket. Pretend that Online Banking has more then one Agent.</p> 
<p>
  - Click "Online Banking" next to "Assigned To". When the window pops up, select "Jane Doe" for "Assignee", write a comment in the text field and then click "Assign".
</p>
<p>
  - Having the ticket assigned to a specific Agent will help with tracking. 
</p>
<br/>

<p>
  <img width="1000" alt="Screenshot 2025-06-17 at 5 45 47 PM" src="https://github.com/user-attachments/assets/0a4df39d-6b51-4939-82d9-cc6e8cbffcea" />
</p>

<p>
  - We should see a confirmation saying that the ticket was assigned to Jane Doe successfully. 
</p>
<p>
  - Also look at the "Assigned To" section of the ticket.
</p>
<p>
  - It should show that the ticket is assigned to Jane Doe of the Online Banking team.
</p>
<br/>

<p>
  <img width="994" alt="Screenshot 2025-06-17 at 5 48 38 PM" src="https://github.com/user-attachments/assets/ff3fa143-a1a1-4535-9416-e9e2d7be76b4" />
</p>
<table>
  <tr>
    <td>
      <img width="996" alt="Screenshot 2025-06-17 at 5 59 00 PM" src="https://github.com/user-attachments/assets/fe8ca808-baa4-4b55-a7f4-342c00f94017" />
    </td>
    <td>
      <img width="999" alt="Screenshot 2025-06-17 at 6 02 02 PM" src="https://github.com/user-attachments/assets/d86972bb-bd0f-4e1a-a93a-b59c04d35764" />
    </td>
  </tr>
</table>

<p>
  - Next, we'll send an update to Karen about the ticket she submitted. Scroll down and be on the Post Reply tab. Click Post Reply if you are not already on it.
</p>
<p>
  - Type in a response to her saying that you suspect the problem have to do with the recent updates. Click "Post Reply".
</p>
<p>
  - Finally, let's notify Karen that we determined a cause for the issue, it has been addressed, and online banking is working again. Again, type in a response and then click "Post Reply". 
</p>

<br/>

<table>
  <tr>
    <td>
      <img width="997" alt="Screenshot 2025-06-17 at 6 06 07 PM" src="https://github.com/user-attachments/assets/bf0fa993-47ad-4174-a27d-bdf2d4ae0760" />
    </td>
    <td>
      <img width="995" alt="Screenshot 2025-06-17 at 6 08 02 PM" src="https://github.com/user-attachments/assets/deb9df1b-7347-4dc5-84af-d39735155c02" />
    </td>
  </tr>
</table>

<p>
  - Scroll up and observe all of Jane's respones in the Ticket Thread.
</p>
<p>
  - Now that the issue is fixed and the end user has been updated, lets close the ticket. 
</p>
<p>
  - Click Status and select Resolved.
</p>
<br/>

<table>
  <tr>
    <td>
      <img width="652" alt="Screenshot 2025-06-17 at 6 08 44 PM" src="https://github.com/user-attachments/assets/62a88605-6e5c-406d-89f3-f8ed3fd99e8c" />
    </td>
    <td>
      <img width="1000" alt="Screenshot 2025-06-17 at 6 09 35 PM" src="https://github.com/user-attachments/assets/727c322d-a164-4729-a2ce-24f66ce4ab78" />

    </td>
  </tr>
</table>

<p>
  - When the window pops up, change the Status to Resolved. You can comment on the change and then click "Close".
</p>
<p>
  - The ticket has been resolved! You should see a confirmation saying so. 
</p> 
<p>
  - Congrats! You have successfully created, worked, and resolved a Help Desk ticket within osTicket! 
</p>
<br/>

<h2>Conclusion</h2>

<p>This concludes our project. We have successfully navigated through the life cycle of a Help Desk ticket within osTicket. This project successfully demonstrated the end-to-end lifecycle of a Help Desk ticket using osTicket, from creation to resolution. Through this hands-on experience, we explored key aspects of ticketing systems, including ticket submission & categorization, workflow management (assignment, prioritization, SLA compliance), and resolution & closure processes
</p>
<p>
I recommend taking the time to play around in osTicket by creating and working different tickets. Use your imagination and have fun being your own Help Desk! Don't forget to Stop (turn off) the VMs in Azure. As always, Thank You for your time and viewing this Project. We'll see you on the next one!
</p>
<br/>





