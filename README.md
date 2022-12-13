# CMPE283_Assignment_3



I had done it alone.

Initially, open the assignment 2 setup VM

Then, update cpuid.c and vmx.c as per the desired requirements

Thn use the following command "make -j 8 modules", (8 is number of CPU's, I have 8 in my VM. Find CPU's using "nproc" command)

Then use command "make -j 8".

Late, use command "sudo make INSTALL_MOD_STRIP=1 modules_install".

Then, Reboot the VM using a "sudo reboot"

Later, open the Virtual Machine created using virtual manager.

Then, create test.c file and run it to get required output.

Later, on the frequency of exits – does the number of exits increase at a stable rate? Or are there more exits performed during certain VM operations? Approximately how many exits does a full VM boot entail?

Here, 5116977 number of exits are not stable and keeps changing. 

-> Of the exit types defined in the SDM, which are the most frequent? Least?

Exit 48:EPT Violation, Exit 1: External Interrupt, Exit 30: IO Interrupt, Exit 32:WRMSR -> Most Frequently occuring. Exit 29: MOV DR, Exit 46: Access to IDTR, Exit 55 XSETBV -> Least Frequently occuring.
