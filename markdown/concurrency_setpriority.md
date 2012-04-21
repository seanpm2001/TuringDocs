
#Concurrency.setpriority

##Syntax
**setpriority** (*p* : **nat**)

##Description
The **setpriority** procedure is used to set the priority of a process in a concurrent program.  This priority cannot  be counted on to guarantee critical access to shared variables.  A smaller value of *p* means increased speed.  The argument to **setpriority** may be limited to the range 0 to 2**15 - 1.

##Status
Part of the language and only conceptually part of the **Concurrency** unit. 
This means that you can only call the function by calling **setpriority**, not by calling **Concurrency.setpriority**.

##See also
**[getpriority.html](getpriority), [fork.html](fork) **and **[monitor.html](monitor)**.