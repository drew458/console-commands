**Disclaimer:** Don't insert the square brackets when typing the command in the console, they are used here just for clarity.  
**Disclaimer:** All the commands are compatible with PowerShell, only a subset is compatible with CMD.

## Generic
* **call**		calls a batch file from another one  
* **cd**		change directory  
* **cls**		clear screen  
* **cmd**		start command prompt  
* **color**		change console color  
* **date**		show/set date  
* **dir**		list directory content  
* **echo**		text output  
* **exit**		exits the command prompt or a batch file  
* **find**		find files  
* **hostname**	display host name  
* **pause**		pauses the execution of a batch file and * shows a message  
* **runas**		start a program as another user  
* **shutdown**	shutdown the computer  
* **sort**		sort the screen output  
* **start**		start an own window to execute a program or command  
* **taskkill**	terminate a process or a application  
* **tasklist**	display applications and related tasks  
* **time**		display/edit the system time  
* **timeout**		wait any time  
* **title**		set title for prompt  
* **ver**		display operating system version  
* **w32tm**		setting time synchronisation/time server/time zone  

## Networking
* **ftp**		transfer files to a FTP server  
* **ftype**		display file type and mapping  
* **getmac**		display MAC address  
* **ipconfig**	display IP network settings  
* **netsh**		configure/control/display network components  
* **netstat**		display TCP/IP connections and status  
* **nslookup**	query the DNS  
* **pathping**	test the connection to a specific IP address  
* **ping _[domainname]_**		pings the network  
* **route**		display network routing table, add static routes  
* **systeminfo**	displays computer-specific properties and configurations  
* **telnet**		establish Telnet connection  
* **tftp**		transfer files to a TFTP server  
* **tracert _[domainname]_**		trace routes similar to patchping  
* **arp _-a_**		display network addresses  
* **nslookup _[domainname]_**	simulate the domain name server  

## File/Directory operations
* **attrib**		display file attributes  
* **comp**		compare file contents  
* **compact**	display/change file compression  
* **copy / xcopy**	copy files  
* **diskcomp**	compare content of two floppy disks  
* **diskcopy**	copy floppy disc to another one  
* **erase / del**	delete one or more files  
* **expand**		extract files  
* **fc**	copare files and display the differences  
* **mkdir**		create a new directory  
* **move**		move/rename files  
* **rename**		rename files  
* **replace**		replace files  
* **rmdir / rd**	delete directory  
* **tree**		display folder structure graphically  
* **type**		display content of text files  

## I/O and Disks
* **chkdsk**		check volumes  
* **chkntfs**		display/change volume check at startup  
* **sfc**	System file scan  
* **defrag**		defragment media  
* **diskpart**	volume management  
* **driverquery**	display installed devices and their properties  
* **format**		format volumes  
* **label**		change volume name  
* **mode**		configure interfaces/devices  
* **mountvol**	assign/delete drive mountpoints  
* **verify**		monitoring whether volumes are written correctly  
* **vol**		show volume description and serial numbers of the HDDs  
* **powercfg**	energy and battery reports and options  

## PowerShell scripting
* **for**		for loop  
* **gpresult**	display group policies  
* **gpupdate**	update group policies  
* **perfmon**		start performance monitor  
* **prompt**		change command prompt  
* **reg**		add/read/import/export registry entries  

## Specific scripts
* batch file	->	**:main   start	goto main**  
(Possible one line console execution of script above)  
**:main & start & goto main**  
* **shutdown _-s -t 60_**  
* **while (1) { ps | sort -desc cpu | select -first 30; sleep-seconds 2; cls }** top command equivalent in Windows