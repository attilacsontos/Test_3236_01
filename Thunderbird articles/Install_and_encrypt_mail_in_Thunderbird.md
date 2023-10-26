# How to install and configure email encryption in Thunderbird?

This step-by-step guide shows how to install and set up email encryption in Thunderbird on a Windows operating system. If you are looking for an open-source email client that is feature-rich and provides easy-to-use end-to-end encryption, then Thunderbird can be an excellent choice.

**Why encrypt emails?**

Sending emails without encryption is like sending postcards to your loved ones: like it or not, anyone and any system that processes emails can intercept and then read its content. Encrypting your emails is like putting your message in an envelope that only the recipient of the email can open.

For further reading on encryption, cryptography, types of cryptographic algorithms (like symmetric- and asymmetric encryption), digital signatures and related topics, please read the article [Encryption: the unnoticed law enforcement force in cyberspace](https://www.cybersecurity.lu/tool/encryption-the-unnoticed-law-enforcement-force-in-cyberspace/).

## 1. What is Thunderbird?

Thunderbird is a free and open-source email, chat, and calendar client that is easy to set up and customize. One of the main principles of Thunderbird is the use and promotion of open standards. As an open-source project, anyone can contribute and share their ideas, designs, code, and time to help other users.

## 2. How to install Thunderbird?

Navigate to the website of Thunderbird (https://www.thunderbird.net/) and click on the Free download button.
 
 ![](http://hdoc.csirt-tooling.org/uploads/upload_216b13edfac58fb5fb42651a886b700e.png)

The process starts, and the below popup shows the progress of the process:
![](http://hdoc.csirt-tooling.org/uploads/upload_c8ab108f1cece441c7c8743ff0ae6a5b.png)

In your Downloads folder, you should be able to see the package:

![](http://hdoc.csirt-tooling.org/uploads/upload_dce15c7da184972e8ff2363b6ca2efff.png)

Double-click on it so the set-up wizard appears:

![](http://hdoc.csirt-tooling.org/uploads/upload_582c0a889ddbba5527744db47bb80083.png)

Click 'Next >' and choose a set-up type (Standard or Custom):

![](http://hdoc.csirt-tooling.org/uploads/upload_0d3bc808859557bd157eef2086d8f069.png)

After you have made your decision and clicked on the 'Next >' button, the Summary window appears. Here, you can see the location where Thunderbird is installed on your hard drive, and you can decide whether you want Thunderbird to become your default mail application. Click 'Upgrade' to continue:

![](http://hdoc.csirt-tooling.org/uploads/upload_42051d756e73ab771888b97627b79f9a.png)

The window that appears as the last step of the installation informs you that Thunderbird has been installed on your computer, and you can start the application by clicking on the 'Finish' button: 

![](http://hdoc.csirt-tooling.org/uploads/upload_526fd31058dd2c04539e80e88e0e60b3.png)

As the next step, the 'Set Up Your Existing Email Address' window appears. Please fill out the fields and choose a strong password. If you already have an email address (for example, in the Zimbra email client), use the same password and login (email address), so Thunderbird can check and set up your account. Click on 'Continue':

![](http://hdoc.csirt-tooling.org/uploads/upload_3d634959510e83c0dc1e65783a0c38a9.png)

Thunderbird probes the email server and auto-populates some fields, as can be seen in the below screenshot:

![](http://hdoc.csirt-tooling.org/uploads/upload_53c2edfb23d3c5d967be3874e19a5406.png)


Please use ’mail.mbox.lu’ as the Hostname. Click on 'Re-test' (if necessary), so Thunderbird can check the settings on the given mail server (mail.mbox.lu). The checkmark and the message on a green background show that the test was successful, Thunderbird found the ports of the incoming and outgoing servers, and the communication is settled. Click on 'Done'.

![](http://hdoc.csirt-tooling.org/uploads/upload_be28ed8b7bcefe01bd9fa245d07edf94.png)

Please note that the configuration may change. Please contact the Helpdesk at sysadmin@lhc.lu for further information if your settings do not work.

The new window informs you that your account has been successfully created. Besides this vital information, you can modify your account settings, add a signature to your emails, and create end-to-end encryption.

![](http://hdoc.csirt-tooling.org/uploads/upload_302d1971c594c8ba1aa0b619e1eb307a.png)

Please click on 'Finish', so your Thunderbird instance opens with the below popup:

![](http://hdoc.csirt-tooling.org/uploads/upload_62d01b8ea7e84ab7cd14a4bd74dfcae4.png)

As the last step of the installation, you can set Thunderbird as the default client for your email, newsgroup, feeds and calendar. You can make these settings default (by checking or unchecking the relevant checkbox and clicking on ' Set as default'). Alternatively, you can choose 'Skip integration' if you do not want these options.

## 3. How to enable end-to-end encryption in Thunderbird?

To use the OpenPGP feature (end-to-end encryption or E2EE), you must set up a public-private key pair for your email address in Thunderbird.

Once your account has been created, Thunderbird offers you to enable end-to-end encryption. Still, you can make this step anytime you want. For security reasons, it is advised to do it as soon as possible. Please navigate to the lower left-hand corner of the screen and click on the gear icon (Settings).

![](http://hdoc.csirt-tooling.org/uploads/upload_c170e16a9fc25d788609a48e1afac1d8.png)

The Settings window opens. Choose 'Account Settings' in the lower section of the left panel:

![](http://hdoc.csirt-tooling.org/uploads/upload_888ddfb9a9dfdb1542df8668041f33ed.png)


The Account Settings window opens. Click on the 'End-To-End Encryption' tab from the drop-down menu on the left panel. To send encrypted emails, you need to configure either OpenPGP or S/MIME. As seen from the screenshot below, there is no OpenPGP key set up yet. 

Click on 'Add Key' to add a personal OpenPGP key for your email:

![](http://hdoc.csirt-tooling.org/uploads/upload_ae2db5d708046700883fffa9f8ba4be4.png)

If you already have a personal key for your email address, you should import it. 

If you do not import your existing key:

"..you will not have access to your Archives of encrypted emails, nor be able to read incoming encrypted emails from people who are still using your existing key!"

If you do not have a personal key associated with your email address, please create a new OpenPGP Key by choosing the first radio button:

![](http://hdoc.csirt-tooling.org/uploads/upload_7f971235bb8e0ffd0f4e4d76a0dc8abe.png)

The 'Generate OpenPGP Key' window opens. PGP keys are always linked to an email address, so first, you need to choose your identity from the drop-down menu. Next, you can set up the expiry date of your key.

![](http://hdoc.csirt-tooling.org/uploads/upload_474bb0bb2c7de2bc494ca037d805c07d.png)

You may leave the 'Advanced settings' untouched as they often are the best settings security-wise. Click on the 'Generate key' button. The following window opens:

![](http://hdoc.csirt-tooling.org/uploads/upload_517ca5bb98cc7bbd906b06e2495ecdae.png)

Once you click on the 'Generate key' button, a public and a private key will be generated. While the key is generating, moving your mouse randomly or doing Internet research is essential. The more things you do, the more random your key will be.

![](http://hdoc.csirt-tooling.org/uploads/upload_74cba852abbdcd5897960210cdb2517b.png)

Send your public key to the people you want to exchange encrypted emails. You can verify other users' keys with your fingerprint. Open the blue area by clicking the down-pointing arrow to reveal your Fingerprint. You may also check your Key Properties. 

![](http://hdoc.csirt-tooling.org/uploads/upload_3c3580eccb14aee9b8e47fdb5803f601.png)

Now, the end-to-end encryption is set up. But there is one essential step that remained. And this is what is discussed in the next chapter.

## 4. How can I send encrypted emails?

Your encryption keys have been created, and now you should be able to use them. Go to your inbox and click on the button 'Write' to create a new email. When you create a new email, a new tab called 'OpenPGP' appears on the screen. Please note that the sub-menus 'Encrypt' and' Digitally sign' are still inactive.

![](http://hdoc.csirt-tooling.org/uploads/upload_53689b4e474870211676be0c40288801.png)

You can encrypt your mail in two ways:
* You can use the 'Encrypt' tab next to 'OpenPGP'
* You can choose the sub-menu 'Encrypt' of the drop-down 'OpenPGP'

![](http://hdoc.csirt-tooling.org/uploads/upload_b6988ee7737391f2ab28117ba73a1132.png)

You can also digitally sign your emails by using the sub-menu 'Digitally Sign' of the drop-down 'OpenPGP'.

**CAUTION!**

Your messages in the sent folder will be encrypted if you send encrypted messages. If you lose your private key, you will not be able to read archived messages. These messages cannot be restored!

Likewise, if you lose your private key, others can still send you encrypted emails, and you will not be able to read them.

Also, note that search functions generally do not work for the body of encrypted messages. It is essential to know that you can only send encrypted emails to those who are similarly able to receive and send encrypted emails. If you want to send an encrypted message to an email address whose public key is not saved on our computer, you receive the following error message:

![](http://hdoc.csirt-tooling.org/uploads/upload_27adce8bc1e8c160956d318bec3d4a20.png)

To solve the problem, you can decide not to encrypt your message. Alternatively, you may try to resolve the issue by clicking the ’Resolve…’ button. If you click on the ’Resolve…’ button, the OpenPGP Assistant window opens and informs you that you do not have the key to the recipient’s email address:

![](http://hdoc.csirt-tooling.org/uploads/upload_4cbf744ccebb7ecf7772afdbe3560579.png)

You can try to discover your recipient’s public key online or import it if your recipient has sent it to you already. If you click the ’Discover Public Keys Online…’ button and Thunderbird cannot find your recipient’s public key online, you will be directed back to the OpenPGP Assistant window. 

In this case, you should click on ’Disable encryption’ to be able to send an unencrypted email to your recipient. You may ask your recipient in an unencrypted email to send you his/her public key, so after importing it, you can send encrypted emails to each other.

## 5. How can you send your public key to other people?

After you have created your private key, you must allow others to obtain your public key. Be careful, and never share your private key with anyone. However, the public key can be widely shared, so people can send you encrypted emails and verify your digital signatures. This is how it works:

1. Start writing a new mail.
1. Navigate to and click on the 'Attach' drop-down in the top right-hand corner
1. Chose the sub-menu 'My OpenPGP Public Key'

![](http://hdoc.csirt-tooling.org/uploads/upload_dbe0fc3d849e2ce506de17eefa8de756.png)

Your recipient will see an attachment in the email with a file name starting with "OpenPGP". If your recipients are using Thunderbird, they can right-click on the message to open a menu of options and select "Import OpenPGP Key" from that menu.

## 6. How to export your OpenPGP public key?

Go to ’Tools’ in the menu bar and choose the sub-menu ’OpenPGP Key Manager’:

![](http://hdoc.csirt-tooling.org/uploads/upload_55948c01a390451b402174ea7fe8f198.png)

Select the OpenPGP public key you want to export and choose the ’Export Public Key(s) To File’ drop-down menu.

![](http://hdoc.csirt-tooling.org/uploads/upload_fb20df8fe1c9d6293706a652161b7ddd.png)

Alternatively, open account settings and select the end-to-end encryption panel to download your OpenPGP keypair's public key directly. Click on the drop-down menu ’More’ and choose the sub-menu ’Export Public Key(s) To File’.

![](http://hdoc.csirt-tooling.org/uploads/upload_3217d614701fdb6e2be801073479ada6.png)

## 7. How to exchange public keys?

Everyone to whom you send encrypted messages must have their own public key. Your recipients also need yours so they can send encrypted messages back to you. There are a few ways to get someone's public key. They may send it to you without notice, or you may ask them to do so. You can even try to find your recipients’ public keys online.

### 7.1. Find a public key online

Go to a key server, for example, https://keys.openpgp.org/ and search by email address, Key ID or Fingerprint:

![](http://hdoc.csirt-tooling.org/uploads/upload_1a5c2e86c2812345d16af915a3841ede.png)

In case there is a record for the searched item on the server, you can see the owner of the public key and see the owner’s fingerprint:

![](http://hdoc.csirt-tooling.org/uploads/upload_262123adb2fd2ab10426eab2ed5d3e6f.png)

You can download the owner’s public key by clicking on the link:

![](http://hdoc.csirt-tooling.org/uploads/upload_0cdadad8500cae42655f3d748a94dcec.png)

### 7.2. You receive someone's public key

Thunderbird includes an 'OpenPGP' button to the right of the email header when you receive an email with an attached public key. The screenshot below shows a message signed with the sender’s public key. 

Also, it was digitally signed, so the certificate icon indicates it. Since this is the first time you have received the below message from your sender, Thunderbird does not know whether the signature is valid (this is why the application shows a question mark next to the icon).

![](http://hdoc.csirt-tooling.org/uploads/upload_42580689a87e7108efb157a04235b626.png)

If you click on the OpenPGP button, the below window pops up:

![](http://hdoc.csirt-tooling.org/uploads/upload_7d2ccc6feadd856e4aebdf5f0d14abd8.png)

The message says that you still do not have this public key, so you need to import it. Besides that, you need to verify that the digital signature is valid.

Click on the ’Discover’ button. The popup informs you that the email attachment contains the sender's public key, and the message shows the sender’s fingerprint and email aliases. By looking at the email addresses, you should be able to identify the sender to import the public key.

In the lower part of the window, you can verify (accept) the signature of the sender.

![](http://hdoc.csirt-tooling.org/uploads/upload_f44e91ca311690b91fbb83996eb19f4f.png)

Let’s choose the radio button ’Accepted (unverified)’ and click on the button ’Import’ in the lower right-hand corner. The following window informs you that the public key was imported successfully:

![](http://hdoc.csirt-tooling.org/uploads/upload_96234bd4f48e6139ab072143fc31a7d2.png)

By clicking on the link at the bottom of the window, you can view the details and manage the key acceptance (do not forget that you just imported the public key successfully, you have not verified it yet).

At the top, you see the key properties (owner, type, Key ID, Fingerprint, Created, Expiry); in the lower section, you have four tabs to choose from. The first tab is the ’Your Acceptance’ tab:

Here, you can decide whether you want to reject the key, or you accept it but have not verified yet, or accept and verify the key that it belongs to the sender:

![](http://hdoc.csirt-tooling.org/uploads/upload_1c9816beb7805737ca537271a8698a09.png)

How can I verify the public key? See chapter ’7.1. Find a public key online’.

Since I know who the sender is, let me choose the option to verify that the public key and the digital signature are valid:

![](http://hdoc.csirt-tooling.org/uploads/upload_ea28cadff1051959f1687135341131fd.png)

Since I have verified the sender’s public key and digital signature, the icons in the top right-hand corner of the email have changed. A green checkmark appears on the key and certificate icon.

![](http://hdoc.csirt-tooling.org/uploads/upload_31757cfe375084d258390fa2ba346a23.png)

If you click on the icon, the below window opens and informs you that the digital signature is valid and the message is encrypted.

![](http://hdoc.csirt-tooling.org/uploads/upload_8fa8fe0313ff8a5ed7f3c544b15ca895.png)

From now on, you can continue sending and receiving encrypted messages with your email partner.

## 8. How can you upload your public key?

Go to a key server (for example, https://keys.openpgp.org/ ) and choose the link ’upload’.

![](http://hdoc.csirt-tooling.org/uploads/upload_ae1ffae76c5856cde56a481e31878bdf.png)

As the next step, click on ’Choose File’ and click on the ’Upload’ button on the right.

![](http://hdoc.csirt-tooling.org/uploads/upload_9fb0c1d7fc398ef3534fc2dde80bc17f.png)

If the upload process is successful, you receive a similar message as the one below:

![](http://hdoc.csirt-tooling.org/uploads/upload_cc9fac9b459042734c6573e514dea895.png)

You may send a verification email to yourself by clicking on the ’Send verification Email’. Shortly, you will receive a similar email as follows:

![](http://hdoc.csirt-tooling.org/uploads/upload_1a22b34b8ca488883c5a05a8a4cd6dbf.png)

## 9. How can you exchange encrypted emails with others?

### 9.1. In theory

Thunderbird's OpenPGP integration allows you to encrypt your email messages. After that, only those whom you want to read your message can do so. This integration also allows the message to be digitally signed, so the recipient can be sure that the message has not been altered in transit.

OpenPGP uses the principle of a pair of public and private (or 'secret') encryption keys. To use OpenPGP, you must have a public and a private key pair. Public keys should be shared with anyone you want to send encrypted messages to, while private keys are never shared with anyone else. Private keys can also decrypt messages encoded with the corresponding public key.

The sender's email client generates a random key to encrypt the message. The random key is then encrypted with the recipient's public key, and the encrypted message and key are sent to the recipient. The recipient's email program uses the recipient's private key to decrypt the random key. The random key can then be used to decrypt the encrypted message.

For each recipient, a random key is encrypted with that person's public key. All encrypted keys are then sent with the message. Each recipient can decrypt a copy of the random key encrypted with their public key and then use the random key to decode the message.

### 9.2. What is needed to send an encrypted message?

You must have your private (secret) and public keys set up. Each recipient of your encrypted message must have an accepted public key.

You should verify that the public keys of your correspondence partners really belong to them. Accepting someone's public key without verifying exposes your communication to Man In The Middle (MITM) attacks.

If you do not have a public key for a particular recipient, the message will be blocked from being sent, and Thunderbird will warn you. You can choose not to send the message at all, disable encryption and send the message unprotected, or send the message only to a subset of recipients who have public keys.

### 9.3. What does key acceptance mean?

Anyone can create a private key on behalf of anyone using any email address. It means that every time you receive an encrypted email from someone with their public key, by accepting it without validating the keys, you risk the key being fake and open yourself up to being scammed.

In connection with encrypted correspondence, it happens less often that we receive emails from complete strangers. If this does happen, an extra filter often enters, meaning we authenticate the sender of the email through a telephone inquiry or another communication channel.

Maybe you talked to someone a few minutes ago and agreed they would send you an email. The point is to ensure that the email that arrives in your mailbox is authentic.

For many, this may seem like an unnecessary hassle or extra pointless work. However, the essence of encrypted email communication would be to exchange information with reliable partners.

For further reading on end-to-end encryption in Thunderbird, please read the article [Introduction to End-to-end encryption in Thunderbird](https://support.mozilla.org/en-US/kb/introduction-to-e2e-encryption).

Once you have set up your private key, you can control whether encryption or digital signatures are used for each message you send. After you have created your private key, allow others to obtain your public key so that you can conduct secret email communications. 

## 10.	Limitations of end-to-end encryption

End-to-end encryption (E2EE) requires caution from both the sender and the recipient. A single mistake by any involved party can be enough to breach E2EE security. 

Also, another limitation of end-to-end encryption is that email metadata cannot be protected. For example, the name and address of the sender and recipient, the time the message was sent, or the time computer emails were sent or received are not encrypted. The letter's subject can also remain unprotected and easily readable, even when using E2EE.

Similar to password manager programs, there is also a secret code with the help of which the entire encryption works: this is called a private key, which should never be shared with anyone.

Protecting the secret key and saving it in a place no one can access it is imperative. If you store your secret key unprotected or save it in the cloud without protection, it is easy for someone to steal and use it to read all the encrypted messages you send.

So do not think that by setting up encryption in Thunderbird (or any of the email clients), all your problems are solved and that no one can access the content of your emails (based on the above, anyone can access the metadata even with encryption).

Also, similar to password manager programs, if you lose your secret key (for example, if you lose your computer or if you delete all data on your computer), you will no longer be able to read your encrypted messages. If this happens, no one can recover your messages (unless you have the private key).
