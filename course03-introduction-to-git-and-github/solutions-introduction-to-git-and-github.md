# Solutions to Problems in Introduction to Git and GitHub

## Week 1

### Course Introduction

### Before Version Control

#### Practice Quiz: Before Version Control

***Solution 01***

- [x] `patch fix_names.conf < fix_names.patch`

***Solution 02***

- [x] `diff fix_permissions.py fix_permissions_modified.py > fix_permissions.patch`

***Solution 03***

- [x] `wdiff`

***Solution 04***

- [x] Using the exit command from the sys module

***Solution 05***

- [x] Diff file

### Version Control Systems

#### Practice Quiz: Version Control Systems

***Solution 01***

Multiple answers:

- [x] Git retains local copies of repositories, resulting in fast operations.
- [x] If something breaks due to a change, you can fix the problem by reverting to a working version before the change.
- [x] Git allows you to review the history of your project.

***Solution 02***

- [x] Linus Torvalds

***Solution 03***

- [x] Version control

***Solution 04***

- [x] commit

***Solution 05***

- [x] repositories

### Using Git

#### Practice Quiz: Using Git

***Solution 01***

- [x] `git add`

***Solution 02***

- [x] `git log`

***Solution 03***

- [x] `git add`

***Solution 04***

- [x] `git config -l`

***Solution 05***

- [x] `git status`

### Module 1 Review

#### Qwiklabs Assessment: Introduction to Git

##### Introduction

In this scenario, you are a project lead in an IT company. You and your team are working on a huge project, which consists of multiple functionalities and modules. This project is evolving over time and so your team is expecting a lot of code revisions. In this lab, you'll learn how to use a distributed version control system called Git. You'll also discover how to connect to a VM instance, install Git, and configure your Git user information. Next, you'll create a local Git repository, add a file to the repository, and do some basic operations like adding a file, editing files, and making commits.

What you'll do

- Create a git repository.
- Add files to this repository
- Edit the files
- Commit the changes to the repository.

You'll have 90 minutes to complete this lab.

###### Start the lab

You'll need to start the lab before you can access the materials in the virtual machine OS. To do this, click the green “Start Lab” button at the top of the screen.

<p align="left">
    <img src="../images/introduction-to-git-and-github-week-01-start-lab.png" alt="../images/introduction-to-git-and-github-week-01-start-lab.png" width="10%" height="10%">
</p>

Note: For this lab you are going to access the Linux VM through your local SSH Client, and not use the Google Console (Open GCP Console button is not available for this lab).

After you click the “Start Lab” button, you will see all the SSH connection details on the left-hand side of your screen. You should have a screen that looks like this:

<p align="center">
    <img src="../images/introduction-to-git-and-github-week-01-ssh-connection.png" alt="../images/introduction-to-git-and-github-week-01-ssh-connection.png" width="50%" height="50%">
</p>

##### Accessing the virtual machine

Please find one of the three relevant options below based on your device's operating system.

Note: Working with Qwiklabs may be similar to the work you'd perform as an IT Support Specialist; you'll be interfacing with a cutting-edge technology that requires multiple steps to access, and perhaps healthy doses of patience and persistence(!). You'll also be using SSH to enter the labs -- a critical skill in IT Support that you’ll be able to practice through the labs.

###### Option 1: Windows Users: Connecting to your VM

In this section, you will use the PuTTY Secure Shell (SSH) client and your VM’s External IP address to connect.

**Download your PPK key file.**

You can download the VM’s private key file in the PuTTY-compatible PPK format from the Qwiklabs Start Lab page. Click on Download PPK.

<p align="center">
    <img src="../images/introduction-to-git-and-github-week-01-download-ppk.png" alt="../images/introduction-to-git-and-github-week-01-download-ppk.png" width="50%" height="50%">
</p>

**Connect to your VM using SSH and PuTTY**

