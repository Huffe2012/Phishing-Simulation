# Phishing-Simulation
🧪 Phishing Lab
This lab is focused on analyzing phishing emails in a secure, controlled environment using a Linux-based virtual machine. Tools like Mozilla Thunderbird and Sublime Text are installed to inspect and work with suspicious email messages.

**Email Analysis Setup**
Install an Email Client
Companies typically use email clients like Outlook or Gmail can be used, I used Mozilla Thunderbird because it is free, open-source, and works well on Ubuntu.

**Installed Thunderbird on your Ubuntu VM**:

~$ sudo apt install thunderbird
![Screenshot 2025-06-22 210202](https://github.com/user-attachments/assets/9a379cff-38b9-43a6-8b1f-d437696e8b6f)


**Lessons Learned**
While installing Thunderbird, the following error occurred:

Failed to fetch http://us.archive.ubuntu.com/ubuntu/pool/main/t/thunderbird/thunderbird_1snap1-0ubuntu3_amd64.deb
Temporary failure resolving 'us.archive.ubuntu.com'
**Root Cause**:
The VM was not connected to the internet due to incorrect network settings.

The VM was not using NAT (Network Address Translation), which is required for internet access in most VirtualBox configurations.

**Resolution:**
Updated the network settings in VirtualBox:

Go to Settings > Network for the VM

Set "Attached to:" → NAT

After that, re-ran the install command successfully.


**Added Sublime Text**
-Downloaded linux sublime text from: https://www.sublimetext.com/docs/linux_repositories.html

![Screenshot 2025-06-22 210520](https://github.com/user-attachments/assets/942d6c75-3375-4a08-a461-f94ebeb04d01)
