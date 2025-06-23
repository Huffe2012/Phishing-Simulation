# Phishing-Simulation
🧪 Phishing Lab
This lab is focused on analyzing phishing emails in a secure, controlled environment using a Linux-based virtual machine. Tools like Mozilla Thunderbird and Sublime Text are installed to inspect and work with suspicious email messages.

📧 Email Analysis Setup
✅ Install an Email Client
While popular email clients like Outlook or Gmail can be used, we will use Mozilla Thunderbird because it is free, open-source, and works well on Ubuntu.

Install Thunderbird on your Ubuntu VM:

sudo apt install thunderbird
⚠️ Lessons Learned
While installing Thunderbird, the following error occurred:

Failed to fetch http://us.archive.ubuntu.com/ubuntu/pool/main/t/thunderbird/thunderbird_1snap1-0ubuntu3_amd64.deb
Temporary failure resolving 'us.archive.ubuntu.com'
🔍 Root Cause:
The VM was not connected to the internet due to incorrect network settings.

Specifically, the VM was not using NAT (Network Address Translation), which is required for internet access in most VirtualBox configurations.

✅ Resolution:
Updated the network settings in VirtualBox:

Go to Settings > Network for the VM

Set "Attached to:" → NAT

After that, re-ran the install command successfully.

