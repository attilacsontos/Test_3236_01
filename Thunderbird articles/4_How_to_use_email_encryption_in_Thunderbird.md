# How to use email encryption in Thunderbird?

## 1. Email encryption in Thunderbird

To use the OpenPGP feature (end-to-end encryption or E2EE), you must set up a public-private key pair for your email address in Thunderbird.

Once your account has been created, Thunderbird offers you to enable end-to-end encryption. Still, you can make this step anytime you want. For security reasons, it is advised to do it as soon as possible. Please navigate to the lower left-hand corner of the screen and click on the gear icon (Settings).

![](http://hdoc.csirt-tooling.org/uploads/upload_fe1b09c1c0f2ffc058a6de63a36ae5ee.png)

The Settings window opens. Choose 'Account Settings' in the lower section of the left panel:

![](http://hdoc.csirt-tooling.org/uploads/upload_9abc0e10d18af024a2d97f271a23818f.png)

The Account Settings window opens. Click on the 'End-To-End Encryption' tab from the drop-down menu on the left panel. To send encrypted emails, you need to configure either OpenPGP or S/MIME. The screenshot below shows that no OpenPGP key is set up yet. 

Click on 'Add Key' to add a personal OpenPGP key for your email:

![](http://hdoc.csirt-tooling.org/uploads/upload_6d8fd6d91fe59733bb65d3ada595180d.png)

If you already have a personal key for your email address, you should import it. 

**If you do not import your existing key:**
„..you will not have access to your Archives of encrypted emails, nor be able to read incoming encrypted emails from people who are still using your existing key!”

If you do not have a personal key associated with your email address, please create a new OpenPGP Key by choosing the first radio button:

![](http://hdoc.csirt-tooling.org/uploads/upload_d199a9662d4228757b66302dd76b0e63.png)

The 'Generate OpenPGP Key' window opens. PGP keys are always linked to an email address, so first, you need to choose your identity from the drop-down menu. Next, you can set up the expiry date of your key.

![](http://hdoc.csirt-tooling.org/uploads/upload_16ff5f1299ea006dc4a67477700a33a7.png)

You may leave the 'Advanced settings' untouched as they often are the best settings security-wise. Click on the 'Generate key' button. The following window opens:

![](http://hdoc.csirt-tooling.org/uploads/upload_c232d11122b10f89d9e65c289353193c.png)

A public and a private key will be generated once you click the 'Generate key' button. While the key is generating, moving your mouse randomly or doing Internet research is essential. The more things you do, the more random your key will be.

![](http://hdoc.csirt-tooling.org/uploads/upload_5fead7cdcb3d252317bcf4ee42ef5324.png)

Send your public key to the people you want to exchange encrypted emails. You can verify other users' keys with your fingerprint. Open the blue area by clicking the down-pointing arrow to reveal your Fingerprint. You may also check your Key Properties. 

![](http://hdoc.csirt-tooling.org/uploads/upload_9b762edb9e95e78dcd3a2d49005223ed.png)

Now, the end-to-end encryption is set up. But there is one essential step that remained. And this is what is discussed in the next chapter.

## 2.	How can you send encrypted emails?

Your encryption keys have been created, and now you should be able to use them. Go to your inbox and click on the button 'Write' to create a new email. When you create a new email, a new tab called 'OpenPGP' appears on the screen. Please note that the sub-menus 'Encrypt' and' Digitally sign' are still inactive.

![](http://hdoc.csirt-tooling.org/uploads/upload_7f66ff18b7d84a7847ff2637f00be7c2.png)

You can encrypt your emails in two ways:

* You can use the 'Encrypt' tab next to 'OpenPGP'
* You can choose the sub-menu 'Encrypt' of the drop-down 'OpenPGP'

You can also digitally sign your emails by using the sub-menu 'Digitally Sign' of the drop-down 'OpenPGP'.

**CAUTION!**

**Your messages in the sent folder will be encrypted if you send encrypted messages. If you lose your private key, you will not be able to read archived messages. These messages cannot be restored!**

**Likewise, if you lose your private key, others can still send you encrypted emails, and you will not be able to read them.**

Also, note that search functions generally do not work for the body of encrypted messages. It is essential to know that you can only send encrypted emails to those who are similarly able to receive and send encrypted emails. If you want to send an encrypted message to an email address whose public key is not saved on our computer, you receive the following error message:

![](http://hdoc.csirt-tooling.org/uploads/upload_85d0059ab6c23e6ca2124965903984a6.png)

To solve the problem, you can decide not to encrypt your message. Alternatively, you may try to resolve the issue by clicking the ’Resolve…’ button. If you click on the ’Resolve…’ button, the OpenPGP Assistant window opens and informs you that you do not have the key to the recipient’s email address:

![](http://hdoc.csirt-tooling.org/uploads/upload_0259c25e4c63344c0358c13b783b4da4.png)

You can try to discover your recipient’s public key online or import it if your recipient has sent it to you already. If you click the ’Discover Public Keys Online…’ button and Thunderbird cannot find your recipient’s public key online, you will be directed back to the OpenPGP Assistant window. In this case, you should click on ’Disable encryption’ to be able to send an unencrypted email to your recipient. You may ask your recipient in an unencrypted email to send you his/her public key, so after importing it, you can send encrypted emails to each other.

## 3.	How can you send your public key to other people?

After you have created your private key, you must allow others to obtain your public key. Be careful, and never share your private key with anyone. However, the public key can be widely shared, so people can send you encrypted emails and verify your digital signatures. This is how it works:

1. Start writing a new email
1. Navigate to and click on the 'Attach' drop-down in the top right-hand corner
1. Chose the sub-menu 'My OpenPGP Public Key'

![](http://hdoc.csirt-tooling.org/uploads/upload_c5713956cdff43742dc2c4c6f451e9bb.png)

Your recipient will see an attachment in the email with a file name starting with "OpenPGP". If your recipients are using Thunderbird, they can right-click on the message to open a menu of options and select "Import OpenPGP Key" from that menu.

## 4.	How to export your OpenPGP public key?

Go to ’Tools’ in the menu bar and choose the sub-menu ’OpenPGP Key Manager’:

![](http://hdoc.csirt-tooling.org/uploads/upload_6bc3f7134ceaf19046f2f98917568a0a.png)

Select the OpenPGP public key you want to export and choose the ’Export Public Key(s) To File’ drop-down menu.

![](http://hdoc.csirt-tooling.org/uploads/upload_8c45a1fc379cc6842ef6f5fa80fdc8e1.png)

Alternatively, open account settings and select the end-to-end encryption panel to download your OpenPGP keypair's public key directly. Click on the drop-down menu ’More’ and choose the sub-menu ’Export Public Key(s) To File’.

![](http://hdoc.csirt-tooling.org/uploads/upload_9fa7c5432f00b2b862b2ebe2cb579a0d.png)

## 5.	How to exchange public keys?

Everyone to whom you send encrypted messages must have their own public key. Your recipients also need yours so they can send encrypted messages back to you. There are a few ways to get someone's public key. They may send it to you without notice, or you may ask them to do so. You can even try to find your recipients’ public keys online.

### 5.1.	Find a public key online

Go to a key server, for example, https://keys.openpgp.org/ and search by email address, Key ID or Fingerprint:

![](http://hdoc.csirt-tooling.org/uploads/upload_87ee205ae0cd0bfe086829c952696bd2.png)

In case there is a record for the searched item on the server, you can see the owner of the public key and see the owner’s fingerprint:

![](http://hdoc.csirt-tooling.org/uploads/upload_e2a6c3af3020709dbe381d20c03d572e.png)

You can download the owner’s public key by clicking on the link:

![](http://hdoc.csirt-tooling.org/uploads/upload_fa70f3d27c61851fa31a8f3af43efe22.png)

### 5.2.	You receive someone’s public key

Thunderbird includes an 'OpenPGP' button to the right of the email header when you receive an email with an attached public key. The screenshot below shows a message signed with the sender’s public key. 

Also, it was digitally signed, so the certificate icon indicates it. Since this is the first time you have received the below message from your sender, Thunderbird does not know whether the signature is valid (this is why the application shows a question mark next to the icon).

![](http://hdoc.csirt-tooling.org/uploads/upload_793a8dc514ce374067270ac51e6fecba.png)

If you click on the OpenPGP button, the below window pops up:

![](http://hdoc.csirt-tooling.org/uploads/upload_f6297275716218290015f9b1ffd9b119.png)

The message says that you still do not have this public key, so you need to import it. Besides that, you need to verify that the digital signature is valid.

Click on the ’Discover’ button. The popup informs you that the email attachment contains the sender's public key, and the message shows the sender’s fingerprint and email aliases. By looking at the email addresses, you should be able to identify the sender to import the public key.

In the lower part of the window, you can verify (accept) the signature of the sender.

![](http://hdoc.csirt-tooling.org/uploads/upload_e9de7b2907bb39ad7610005c08bc7119.png)

Let’s choose the radio button ’Accepted (unverified)’ and click on the button ’Import’ in the lower right-hand corner. The following window informs you that the public key was imported successfully:

![](http://hdoc.csirt-tooling.org/uploads/upload_157f9fa6511a1e8a2093d2747a105b51.png)

By clicking on the link at the bottom of the window, you can view the details and manage the key acceptance (do not forget that you just imported the public key successfully, you have not verified it yet).

At the top, you see the key properties (owner, type, Key ID, Fingerprint, Created, Expiry); in the lower section, you have four tabs to choose from. The first tab is the ’Your Acceptance’ tab:

Here, you can decide whether you want to reject the key, or you accept it but have not verified yet, or accept and verify the key that it belongs to the sender:

![](http://hdoc.csirt-tooling.org/uploads/upload_cd6736b6d164eefb1e987a5066fdd111.png)

How can I verify the public key? See Chapter ’5.1. Find a public key online’.

Since I know who the sender is, let me choose the option to verify that the public key and the digital signature are valid:

![](http://hdoc.csirt-tooling.org/uploads/upload_af1fda6c78b44bf9900ce2dd5bccca08.png)

Since I have verified the sender’s public key and digital signature, the icons in the top right-hand corner of the email have changed. A green checkmark appears on the key and certificate icon.

![](http://hdoc.csirt-tooling.org/uploads/upload_5d732bef9361f9777b0335d131657d46.png)

If you click on the icon, the below window opens and informs you that the digital signature is valid and the message is encrypted.

![](http://hdoc.csirt-tooling.org/uploads/upload_9d91f25c1d522111f334148c67321fba.png)

From now on, you can continue sending and receiving encrypted messages with your email partner.

## 6.	How can you upload your public key?

Go to a key server (for example, https://keys.openpgp.org/ ) and choose the link ’upload’.

![](http://hdoc.csirt-tooling.org/uploads/upload_5bbbcd970e15c74ce77015a82c26b50d.png)

As the next step, click on ’Choose File’ and click on the ’Upload’ button on the right.

![](http://hdoc.csirt-tooling.org/uploads/upload_eedd0a500f03cc63a04642428fd8ce13.png)

If the upload process is successful, you receive a similar message as the one below:

![](http://hdoc.csirt-tooling.org/uploads/upload_94afb1b6f09292eb4e194a2798c94b9d.png)

You may send a verification email to yourself by clicking on the ’Send verification Email’. Shortly, you will receive a similar email as follows:

![](http://hdoc.csirt-tooling.org/uploads/upload_4d7bf76e5d6301201a87118116e6cfa7.png)

## 7.	How can you exchange encrypted emails with others?

### 7.1.	The theory

Thunderbird's OpenPGP integration allows you to encrypt your email messages. After that, only those whom you want to read your message can do so. This integration also allows the message to be digitally signed, so the recipient can be sure that the message has not been altered in transit.

OpenPGP uses the principle of a pair of public and private (or 'secret') encryption keys. To use OpenPGP, you must have a public and a private key pair. Public keys should be shared with anyone you want to send encrypted messages to, while private keys are never shared with anyone else. Private keys can also decrypt messages encoded with the corresponding public key.

The sender's email client generates a random key to encrypt the message. The random key is then encrypted with the recipient's public key, and the encrypted message and key are sent to the recipient. The recipient's email program uses the recipient's private key to decrypt the random key. The random key can then be used to decrypt the encrypted message.

A random key is encrypted for each recipient with that person's public key. All encrypted keys are then sent with the message. Each recipient can decrypt a copy of the random key encrypted with their public key and then use the random key to decode the message.

### 7.2.	What is needed to send an encrypted message?

You must have your private (secret) and public keys set up. Each recipient of your encrypted message must have an accepted public key.

You should verify that the public keys of your correspondence partners really belong to them. Accepting someone's public key without verifying exposes your communication to Man In The Middle (MITM) attacks.

If you do not have a public key for a particular recipient, the message will be blocked from being sent, and Thunderbird will warn you. You can choose not to send the message at all, disable encryption and send the message unprotected, or send the message only to a subset of recipients who have public keys.

### 7.3.	What does key acceptance mean?

Anyone can create a private key on behalf of anyone using any email address. It means that every time you receive an encrypted email from someone with their public key, by accepting it without validating the keys, you risk the key being fake and open yourself up to being scammed.

In connection with encrypted correspondence, it happens less often that we receive emails from complete strangers. If this does happen, an extra filter often enters, meaning we authenticate the sender of the email through a telephone inquiry or another communication channel.

Maybe you talked to someone a few minutes ago and agreed they would send you an email. The point is to ensure that the email arrives in your mailbox is authentic.
For many, this may seem like an unnecessary hassle or extra pointless work. However, the essence of encrypted email communication would be to exchange information with reliable partners.

For further reading on end-to-end encryption in Thunderbird, please read the article [Introduction to End-to-end encryption in Thunderbird](https://support.mozilla.org/en-US/kb/introduction-to-e2e-encryption).

Once you have set up your private key, you can control whether encryption or digital signatures are used for each message you send. After you have created your private key, allow others to obtain your public key so that you can conduct secret email communications. 

## 8.	Limitations of end-to-end encryption

End-to-end encryption (E2EE) requires caution from both the sender and the recipient. A single mistake by any involved party can be enough to breach E2EE security. 

Also, another limitation of end-to-end encryption is that email metadata cannot be protected. For example, the name and address of the sender and recipient, the time the message was sent, or the time computer emails were sent or received are not encrypted. The letter's subject can also remain unprotected and easily readable, even when using E2EE.

Similar to password manager programs, there is also a secret code with the help of which the entire encryption works: this is called a private key, which should never be shared with anyone.

Protecting the secret key and saving it in a place no one can access it is imperative. If you store your secret key unprotected or save it in the cloud without protection, it is easy for someone to steal and use it to read all the encrypted messages you send.

So do not think that by setting up encryption in Thunderbird (or any of the email clients), all your problems are solved and that no one can access the content of your emails (based on the above, anyone can access the metadata even with encryption).

Also, similar to password manager programs, if you lose your secret key (for example, if you lose your computer or if you delete all data on your computer), you will no longer be able to read your encrypted messages. If this happens, no one can recover your messages (unless you have the private key).