# How to set up an IMAP e-mail account in Thunderbird?

This article explains the difference between the POP and IMAP protocols, why you should use IMAP (what are its benefits), and how to configure this protocol in the Thunderbird mail program.

## 1.	What is POP?

POP ([Post Office Protocol](https://en.wikipedia.org/wiki/Post_Office_Protocol)) is a protocol for accessing mail messages. However, the logic behind POP is entirely different from IMAP. When using POP, you contact your e-mail provider, log in to the e-mail server and download new messages.

However, after you have downloaded your messages to your computer, the e-mails are deleted from the e-mail server (so it is as if you moved them to your local computer).

After downloading the e-mails, the downloaded e-mails are only available on the computer where they were downloaded. If you try to access your e-mails from another device, the previously downloaded messages will not be available.

Obviously, in today's fast-paced world, when we want to access our e-mails once from one laptop, then from another computer, and then from our mobile phone at home (and possibly respond to them or work from home), this method is already very outdated, not a solution.

This method had its heyday at the beginning of the spread of the Internet when many people could only access their e-mails and communicate with others from a home computer (a single computer).

In the case of smaller companies, on closed internal networks, and communication from the same machine, this protocol can still be a solution, but it has extreme limitations.

## 2.	What is IMAP?

IMAP stands for the [Internet Message Access Protocol](https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol). It is a standard Internet protocol e-mail clients use to retrieve e-mail messages from a mail server over a TCP/IP connection. This protocol allows e-mail clients (such as Thunderbird) to access messages stored on the mail server. IMAP is the most modern and widely-used e-mail protocol.

## 3.	What is the advantage of using IMAP?

The advantage of IMAP is that you can use it to access your e-mails from any device because by using IMAP, you do not download or store them on your computer but read them on the e-mail provider's server. 

What is the significance of this in terms of cybersecurity? In most cases (unless you specifically want it), you do not download anything; thus, harmful codes do not end up on your machine either. It is clear that the service provider protects its e-mail server and does everything to ensure that no harmful codes can occur there. However, this also protects you since you read our e-mails from or on a reliable source (on the service provider's e-mail server).

## 4.	How to set up IMAP in Thunderbird?

### 4.1.	 Check that your e-mail provider supports IMAP

While most e-mail providers support IMAP, some still do not: so make sure your e-mail provider supports IMAP first.

### 4.2.	 Disable your POP account

For smoother e-mail management and to avoid duplication of checking new messages, the POP protocol must be turned off before the IMAP is turned on.  To achieve this, go to your account settings by opening the Tools > Account Settings menu, and select ’Server settings’ on the left panel. 

![](http://hdoc.csirt-tooling.org/uploads/upload_5b30c42b585cd98b2a0e80562d72f572.png)

Then, un-check both ’Check for new messages at startup’ and ’Check for new messages every XX minutes’.

![](http://hdoc.csirt-tooling.org/uploads/upload_f1cabd733013a8805e7f8fd737a17ce0.png)

### 4.3.	 Create your IMAP account

Go to ’File – New – Existing Mail Account…’

![](http://hdoc.csirt-tooling.org/uploads/upload_3960cefb6602804ba9dca8b059c198eb.png)

The ’Account Setup’ window opens. Provide your full name, e-mail address and password for your e-mail provider and click ’Continue’. 

![](http://hdoc.csirt-tooling.org/uploads/upload_7b5c2f271664eeb73e29d05d6bff8928.png)

With the help of Thunderbird’s Automatic Account Configuration, Thunderbird determines connection details (such as ports, server names, security protocols, etc.) by looking up your e-mail provider in a database. Once the probing of the configuration is successful, Thunderbird will show you the below message:

![](http://hdoc.csirt-tooling.org/uploads/upload_d3e0db687ca8feaf28b5c0d756079a2f.png)

## 5.	How can I check whether I have a POP or IMAP folder?

To check whether your account uses IMAP or POP, go to the Server Settings page in the Account Settings:

![](http://hdoc.csirt-tooling.org/uploads/upload_390e2ef40ba27e71b18764f35a350cb1.png)

## 6.	Useful links for further information

* The difference between IMAP and POP3
https://support.mozilla.org/en-US/kb/difference-between-imap-and-pop3#:~:text=When%20adding%20an%20email%20account,are%20kept%20on%20the%20server.
* Switch from POP to IMAP account
https://support.mozilla.org/en-US/kb/switch-pop-imap-account
* IMAP Synchronization
https://support.mozilla.org/en-US/kb/imap-synchronization#:~:text=IMAP%20stands%20for%20the%20Internet,protocol%20for%20accessing%20mail%20messages.
* Set up an IMAP e-mail account in ThunderBird
https://www.fastcomet.com/tutorials/mail/thunderbird-imap-configuration
* Automatic Account Configuration
https://support.mozilla.org/en-US/kb/automatic-account-configuration
* Thunderbird: How to Configure an IMAP E-mail Account With SSL
https://www.youtube.com/watch?v=RDQSr5dDDtM
* How To Set Up Thunderbird (IMAP & SMTP over SSL)
https://www.youtube.com/watch?v=2K_1KirVmkM


# How do I set up IMAP in Thunderbird?
**(short version)**

1. Check that your e-mail provider supports IMAP
1. Disable your POP account
1. Create your IMAP account
1. Open File > New > Existing account menu
1. Set up your account with the help of the assistant (Automatic Account Configuration)
1. Your new IMAP account will be created and appear at the bottom of your existing mail accounts