1. You can download Putty from [here](https://the.earth.li/~sgtatham/putty/latest/w64/putty.exe)

2. In the Host Name (or IP address) box, enter username@external_ip_address.

Note: Replace username and external_ip_address with values provided in the lab.

<p align="center">
    <img src="../images/introduction-to-git-and-github-week-01-putty-config.gif" alt="../images/introduction-to-git-and-github-week-01-putty-config.gif" width="50%" height="50%">
</p>

3. In the Connection list, expand SSH.

4. Then expand Auth by clicking on + icon.

5. Now, select the Credentials from the Auth list.

6. In the Private key file for authentication box, browse to the PPK file that you downloaded and double-click it.

7. Click on the Open button.

Note: PPK file is to be imported into PuTTY tool using the Browse option available in it. It should not be opened directly but only to be used in PuTTY.

<p align="center">
    <img src="../images/introduction-to-git-and-github-week-01-putty-config-ssh-connection-auth.gif" alt="../images/introduction-to-git-and-github-week-01-putty-config-ssh-connection-auth.gif" width="50%" height="50%">
</p>

8. Click Yes when prompted to allow a first connection to this remote SSH server. Because you are using a key pair for authentication, you will not be prompted for a password.

**Common issues**

If PuTTY fails to connect to your Linux VM, verify that:

- You entered `<username>@<external ip address>` in PuTTY.
- You downloaded the fresh new PPK file for this lab from Qwiklabs.
- You are using the downloaded PPK file in PuTTY.

###### Option 2: OSX and Linux users: Connecting to your VM via SSH

**Download your VM’s private key file.**

You can download the private key file in PEM format from the Qwiklabs Start Lab page. Click on Download PEM.

<p align="center">
    <img src="../images/introduction-to-git-and-github-week-01-download-pem.png" alt="../images/introduction-to-git-and-github-week-01-download-pem.png" width="50%" height="50%">
</p>

**Connect to the VM using the local Terminal application**

A terminal is a program which provides a text-based interface for typing commands. Here you will use your terminal as an SSH client to connect with lab provided Linux VM.

1. Open the Terminal application.
   - To open the terminal in Linux use the shortcut key Ctrl+Alt+t.
   - To open terminal in Mac (OSX) enter cmd + space and search for terminal.
2. Enter the following commands.

Note: Substitute the path/filename for the PEM file you downloaded, username and External IP Address.

You will most likely find the PEM file in Downloads. If you have not changed the download settings of your system, then the path of the PEM key will be ~/Downloads/qwikLABS-XXXXX.pem

```code
chmod 600 ~/Downloads/qwikLABS-XXXXX.pem
```

```code
ssh -i ~/Downloads/qwikLABS-XXXXX.pem username@External Ip Address
```

<p align="center">
    <img src="../images/introduction-to-git-and-github-week-01-ssh-command-connecting-vm.png" alt="../images/introduction-to-git-and-github-week-01-ssh-command-connecting-vm.png" width="50%" height="50%">
</p>

###### Option 3: Chrome OS users: Connecting to your VM via SSH

Note: Make sure you are not in Incognito/Private mode while launching the application.

**Download your VM’s private key file.**

You can download the private key file in PEM format from the Qwiklabs Start Lab page. Click on Download PEM.

<p align="center">
    <img src="../images/introduction-to-git-and-github-week-01-download-pem.png" alt="../images/introduction-to-git-and-github-week-01-download-pem.png" width="50%" height="50%">
</p>

**Connect to your VM**

1. Add Secure Shell from [here](https://chrome.google.com/webstore/detail/secure-shell/iodihamcpbpeioajjeobimgagajmlibd) to your Chrome browser.

2. Open the Secure Shell app and click on [New Connection].

<p align="center">
    <img src="../images/introduction-to-git-and-github-week-01-vm-new-connection.png" alt="../images/introduction-to-git-and-github-week-01-vm-new-connection.png" width="50%" height="50%">
</p>

3. In the username section, enter the username given in the Connection Details Panel of the lab. And for the hostname section, enter the external IP of your VM instance that is mentioned in the Connection Details Panel of the lab.

<p align="center">
    <img src="../images/introduction-to-git-and-github-week-01-vm-username-hostname.png" alt="../images/introduction-to-git-and-github-week-01-vm-username-hostname.png" width="50%" height="50%">
</p>

4. In the Identity section, import the downloaded PEM key by clicking on the Import… button beside the field. Choose your PEM key and click on the OPEN button.

Note: If the key is still not available after importing it, refresh the application, and select it from the Identity drop-down menu.

5. Once your key is uploaded, click on the [ENTER] Connect button below.

<p align="center">
    <img src="../images/introduction-to-git-and-github-week-01-vm-identity.png" alt="../images/introduction-to-git-and-github-week-01-vm-identity.png" width="50%" height="50%">
</p>

6. For any prompts, type yes to continue.

7. You have now successfully connected to your Linux VM.

You're now ready to continue with the lab!



## Week 2

### Advanced Git interaction

#### Practice Quiz: Advanced Git Interaction

***Solution 01***

- [x] `git mv`

***Solution 02***

- [x] A file containing a list of files or filename patterns for Git to skip for the current repo.

***Solution 03***

- [x] New files

***Solution 04***

- [x] The currently checked-out snapshot of your project

***Solution 05***

- [x] `--stat`

### Undoing Things

#### Practice Quiz: Undoing Things

***Solution 01***

- [x] `git revert``

***Solution 02***

- [x] use the commit ID at the end of the git revert command

***Solution 03***

- [x] To guarantee the consistency of our repository

***Solution 04***

- [x] Overwrite the previous commit

***Solution 05***

- [x] `git show`

### Branching and Merging

### Module 2 Review

## Week 3

### Introduction to GitHub

### Using a Remote Repository

### Solving Conflicts

### Module 3 Review

## Week 4

### Pull Requests

### Code Reviews

### Managing Projects

### Module 4 Review

### Course Wrap Up
