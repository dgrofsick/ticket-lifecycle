<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10 22H2

<h2>Ticket Lifecycle Stages</h2>

- Ticket Creation
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>

<h3>Ticket Creation</h3>

<br />

- Continuing where we last left off, use http://localhost/osTicket/ to submit a ticket as <b>Karen Doe</b>
  -  The following mock situation we'll be addressing will simulate Karen being locked out of her account and needing a new password.

![image](https://github.com/dgrofsick/ticket-lifecycle/assets/148154704/e3312b25-8796-469e-8dc3-d5b7274b2c57)

<br />

- Enter Karen's information in the necessary boxes and within the <b>Issue Summary</b> text box, enter the description of the problem.  Once completed, select <b>Create Ticket</b>

![image](https://github.com/dgrofsick/ticket-lifecycle/assets/148154704/04be3f79-9f7e-4ff0-b651-84f47eeffbf3)

![image](https://github.com/dgrofsick/ticket-lifecycle/assets/148154704/f4f5294d-7dd7-4182-8ff8-b989664ddd4a)

<br />

- Next, we will log back into osTicket under our original admin profile (i.e. dustin_admin) and create a log in password for jane_admin.
  -  Ensure that the <b>Agent Panel</b> link is visible in the top right corner (this tells us that we are actually under the Admin status)
  -  Click the <b>Agents</b> tab
  -  Select <b>Set Password</b> 

- Set jane_admin's password to Password1 (or whatever you choose) and leave 'Require password change at next login' unchecked. 

![image](https://github.com/dgrofsick/ticket-lifecycle/assets/148154704/bad66ece-cb54-4aa0-9917-bdefdbf6d3ae)

![image](https://github.com/dgrofsick/ticket-lifecycle/assets/148154704/547fd7dc-bb1b-424a-846f-3675ee90d1c6)

<br />

<h3>Ticket Assignment and Communication</h3>

- Logout of osTicket and log back in as Jane using the below email address created for her profile and <b>Password1</b> as the password.  Upon successfully logging in, Karen Doe's ticket should be visible and ready for assistance.

![image](https://github.com/dgrofsick/ticket-lifecycle/assets/148154704/d6455a10-eab7-4cef-95f4-b2b84bb007a3)

![image](https://github.com/dgrofsick/ticket-lifecycle/assets/148154704/d6f1597d-31c3-493c-a020-22d4ae1e3b7c)

<br />

<h3>Working the Issue</h3>

- Use Response drop down menu to select your reply method.  Since we will be using a custom message, select <b>Original Message</b>.  Beneath the Response menu you will find your text box to enter a professional response addressing the matter at hand.  Lastly, <b>Ticket Status</b> can be found at the bottom of your reply menu.  

![image](https://github.com/dgrofsick/ticket-lifecycle/assets/148154704/25ffbc44-f8fb-4577-b73a-7d08ca9d5d68)
 
 <br />

<h3>Ticket Resolution</h3>

- Until the matter has been fully resolved, the ticket status should remain as <b>Open (current)</b>.  Otherwise select the option that best suits the circumstances.   Click <b>Post Reply</b> when a proper response has been entered.

NOTE:  When using the above methods to create and submit tickets, be sure to vary the severity of the problems.  By doing this and addressing the created tickets as Help Desk employees, you allow yourself to make judgement calls and categorize the tickets in accordance to their severity.  Select the appropriate SLA status for the ticket created as well as which department/team the ticket is best suited for <b>i.e. a Sev-C issue for the Support Department may be best used for an issue submitted by someone who requested new equipment or a new password while a Sev-A issue such as customers not being able to check out and pay for their orders due to a system error is best suited for the System Administration Team.</b>  These options can be found in the same menu where you would post your reply to the customer's submitted ticket.  When or if these tickets are categorized as such, they will be forwarded to the assigned department and await a proper response.

![image](https://github.com/dgrofsick/ticket-lifecycle/assets/148154704/6dea56f8-70e0-490a-86ab-93c59279e9fa)

<h2>Resource Cleanup</h2>

- Close your Remote Desktop connection
- Delete the Resource Group(s) created at the beginning of this turtorial, including the Network Watcher
- Verify Resource Group Deletion
