# TASK 3
## Part1
1. How many states could has a process in Linux?
   - **Foreground processes** lso referred to as interactive processes) – these are initialized and
controlled through a terminal session. In other words, there has to be a user connected to the
system to start such processes; they haven’t started automatically as part of the system
functions/services.
   - **Background processes** (also referred to as non-interactive/automatic processes) – are processes
not connected to a terminal; they don’t expect any user input.
2. Examine the **pstree** command. Make output (highlight) the chain (ancestors) of the current process.


![000_pstree]()
- when use this command we can see all tree of process with pearent and child process.
3. What is a **proc** file system?
- The **proc filesystem (procfs)** is a **special filesystem** in Unix-like operating systems that presents information about processes and other system information in a hierarchical file-like structure, providing a more convenient and standardized method for dynamically accessing process data held in the kernel than traditional tracing methods or direct access to kernel memory. 
4. Print information about the processor (its type, supported technologies, etc.).
- Use to prit information **cat /proc/cpuinfo** to see all information about currient core, of processor.

![002_CPUINFO]()
5. Use the **ps aux** *command* to get information about the process. 

![001_ps_aux]()
6. How to define kernel processes and user processes?
- User-space processes have its own virtual address space. **Kernel processes** or threads **do not have their own address space**, they operate within kernel address space only.
7. Print the list of processes to the terminal. Briefly describe the statuses of the processes.
What condition are they in, or can they be arriving in?
![003_top]()

8. Display only the processes of a specific user.![004_ps]()
9. What utilities can be used to analyze existing running tasks (by analyzing the help for the ps command)?
- **ps aux; ps fax**
10. What information does top command display?
- **PID; USER; %CPU; %MEMORY; %Virtual address;
12. Display the processes of the specific user using the top command. ![005_top_spec_user]()
12. What interactive commands can be used to control the top command? Give a couple of examples.![006_interactive_command]()
13. Sort the contents of the processes window using various parameters (for example, the
amount of processor time taken up, etc.)
14. Concept of priority, what commands are used to set priority?
- press **k** input priority **20>**
15.  Can I change the priority of a process using the top command.
16. Examine the kill command. How to send with the kill command process control signal? Give an example of commonly used signals.
- ![007_kill_sig]()
17. Commands jobs, fg, bg, nohup. What are they for? Use the sleep, yes command to demonstrate the process control mechanism with fg, bg.
- This commands use to move process from foreground / bakground / sleep
## Part2
1. Check the implementability of the most frequently used OPENSSH commands in the MS
Windows operating system. (Description of the expected result of the commands +
screenshots: command – result should be presented)
2. Implement basic SSH settings to increase the security of the client-server connection (at least
3. List the options for choosing keys for encryption in SSH. Implement 3 of them.
4. Implement port forwarding for the SSH client from the host machine to the guest Linux
virtual machine behind NAT.
5*. Intercept (capture) traffic (tcpdump, wireshark) while authorizing the remote client on the
server using ssh, telnet, rlogin. Analyze the result.
