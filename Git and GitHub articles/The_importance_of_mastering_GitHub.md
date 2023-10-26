# Git and GitHub

## 1. What is the purpose of this document?

This document aims to show you how to use Git and GitHub in as simple and easy-to-follow steps as possible to create version-tracked and easily shareable documents.

However, for this, some basic concepts must first be clarified to understand why it is worth using Git and GitHub, what version control is and why it is better to use this method than, for example, to create separate Word documents and manage the content through it.

When people hear Git or GitHub, they immediately think developers use them for coding, tracking conversions, collaborative code development, etc. And this is indeed true, as both tools are prevalent among developers. But the purpose of this document is to explain comprehensibly, even for non-developers, how to use these two tools effectively to create content and prove that 'general users' can also use them successfully in many cases.

## 2. What is version control?

There are two fundamental aspects to consider when creating content:

The first is that we can track the changes made to the content; we know when and who made what changes to the given content, and we should also be able to return to any previous versions if we see that the latest version is not the best.

The second aspect is that the content we create should be easily shareable: others can express their opinions as efficiently as possible and make suggestions for improving the content. Also, the content creator should be able to integrate these improvements and modifications into the latest version easily: version control is about controlling and tracking different versions of a given project. 

A sound version control system (VCS) tracks and records changes to any file (or group of files), allowing you to revert to earlier versions when necessary. Version tracking enables team members working elsewhere in space and time to communicate with each other and develop specific content.

The most significant advantage of version tracking is that everyone sees the latest content and can make constructive comments and suggestions, thereby improving the quality of the given content.

## 3. What is Git?

Git is a distributed, open-source version control system.

By distributed, we mean there is no central data repository, but its users download the Git source code to their machine and use it to modify the content they create (code, text and other types of content).

Git is open-source because it can be freely used, copied, distributed, studied and modified.

Git is also a version control software: actually, it is so popular that [Git is used by more than 90% of professional developers](https://www.datacamp.com/blog/all-about-git).

With its help, you can store your created content, perform version tracking, and send it to GitHub.

## 4. What is GitHub?

GitHub is a cloud-based repository hosting service that allows team members to work together and manage their content. 

A repository (usually abbreviated as "repo") is where all files belonging to a given project are stored. Each project has its own repo and can be accessed via a unique URL.

Github has three main functionality groups: a cloud repository, a collaborative development platform and a project management tool.

If you want to create and develop content, you can do it without GitHub. Git is perfectly sufficient so that you can return to an earlier version of the given content at any time by using its version control capabilities, and you can also store the content in it. Therefore, you do not need to look for a cloud service provider but store the data locally on your computer.

However, in the case of locally stored data, there is a considerable risk of complete data loss in the event of a computer failure.

Most people create backups to avoid this. In the case of backup copies, however, there is no explicit version tracking, and especially if the version number of a particular piece of content increases a lot, it makes it very difficult to perform proper version tracking. After a while, we will not know which version has changed and which has not. Another huge disadvantage of storing content locally is that it makes joint work with others almost impossible.

To solve these burning problems, GitHub was born in 2008 to make working with Git as easy as possible. Today, Git and GitHub are complementary technologies that help each other work together as efficiently as possible.

The content created in Git is saved and stored in a remote repository on GitHub, and we make changes to the content either in Git or directly on GitHub and take advantage of the benefits provided by these popular tools.

If, after this, you think you give a chance to use Git and GitHub to create content, then please stay with me and let's get down to business: let's see how to install Git, create a repository on Github, create content and develop it collaboratively.

## 5. How to install Git?

The best way to install Git is to go to the official Git website, choose your operation system and download it from there. Git supports all operating systems, and the process is hassle-free. Once the download is complete, run the installer and follow the steps required.

There are various options during installation, but the default settings are sufficient for most users.

![](http://hdoc.csirt-tooling.org/uploads/upload_92a7884a81763d26a279b2b0e30d8c46.png)

After choosing your installation options, the installer installs Git on your computer.

Git is designed to be used by more than one person. After successful installation, use the Git Config command and set the username and user email address you want to use. Since Git is a terminal without having a usual user interface, this code should be written in the Git command line interface as follows:

git config --global user.name "your-user-name"
git config --global user.email "your@email.com"

The global option ensures that every project on your computer will use the same name and email address. You may use your GitHub email address here if you already have a GitHub account. After the installation, please verify that Git has been installed correctly: open your comment prompt and run the command as follows:

git --version

After hitting enter, your current Git version should be displayed and look something like this:

git version 2.42.0.windows.2.

![](http://hdoc.csirt-tooling.org/uploads/upload_92fe28da0bd405538d6001f177c11358.png)

## 6. How to initialize Git?

Once you configured Git, the next step is to prepare the folder that will hold the project. With the following command, you can initialize an empty repository on your machine:

% git init

When you initialize Git, it creates an invisible folder called .git in the project folder, where Git stores all the information about the project. Git is going to write these files for you and take care of keeping track of what the project is doing.

In order to create an entry that we can go back to, we have to add the files to the staging environment. With the add command, staging is a temporary area where we can store files that we want to commit later on; you use the git add command and specify the file name that you want to move to staging:

% git add FILENAME

The last step in the process is to commit the files with the commit command. Look at the commit command as if you had pressed the save button in a regular application: we are creating a 'snapshot' of our content, a point to which we can return later if necessary.

You always need to include a message for this, and the syntax for that is as follows: 

% git commit -m "First commit"

It tells Git that this is one of the checkpoints you want to track for your project so that you can return to it later.

### 6.1. Why is it so important? 

Do you remember we said that Git is a version tracking software, the essence of which is to log the changes of a given file or content over time and to be able to view any previously created version at any time?

For each commit, it is worth giving a short but good description of what kind of change you made so that when you look back in three months or half a year, you can still remember what that change was.

Also, let's not forget that the 'soul' of Git and GitHub is cooperation, collaborative work, content and code sharing (open-source projects), and in light of this, your commit comment must be understandable to others as well.



