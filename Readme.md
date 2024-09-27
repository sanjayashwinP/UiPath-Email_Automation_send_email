## Exercise_10-Email Automation-send_email

## Aim:

To automate the process of sending an email using UiPath Studio.

## Equipment Required:

UiPath Studio installed on your computer.<br>
Email Account (e.g., Gmail, Outlook) with necessary credentials.<br>
SMTP, IMAP, or Outlook Integration (depends on your email provider).<br>
Computer with:<br>
Minimum 4 GB RAM.<br>
Minimum 2.0 GHz CPU.<br>
Windows operating system.

## Procedure:

### Create a New Process in UiPath Studio:

Open UiPath Studio and create a new project by selecting Process under the New Project tab.<br>
Name the process (e.g., Email Automation) and click Create.

### Add Email Activities Package:

In the Manage Packages panel (top ribbon), click on Manage Packages.<br>
Search for UiPath.Mail.Activities and install the package. This allows you to use email-related activities like sending and receiving emails.

### Choose an Email Activity: Depending on the type of email provider you're using, select the appropriate activity:

SMTP (Simple Mail Transfer Protocol): For sending emails.

### Send Email Using SMTP (For Gmail/Other Providers):

#### Add SMTP Mail Message Activity:

In the Activities panel, search for the Send SMTP Mail Message activity and drag it into your workflow.

#### Configure SMTP Server:

In the Properties panel for the activity, configure the SMTP server settings:<br>
Port: For Gmail, use 587.<br>
Server: For Gmail, use smtp.gmail.com.<br>
SecureConnection: Use StartTls for secure connection.<br>

#### Configure the Email Parameters:

To: Enter the recipient's email address (e.g., recipient@example.com).<br>
From: Enter the sender's email address (your Gmail address, e.g., youraddress@gmail.com).<br>
Subject: Enter the subject of the email (e.g., Test Email from UiPath).<br>
Body: Enter the email body content (e.g., Hello, this is an automated email from UiPath.).<br>
Attachments (Optional): If you want to attach a file, provide the file path in the Attachments property.

#### Set Authentication:

You need to authenticate the email sending by providing your username (Gmail address) and password in the Properties panel under the Username and Password sections.

### Save and Run the Workflow:

Press CTRL+S to save the workflow.<br>
Click the Run button in UiPath Studio to execute the automation.<br>
The email will be sent automatically using either SMTP or Outlook, depending on the chosen activity.<br>

## UiPath WorkFlow:

![alt text](<img/Screenshot 2024-09-27 192351.png>)
![alt text](<img/Screenshot 2024-09-27 192410.png>)
![alt text](<img/Screenshot 2024-09-27 205823.png>)
![alt text](<img/Screenshot 2024-09-27 205849.png>)
![alt text](<img/Screenshot 2024-09-27 205915.png>)
![alt text](<img/Screenshot 2024-09-27 205933.png>)
![alt text](<img/Screenshot 2024-09-27 205733.png>)

## Result:

The email is successfully sent to the recipient using the configured email account and the appropriate activity (SMTP).
