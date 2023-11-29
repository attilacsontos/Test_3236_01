# How to connect your Zimbra calendar to Thunderbird?

You can connect your Zimbra calendar to Thunderbird in two ways: you may share or move your calendar.

**Share:**

In this case, you continue to use your Zimbra instance and make your calendar available to a user (or users) who use Thunderbird (or another mail program).

**Move (import):**

In this case, you decide to use Thunderbird instead of Zimbra. Therefore, you first export your calendar from Zimbra, then import it into Thunderbird and continue your work in Thunderbird.

In both cases, you need to use the Lightning Add-on, so first, check if it is installed in Thunderbird.

## 1.	Check whether you have the Lightning Add-on

To view your Zimbra Calendar in Thunderbird, first, you need to download the Lightning Add-on for Thunderbird. Since Thunderbird version 38, [Lightning is bundled](https://support.mozilla.org/en-US/kb/installing-lightning-thunderbird) with the application. Go to the Add-ons Manager to check it. 

![](http://hdoc.csirt-tooling.org/uploads/upload_fc7854be6d8a981444f66e98da7e5068.png)

To configure this add-on, choose the ’Events and Tasks’ top menu and then the ’LCT Options’ sub-menu.

![](http://hdoc.csirt-tooling.org/uploads/upload_efeb9917f41fd2fd57e5eb3aaec8659b.png)

The Calendar tab settings window opens up, so you can make many setting changes.

![](http://hdoc.csirt-tooling.org/uploads/upload_a19d926cdfd0fb0847a446453ecd5678.png)

## 2.	How to share your Zimbra Calendar?

Open your calendar in Zimbra. Then choose the calendar you want to share, right-click on the name of it and choose ’Share Calendar’ in the pop-up menu.

![](http://hdoc.csirt-tooling.org/uploads/upload_d797ce35cdbf6cad061c362fceebc753.png)

The Share Properties window opens. You can set whether you want to share the chosen calendar with internal-, external, or public users (so anyone can access it without a password – if you share the link of the calendar with the person).

![](http://hdoc.csirt-tooling.org/uploads/upload_913cc9d4fc9f9aa28f8d992b0fe90148.png)

Also, you can set the ’Role’, that is, the user's access right (with options as follows: None, View, Edit, Add, Remove, Administer). You can also message the person you share your calendar with.

Last but not least, you need to share a link to your calendar (the URL can be seen at the bottom of the window, this part of the screenshot has been removed). Please follow general cybersecurity hygiene techniques while sharing URLs with others: failure to comply with the recommendations may result in unauthorized persons gaining access to your calendar and being able to see who and when you have meetings with.

Now, you need to open Thunderbird and navigate to its calendar. Right-click on the lower section of the left panel, where you can see the list of your calendars (in the below screenshot, the calendars ’Home’ and ’Calendars’ have already been added. From the pop-up menu, please choose the option ’New Calendar…’

![](http://hdoc.csirt-tooling.org/uploads/upload_d159ff67031e9afd10da30ebc268aeb7.png)

Alternatively, click on the ’+’ sign. Either way, the ’Create New Calendar’ window opens, where you can choose whether to create your calendar locally (On My Computer), access it remotely, or share it with your friends or co-workers (On the Network).

![](http://hdoc.csirt-tooling.org/uploads/upload_c893566cdcec82c488b9d28343d63d59.png)

Unless you want to use your calendar only at home (and do not want to share it with anyone), you want to create a calendar somewhere on the network and accessible to other people. Check the ’On the Network’ radio button and click ’Next’.

Then, populate the fields ’Username’ and ’Location’. The username is the e-mail address you use for your Zimbra account, whereas the ’Location is the URL or host name of the server you log in when you use your Zimbra calendar.	 

![](http://hdoc.csirt-tooling.org/uploads/upload_70a0abafe9685b02ba4a274ccea06159.png)

Populate the fields. If you run into difficulties, please contact your administrator (or your Helpdesk).

![](http://hdoc.csirt-tooling.org/uploads/upload_94c2925857f44241c0739a4bac1051cf.png)

Enter your Zimbra password and click ’OK’ to verify your account. The following window opens, where you can decide whether to subscribe (link) to your calendar, tasks, or both (using the relevant checkboxes).

![](http://hdoc.csirt-tooling.org/uploads/upload_1057356777e3ce54e827f2e09e135158.png)

Click ’Subscribe’, so the chosen calendar and tasks have been linked to your Thunderbird instance (so you can see them from Thunderbird).

![](http://hdoc.csirt-tooling.org/uploads/upload_7caac2c529cfeafe329e2b489cca8b88.png)

## 3.	How to move (import) your Zimbra Calendar into Thunderbird?

First, you need to export your calendar from Zimbra. Go to 'Preferences, and choose the option 'Import/Export'. In the field 'Export', choose Calendar as type and click on the button 'Export' to create an iCalendar (.ics) file.

![](http://hdoc.csirt-tooling.org/uploads/upload_df542b6c18088df2743cada6ba28cbee.png)

Then, open your Thunderbird and choose the top menu 'Events and Tasks' and the submenu 'Import…' from the dropdown menu:

![](http://hdoc.csirt-tooling.org/uploads/upload_d8ac5a1d798ca6776af3cdf09c272fcb.png)

Once you click on 'Import…', the Import wizard opens. 

![](http://hdoc.csirt-tooling.org/uploads/upload_649b5f924be7271cc615e32ac26f9978.png)

Please follow the steps required, and click on 'Continue'. In the second step, you can choose where to import your .ics file (that is why it is advisable to create and rename your calendar before importing it, so your previously-created calendar will show up in the list. If you have not created a calendar earlier, you may create a new one in the second step by choosing "Create a new calendar called…'.

![](http://hdoc.csirt-tooling.org/uploads/upload_65cfb0dcf2e68e47968825f6b44af2fb.png)

Click ‘Continue’ so you are directed to the next step. Here, you can see how many calendar items are imported and where the source file is located.

![](http://hdoc.csirt-tooling.org/uploads/upload_3770e3ff946350ab9adb0616036cfd76.png)

Click ‘Start Import’ and wait while your Calendar is imported. The last screen shows the process of the import, which you can acknowledge by clicking on the 'Finish' button:

![](http://hdoc.csirt-tooling.org/uploads/upload_429cabe9c1212d5e3dcc3ffae81a987b.png)

Once imported, the calendar is shown among your calendars in Thunderbird. Do not worry about the name of the calendar. You can change it any time by right-clicking on the calendar’s name, then selecting the 'Properties' dropdown menu option and changing the calendar's name in the pop-up window.

![](http://hdoc.csirt-tooling.org/uploads/upload_60043a75411726e0fbffb80bffc29d81.png)

## 4.	Further links related to this topic

1. Official Thunderbird website – Lightning Calendar
https://www.thunderbird.net/en-US/calendar/
2. Official Thunderbird website – Support site Related to the Lightning add-on for Calendar
https://support.mozilla.org/en-US/products/thunderbird/calendar
3. Thunderbird Blog post - Why We’re Rebuilding The Thunderbird Interface From Scratch
https://blog.thunderbird.net/2023/02/the-future-of-thunderbird-why-were-rebuilding-from-the-ground-up/
4. Zimbra Wiki site - Accessing Zimbra Collaboration with Thunderbird
https://wiki.zimbra.com/wiki/Accessing_Zimbra_Collaboration_Server_with_Thunderbird
5. Syncing Zimbra calendars using Thunderbird & CalDAV
https://system.cs.kuleuven.be/cs/system/software/Zimbra-calendar/Thunderbird-CalDAV-setup.shtml
