## Lab 1 - Pseudo Random Number Generation
In this [lab](https://seedsecuritylabs.org/Labs_20.04/Files/Crypto_Random_Number/Crypto_Random_Number.pdf), you will apply your knowledge in class to find out some interesting facts and do some experiments on crypto programming. You need to complete all the five tasks in this lab and submit a detailed lab report, with screenshots, to describe what you have done and what you have observed with necessary explanation. Please refer to the example report. Please include important code snippets followed by explanation. Simply attaching code without any explanation will receive no credits.


## Lab Enviroment
The lab is one of the exercises in SEED Labs. It uses a [Virtual Machine](https://seedsecuritylabs.org/labsetup.html) (VM) to simplify the experiment setup. Load the VM image with your VirtualBox or VMware (whichever you prefer). [Here](https://github.com/seed-labs/seed-labs/blob/master/manuals/vm/seedvm-manual.md) is the manual to install the VM on your computer. Please read the VM [User Manual](https://web.ecs.syr.edu/~wedu/seed/Documentation/Ubuntu16_04_VM/Ubuntu16_04_VM_Manual.pdf) (which is for an older version, but basically same) carefully before you start working on the labs.


## Environment Setup

### Intel/AMD (x86-64)

1. Download and install [VirtualBox](https://www.virtualbox.org/wiki/Downloads).
2. Download the [pre-built SEED Ubuntu 20.04 VirtualBox image](https://seedsecuritylabs.org/labsetup.html).
3. Follow the [SEED Lab Manual](https://github.com/seed-labs/seed-labs/blob/master/manuals/vm/seedvm-manual.md) to load the VM image in VirtualBox and complete the VM setup.
4. Start your VM and log in with the default credentials `seed:dees`.

### Apple Silicon (ARM64)
**Note that the Ubuntu image download link in the instructions no longer works. Download [22.04.5 LTS](https://cdimage.ubuntu.com/releases/jammy/release/) (No GUI) or [24.10](https://cdimage.ubuntu.com/daily-live/current/) (Use this if you don't know what the previous is) instead**

**Currently not support lab 1**: Due to the higher kernel version on Ubuntu 22.04 , the [random number generator](https://github.com/seed-labs/seed-labs/blob/master/lab-setup/apple-arm/Notes/Crypto.md#random-number) works different on ARM VM 22.04. If you are working on lab 1, we suggest switching to windows or using machines in MSSI lab.      
**Using VMware Fusion Player**: VirtualBox does not fully support our SEED Ubuntu 20.04 VM on Apple Silicon machines (M chips). We recommend using **VMware Fusion Player** to set up the lab VM.  

1. Download and install [VMware Fusion Player](https://blogs.vmware.com/teamfusion/2024/05/fusion-pro-now-available-free-for-personal-use.html) (free).
2. Download the [Ubuntu 22.04 ISO image](https://cdimage.ubuntu.com/jammy/daily-live/current/) for the operating system. Be sure to select the **64-bit ARM (ARMv8/AArch64)** version.
3. Follow the instructions for [Apple Silicon Machines](https://github.com/seed-labs/seed-labs/blob/master/lab-setup/apple-arm/seedvm-fusion.md) to create an Ubuntu 22.04 VM on VMware Fusion Player and complete the VM setup.
4. Start your VM and log in with the default credentials `seed:dees` (if not changed).

## Troubleshooting
* If the `Enable Nested VT-x/AMD-V` checkbox is grayed out in VirtualBox, try running the command `VBoxManage modifyvm "VM_NAME" --nested-hw-virt` on to enable it.
* If you are using a chip with arm architecture, you could download UTM instead of virtual box. You need to create a VM from scratch. Follow this [link](https://mac.getutm.app/gallery/ubuntu-20-04) and download ths iso from [here](https://cdimage.ubuntu.com/releases/20.04/release/). Also, you need to follow the [steps](https://github.com/seed-labs/seed-labs/blob/master/manuals/vm/seedvm-from-scratch.md) of building from scratch in Seed. (Remember to correct your local time in VM, otherwise you might get the wrong answers for this lab.)
* If you are still having trouble setting up the environment, you can perform lab activities on the [MSSI Lab](https://wiki.isi.jhu.edu/index.php/Category:MSSI_Lab) workstations located in Malone 316.

## Useful Instructions
The lab description has the step-by-step walkthrough and detailed instruction. Here are some additional hints and notices:
* The VM image is an archive of vmdk files. VirtualBox users can follow the instruction in the [User Manual](https://github.com/seed-labs/seed-labs/blob/master/manuals/vm/seedvm-manual.md) to import those files. For VMware user, please refer to this [video](https://www.youtube.com/watch?v=1g7qkozxh4o&ab_channel=Magazie) for lab setup.
* In Task 2, you need to implement an AES-128-CBC program to perform encryption. Python is recommended here since you may use libraries like Crypto, pycrypto or cryptography to simplify the task. However, it is also acceptable to use any other languages. Just remember to attach the code with enough explanation.
* The plaintext, ciphertext and IV provided in Task 2, together with the key you generate in Task 1, are all hexadecimal codes. Conversion may be applied to handle them in your program.
* The question at the end of Task 4 is optional.
* The 256-bit key in the last step is supposed to be a binary string (sequence of 0s and 1s of length 256).
* Please take screenshots periodically and regularly and include them in your report. They not only serve as evidence of completion but also help the grader understand what you try to achieve.
* Please attach your code with adequate explanation for each task in your report to receive full credits. See the example for what it should look like.

## Points Break Down
This lab has 40 points in total. Task 1 through Task 5 are worth 5, 15, 5, 5, 10 points respectively.

## Submission Details
* You will work in a team.
* Only one report is accepted from each group. Please list group members in your report explicitly.
* Please type your solutions. In general NO hand-written report is accepted.

## Grading
* Completeness (25 pts): All the steps as instructed in the lab manual must be included in the report with adequate evidence.
* Presentation (15 pts): The report must be clear and correct in organization and writing with adequate explanation.
