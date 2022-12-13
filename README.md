# 283Assignment3
1.For each member in your team, provide 1 paragraph detailing what parts of the lab that member implemented / researched.

I have done it alone. 

Steps
1.Take the assignment 2 setup VM

modify cpuid.c and vmx.c as per assignment 3 requirements

Fire command "make -j 8 modules", (8 is number of CPU's, I have 8 in my VM. Find CPU's using "nproc" command)

After above step,fire command "make -j 8".

After above step, fire command "sudo make INSTALL_MOD_STRIP=1 modules_install".

Reboot VM using "sudo reboot"

Open the VM created using virtual manager.

Crate test.c file and run it to get required output.

3.Comment on the frequency of exits – does the number of exits increase at a stable rate? Or are there more exits performed during certain VM operations? Approximately how many exits does a full VM boot entail?

Approximately 5116977. Number of exits are not stable and keeps changing. It depends on the activities performed on VM.

4.Of the exit types defined in the SDM, which are the most frequent? Least?

Exit 48:EPT Violation, Exit 1: External Interrupt, Exit 30: IO Interrupt, Exit 32:WRMSR -> Most Frequently occuring. Exit 29: MOV DR, Exit 46: Access to IDTR, Exit 55 XSETBV -> Least Frequently occuring.
