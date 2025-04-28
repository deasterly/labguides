# [Linux Command Line Skills]
## Intro to the Lab Environment

### Getting Lab Access

Instructors will provide learners with a URL to access the lab virtual machines. The URL may contain a built-in authentication token OR the instructor may provide a login and password.
If the lab environment URL requires a username and password, it will typically use the MyLearning Class ID number and lab station numbers in this form:
| LOGIN | PASSWORD |
|:------|:---------|
|class#-lab#@dell.com|class#-lab#|

For example, lab station 6 for class number 12345 would use these credentials:
| LOGIN | PASSWORD |
|:------|:---------|
|12345-6@dell.com|12345-6|

### Logging Into Linux VMs

After logging in, you should a screen like this:

![image](https://github.com/user-attachments/assets/393a07ae-7a4f-4ce0-ae9c-7270f3f2e491)

Use page 4 of the built-in lab guide tab to find information about Linux user credentials and other details about the environment.

![image](https://github.com/user-attachments/assets/9f41b063-f5f9-4710-a3fa-371d862d6111)

After logging into the Ubuntu Desktop with the hostname of **labserver** as the **student** user authenticated with **Passw0rd**, find the icon to launch **Virtual Machine Manager (VMM)** in the Favorite applications under the Activities menu.

 ![image](https://github.com/user-attachments/assets/bc8fe590-77cc-4169-911e-57e49de02edf)

![image](https://github.com/user-attachments/assets/145d2bc0-3a32-4260-be10-6a80046b596d)

After starting **VMM** you will see the Linux VMs running on the Ubuntu **labserver** KVM hypervisor.  Most lab work will be performed on these VMs.

![image](https://github.com/user-attachments/assets/7e01c819-5194-48b4-bf91-81a14c8cd847)

Double-clicking on a VM will open the console for that VM.  Page 4 of the built-in lab guide tab instructs you to log in the console of the **Workstation** VM.

If you see the date and time on the **Workstation** console, this is the desktop lock screen.  Click on the window then press the **`SPACE`** key to unlock the screen, revealing the GNOME Display Manager login screen where you can use the same **student / Passw0rd** credentials.

![image](https://github.com/user-attachments/assets/9162da6b-958d-47b8-b4ad-6e7b6ad9eb9f)

![image](https://github.com/user-attachments/assets/4205c844-4d57-4541-ba58-0a44d634ed5a)

From the Activities menu on the **Workstation** console (not the Ubuntu GNOME Desktop), launch a **Terminal** from the Favorite applications.

![image](https://github.com/user-attachments/assets/fcb8fcfc-d07f-4e69-80dc-bf53586a9c26)

![image](https://github.com/user-attachments/assets/a383b4ef-a9b7-49c0-8b06-9a681fc73054)

To maximize the terminal window, look for the title bar that reads `student@workstation:~` and double-click the title bar.
Then test connectivity to all the remaining VMs with these commands:

`ping -c1 server1`
- > This sends a single ping to the host **server1**

`ping -c1 server2`

`ping -c1 server3`

`ping -c1 infrastructure`

![image](https://github.com/user-attachments/assets/8e0041b4-cb31-4079-be20-0f3bbcfc026e)

They should all respond without errors or timeouts.  If any VMs are not responding, the right-click menu in **VMM** can be used to run, reboot, or reset each VM.

![image](https://github.com/user-attachments/assets/cd3f0cdb-a82b-4fb8-a6d7-a33198edfc57)

If a VM becomes unusable OR if you wish to start over, the console window for each VM has a **Start_Of_Class** snapshot that can be restored by double-clicking, confirming the reversion to the "start of class" state, and finally powering on the VM again.

![image](https://github.com/user-attachments/assets/2d856744-f8f9-4976-b9e9-ededf2c935a8)

![image](https://github.com/user-attachments/assets/eb23d86a-ad5e-4137-8d90-93920aef7153)

At this point, the built-in lab manual tab is no longer needed.  You can make the Ubuntu GNOME Desktop screen resolution larger by collapsing the tab with the **>>** to the left of **Manual**.

![image](https://github.com/user-attachments/assets/5f0af619-aca9-4ca8-908c-b4d5ae19a205)

On the Ubuntu GNOME Desktop of **labserver** open a GNOME Terminal.  The title bar and prompt should read `student@labserver:~`.

![image](https://github.com/user-attachments/assets/79d33604-b80c-411e-8be4-ff88cf96105a)

From this terminal you can open multiple tabs, and log in to all the hosted VMs using SSH if you would like.  

![image](https://github.com/user-attachments/assets/48cb72a7-5fa2-4588-9c01-20bd61487259)

| FQDN | HOSTNAME | DISTRO | VERSION | IPv4 ADDRESS |
|:-----|:---------|-------:|:--------|-------------:|
|labserver.lab.dell|labserver|Ubuntu|20.04.6|192.168.4.1|
|infrastructure.lab.dell|infrastructure|Oracle Linux|8.10|192.168.4.2|
|server1.lab.dell|server1|Oracle Linux|8.7|192.168.4.3|
|server2.lab.dell|server2|Oracle Linux|8.7|192.168.4.4|
|server3.lab.dell|server3|Oracle Linux|9.1|192.168.4.5|
|workstation.lab.dell|workstation|Oracle Linux|8.7|192.168.4.200|



******
