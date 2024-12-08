
## Lab 2 - Secret-Key Encryption
This [lab](https://seedsecuritylabs.org/Labs_20.04/Files/Crypto_Encryption/Crypto_Encryption.pdf) will apply your knowledge of block cipher modes of operation to find out some interesting results. You have to complete five tasks in this lab and submit a report describing your works and observations. The lab is one of the exercises in [SEED Project](https://seedsecuritylabs.org/Labs_20.04/Crypto/). Load the VM image with your Virtualbox or VMware, and read the User Manual carefully before you start working on the tasks.

## Environment Setup

### Intel/AMD Machines x86-64

1. Install VirtualBox first, https://www.virtualbox.org/ if you do not have it already. (Note: VirtualBox is available for most consumer computers, If you have trouble with this step, we encourage you to find a solution by yourself.)
2. VM setup instructions (read very carefully): https://github.com/seed-labs/seed-labs/blob/master/manuals/vm/seedvm-manual.md
3. Go to [Lab Environment Setup page](https://seedsecuritylabs.org/labsetup.html) to install the pre-built VM image (for Ubuntu 20.04 VM 64 bits).
4. After building the VM, you can start the VM and log in with the username and password provided in the lab setup page.
5. Download the lab specific zip file (Labsetup.zip) from the [lab page](https://seedsecuritylabs.org/Labs_20.04/Crypto/Crypto_Encryption/). You can download it directly on the VM or download it on your host machine and transfer it to the VM using the shared folder feature of VirtualBox.
6. Unzip the setup file and start your lab.

### Apple Silicon Machines ARM64
**Note that the Ubuntu image download link in the instructions no longer works. You can install (1) [22.04.5 LTS](https://cdimage.ubuntu.com/releases/jammy/release/) (No GUI) or (2) [24.10](https://cdimage.ubuntu.com/daily-live/current/) (Use the second option if you are not familiar with the first) instead.**
1. Install VMware Fusion first, https://blogs.vmware.com/teamfusion/2024/05/fusion-pro-now-available-free-for-personal-use.html if you do not have it already. (Note: VMware Fusion is available for Apple Silicon M chiip Macs, If you have trouble with this step, we encourage you to find a solution by yourself)
2. VM setup instructions (read very carefully): https://github.com/seed-labs/seed-labs/blob/master/lab-setup/apple-arm/seedvm-fusion.md
3. Go to [Lab Environment Setup page](https://seedsecuritylabs.org/labsetup.html) to install the VM (Ubuntu 22.04).
4. After building the VM, you can start the VM and log in with the username and password provided in the lab setup page.
5. Download the lab specific zip file (Labsetup-arm.zip) from the [lab page](https://seedsecuritylabs.org/Labs_20.04/Crypto/Crypto_Encryption/). You can download it directly on the VM or download it on your host machine and transfer it to the VM using the shared folder feature of VMware Fusion.
6. Unzip the setup file and start your lab.


## Lab Notices
* You can skip **Tasks 1, 6.2, 6.3 and 7**– frequency analysis against monoalphabetic substitution cipher and programming using the crypto library.
* Container setup is not required. You may ignore section *2 Lab Environment* of the lab manual.
* The original image, [pic_original.bmp](https://raw.githubusercontent.com/xyliatgithub/IntroCrypto2024/main/Lab%202/pic_original.bmp), is available in this GitHub repository. It is the image mentioned for Task 3.
* You can use any **bmp file** you found for Task 3 as long as you can see the differences when it is encrypted using ECB and CBC. Though [lena](https://github.com/Yu-Tsern/EN.650.658/blob/master/lab/lena_color.gif) is the standard testing image, it is not a good choice in this lab due to its complexity. Use some simple image that has large areas of same colors instead, such as [legoshi.bmp](https://raw.githubusercontent.com/xyliatgithub/IntroCrypto2024/main/Lab%202/legoshi.bmp). The header of pictures encrypted by ECB and CBC should be the same.
* For Task 5, you should consider the decryption processes for ECB, CBC, CFB and OFB.
* Include screenshots, original pictures, codes, IVs, keys you use in your report.
* Take screenshots periodically and include it in your report. They not only serve as evidences of completion but also help the grader understand what you're trying to achieve.

## Points Breakdown
This lab has 40 points in total. The five tasks (2, 3, 4, 5, 6.1) are worth 5, 10, 10, 10, 5 points respectively.

Note that **Task Number** is not the same as **Section Number**, for example: 
> 3 Task 1

Task 1 is in Section 3. Please use the **Task Number** in your report.

## Grading
* Completeness (25 pts): All the steps as instructed in the lab manual must be included in the report with adequate evidence.
* Presentation (15 pts): The report must be clear and correct in organization and writing with adequate explanation.
