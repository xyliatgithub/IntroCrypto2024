## Lab 1 - Pseudo Random Number Generation
In this [lab](https://seedsecuritylabs.org/Labs_20.04/Files/Crypto_Random_Number/Crypto_Random_Number.pdf), you will apply your knowledge in class to find out some interesting facts and do some experiments on crypto programming. You need to complete all the five tasks in this lab and submit a detailed lab report, with screenshots, to describe what you have done and what you have observed with necessary explanation. Please include important code snippets followed by explanation. Simply attaching code without any explanation will receive no credits.

The lab is one of the exercises in SEED Project. It uses a Virtual Machine (VM) [image](https://seedsecuritylabs.org/labsetup.html) in order to simplify the experiment setup. We are using the Ubuntu 20.04 image for this lab. Load the VM image with your VirtualBox or VMware (whichever you prefer). [Here](https://github.com/seed-labs/seed-labs/blob/master/manuals/vm/seedvm-manual.md) is the manual to install the VM on your computer. Please read the VM [User Manual](https://web.ecs.syr.edu/~wedu/seed/Documentation/Ubuntu16_04_VM/Ubuntu16_04_VM_Manual.pdf) (which is for an older version, but basically same) carefully before you start working on the labs.

## Special Notice for Non-x86 Chip
A computer with a Non-x86 Chip(Apple M chips, Snapdragon) may not be able to use the pre-build SEED Lab Ubuntu20.04 image.
* SEED Lab provided special instruction for [Apple Silicon Machine](https://github.com/seed-labs/seed-labs/blob/master/lab-setup/apple-arm/seedvm-fusion.md)
* If you are using a chip with arm architecture, you could download UTM instead of virtual box. You need to create a VM from scratch. Follow this [link](https://mac.getutm.app/gallery/ubuntu-20-04) and download ths iso from [here](https://cdimage.ubuntu.com/releases/20.04/release/). Also, you need to follow the [steps](https://github.com/seed-labs/seed-labs/blob/master/manuals/vm/seedvm-from-scratch.md) of building from scratch in Seed. (Remember to correct your local time in VM, otherwise you might get the wrong answers for this lab.)
* MSSI students can perform lab activity in the [MSSI Lab](https://wiki.isi.jhu.edu/index.php/Category:MSSI_Lab) Workstations.

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
* Only one report is needed from each group. Please list group members in your report explicitly.
* Please type your solutions. In general NO hand-written report is accepted.

## Grading
* Completeness (25 pts): All the steps as instructed in the lab manual must be included in the report with adequate evidence.
* Presentation (15 pts): The report must be clear and correct in organization and writing with adequate explanation.
