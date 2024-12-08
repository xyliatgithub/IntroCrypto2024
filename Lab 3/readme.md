## Lab 3 - Public-Key Infrastructure
In this [lab](https://seedsecuritylabs.org/Labs_16.04/PDF/Crypto_PKI.pdf), you will apply your knowledge of certificates authority to explore how to verify the ownership of a public key and gain the first-hand experience on PKI. You will submit a report describing your works and observations. The lab is one of the exercises in [SEED Project](https://seedsecuritylabs.org/index.html). It provides [Virtual Machine (VM) image](https://seedsecuritylabs.org/labsetup.html) in order to simplify setups of experimental environment. We are using the Ubuntu 20.04 image for this lab. Load the VM image with your Virtualbox or VMware, and read the User Manual carefully before you start working on the tasks.

## Environment Setup

### Intel/AMD Machines x86-64

1. Install VirtualBox first, https://www.virtualbox.org/ if you do not have it already. (Note: VirtualBox is available for most consumer computers, If you have trouble with this step, we encourage you to find a solution by yourself.)
2. VM setup instructions (read very carefully): https://github.com/seed-labs/seed-labs/blob/master/manuals/vm/seedvm-manual.md
3. Go to [Lab Environment Setup page](https://seedsecuritylabs.org/labsetup.html) to install the pre-built VM image (for Ubuntu 20.04 VM 64 bits).
4. After building the VM, you can start the VM and log in with the username and password provided in the lab setup page.


### Apple Silicon Machines ARM64
**Note that the Ubuntu image download link in the instructions no longer works. You can install (1) [22.04.5 LTS](https://cdimage.ubuntu.com/releases/jammy/release/) (No GUI) or (2) [24.10](https://cdimage.ubuntu.com/daily-live/current/) (Use the second option if you are not familiar with the first) instead.**
1. Install VMware Fusion first, https://blogs.vmware.com/teamfusion/2024/05/fusion-pro-now-available-free-for-personal-use.html if you do not have it already. (Note: VMware Fusion is available for Apple Silicon M chiip Macs, If you have trouble with this step, we encourage you to find a solution by yourself)
2. VM setup instructions (read very carefully): https://github.com/seed-labs/seed-labs/blob/master/lab-setup/apple-arm/seedvm-fusion.md
3. Go to [Lab Environment Setup page](https://seedsecuritylabs.org/labsetup.html) to install the VM (Ubuntu 22.04).
4. After building the VM, you can start the VM and log in with the username and password provided in the lab setup page.



## Lab Notices
* Please only complete **Tasks 1-4**. You can **skip Tasks 5 and 6**.
### Mix of _SEEDPKILab2018.com_ and _SEEDPKILab2020.com_
* There is a mix of _SEEDPKILab2018.com_ and _SEEDPKILab2020.com_ in the instruction and example command.
* You may want to change all the company names or domain names with **year 2018, replace the year with 2020** in the lab manual. Most significantly, use SEEDPKILab2020.com instead of SEEDPKILab2018.com.
* For Task 3 Step 2, you may want to visit https://SEEDPKILab2020.com:4433/ and check the error message.
<br>**Hint:** You can use ***chmod 666 /etc/hosts*** to change the file permissions; 
<br>&emsp;&emsp; again ***use SEEDPKILab2020.com instead of SEEDPKILab2018.com***
* For Task 4, remember to change the content in the file default-ssl.conf (and remove the ➀ and ➁ symbols). You might not be able to access two.example.com because the corresponding DocumentRoot does not exist. You can set the ServerName to SEEDPKILab2020.com, DocumentRoot into /var/www/html and DirectoryIndex into index.html to see Apache server works. You will get the default page once successful.
<br> **Hint:** You can install Apache on your machine by the following steps if it doesn't exist:
<br>&emsp;&emsp;&emsp;***sudo apt update***
<br>&emsp;&emsp;&emsp;***sudo apt install apache2***
* Include screenshots in your report with adequate explanations. They not only serve as evidences of completion but also help the grader understand what you try to achieve.

## Points Breakdown
This lab has 40 points in total. The four tasks (1, 2, 3, 4) are worth 5, 9, 12, 14 points respectively.

## Grading
* Completeness (30 pts): All the steps as instructed in the lab manual must be included in the report with adequate evidence.
* Presentation (10 pts): The report must be clear and correct in organization and writing with adequate explanation.
