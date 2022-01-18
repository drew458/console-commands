**Disclaimer:** Don't insert the square brackets when typing the command in the console, they are used here just for the sake of clarity.  
**Disclaimer:** All the commands are compatible with PowerShell, only a subset is compatible with CMD.

## Generic
* `call`		Calls a batch file from another one  
* `cd`		Change directory  
* `cls`		Clear screen  
* `cmd`		Start command prompt  
* `color`		Change console color  
* `date`		Show/set date  
* `dir`		List directory content  
* `echo`		Text output  
* `exit`		Exits the command prompt or a batch file  
* `find`		Find files  
* `hostname`	Display host name  
* `pause`		Pauses the execution of a batch file and * shows a message  
* `runas`		Start a program as another user  
* `shutdown`	Shutdown the computer  
* `sort`		Sort the screen output  
* `start`		Start an own window to execute a program or command  
* `taskkill`	Terminate a process or a application  
* `tasklist`	Display applications and related tasks  
* `time`		Display/edit the system time  
* `timeout`		Wait any time  
* `title`		Set title for prompt  
* `ver`		Display operating system version  
* `w32tm`		Setting time synchronisation/time server/time zone  

## Networking
* `ftp`		Transfer files to a FTP server  
* `ftype`		Display file type and mapping  
* `getmac`		Sisplay MAC address  
* `ipconfig`	Sisplay IP network settings  
* `netsh`		Configure/control/display network components  
* `netstat`		Display TCP/IP connections and status  
* `nslookup`	Query the DNS  
* `pathping`	Test the connection to a specific IP address  
* `ping [domainname]`		Pings the network  
* `route`		Display network routing table, add static routes  
* `systeminfo`	Displays computer-specific properties and configurations  
* `telnet`		Establish Telnet connection  
* `tftp`		Transfer files to a TFTP server  
* `tracert [domainname]`		Trace routes similar to patchping  
* `arp -a`		Display network addresses  
* `nslookup [domainname]`	Simulate the domain name server  

## File/Directory operations
* `attrib`		Display file attributes  
* `comp`		Compare file contents  
* `compact`	Display/change file compression  
* `copy / xcopy`	Copy files  
* `diskcomp`	Compare content of two floppy disks  
* `diskcopy`	Copy floppy disc to another one  
* `erase / del`	Delete one or more files  
* `expand`		Extract files  
* `fc`	Compare files and display the differences  
* `mkdir`		Create a new directory  
* `move`		Move/rename files  
* `rename`		Rename files  
* `replace`		Replace files  
* `rmdir / rd`	Delete directory  
* `tree`		Display folder structure graphically  
* `type`		Display content of text files  

## I/O and Disks
* `chkdsk`		Check volumes  
* `chkntfs`		Display/change volume check at startup  
* `sfc`	System file scan  
* `defrag`		Defragment media  
* `diskpart`	Volume management  
* `driverquery`	Display installed devices and their properties  
* `format`		Format volumes  
* `label`		Change volume name  
* `mode`		Configure interfaces/devices  
* `mountvol`	Assign/delete drive mountpoints  
* `verify`		Monitoring whether volumes are written correctly  
* `vol`		Show volume description and serial numbers of the HDDs  
* `powercfg`	Energy and battery reports and options  

## PowerShell scripting
* `for`		for loop  
* `gpresult`	Display group policies  
* `gpupdate`	Update group policies  
* `perfmon`		Start performance monitor  
* `prompt`		Change command prompt  
* `reg`		Add/read/import/export registry entries  

## Specific scripts
* In a batch file (.bat) ->	`:main   start	goto main`  
(Possible one line console execution of script above)  
`:main & start & goto main`  
* `shutdown -s -t 60`  
* `while (1) { ps | sort -desc cpu | select -first 30; sleep-seconds 2; cls }` top command equivalent in Windows
