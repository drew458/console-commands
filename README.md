# Unix
**Disclaimer:** Don't insert the square brackets when typing the command in the console, they are used here just for the sake of clarity.

## Basics  
* `/` (Forward Slash)   Top level directory  
* `.` (Single Period)	Current directory  
* `..` (Double Period)	Parent directory  
* `~` (Tilde)	Home directory  
* `sudo [command]`	Run command with the security privileges of the super user  
* `nano [file]`	Opens the Terminal editor  
* `open [file]`	Opens a file  
* `[command] -h`	Get help about a command  
* `man [command]`	Show the help manual of the command  

## Change Directory
* `cd`	Home directory  
* `cd [folder]`	Change directory, e.g. cd Documents  
* `cd ~`	Home directory  
* `cd/`	Root of the drive  
* `cd -`	Previous directory or folder you last browsed  
* `pwd`	Show your working directory  
* `cd..`	Move up to the parent directory  
* `cd../..`	Move up two levels  

## List Directory Contents  
* `ls`	Display the name of files and subdirectories in the directory  
* `ls -C`	Force multi-column output of the listing  
* `ls -a`	List all entries including those with .(period) and ..(double period)  
* `ls -1`	Output the list of files in one entry per line format  
* `ls -F`	Display a / (slash) immediately after each path that is a directory, * (asterisk) after executable programs or scripts, and @ after a symbolic link
* `ls -S`	Sort files or entries by size  
* `ls -l`	List in a long format. Includes file mode, owner and group name, date and time file was modified, pathname, and more  
* `ls -lt`	List the files sorted by time modified (most recent first)  
* `ls -lh`	Long listing with human readable file sizes in KB, MB, or GB  
* `ls -lo`	List the file names with size, owner, and flags  
* `ls -la`	List detailed directory contents, including hidden files  

## File Size and Disk Space
* `du`	List usage for each subdirectory and its contents
* `du -sh [folder]`	Human readable output of all files in a directory
* `du -s`	Display an entry for each specified file
* `du -sk* | sort -nr`	List files and folders, totaling the size including the subfolders. Replace sk* with sm* to list directories in MB
* `df -h`	Calculate your system's free disk space
* `df -H`	Calculate free disk space in powers of 1,000 (as opposed to 1,024)
* `lscpu`   Show cpu stats
* `lshw`    Show hardware stats
* `hwinfo`  Show hardware infos
* `inixi -Fx`   Show hardware info, beautifully wrapped
* `df` Show file system usage

## File and Directory Management
* `mkdir [dir]`	Create new folder named dir  
* `mkdir -p [dir/dir]`	Create nested folders  
* `mkdir [dir1] [dir2] [dir3]`	Create several folders at once  
* `mkdir ["dir"]`	Create a folder with a space in the filename  
* `rmdir [dir]`	Delete a folder (only works on empty folders)  
* `rm -R [dir]`	Delete a folder and its contents    
* `cp [file] [dir]`	Copy a file to the folder  
* `cp [file] [newfile]`	Copy a file to the current folder  
* `cp [file] [~/dir/newfile]`	Copy a file to the folder and rename the copied file  
* `cp -R [dir] ["new dir"]`	Copy a folder to a new folder with spaces in the filename  
* `cp -i [filedir]`	Prompts you before copying a file with a warning overwrite message  
* `cp [file1] [file2] [file3/dir]`	Copy multiple files to a folder  
* `rm [file]`	Delete a file (This deletes the file permanently; use with caution.)  
* `rm -i [file]`	Delete a file only when you give confirmation  
* `rm -f [file]`	Force removal without confirmation  
* `rm [file1] [file2] [file3]`	Delete multiple files without any confirmation  
* `mv [file] [newfilename]`	Move/rename  
* `mv [file] [dir]` Move a file to the folder, possibly by overwriting an existing file  
* `mv -i [file] [dir]`	Optional -i flag to warn you before overwriting the file  
* <strong>mv *.png [~/dir]</strong>	Move all PNG files from current folder to a different folder  
* `mdfind`  Spotlight search file  
* `open`    Open a file with desktop app

## Command History  
* `Ctrl + R`	Search through previously used commands  
* `history n`	Shows the previous commands you've typed Add a number to limit to the last n items  
* `![value]`	Execute the last command typed that starts with a value  
* `!!`	Execute the last command typed  

## Permissions  
* `ls -ld`	Display the default permission for a home directory  
* `ls -ld/[dir]`	Display the read, write, and access permission of a particular folder  
* `chmod 755 [file]`	Change the permission of a file to 755  
* `chmod -R 600 [dir]`	Change the permission of a folder (and its contents) to 600  
* `chown user:group [file]`	Change the ownership of a file to user and group. Add -R to include folder contents

## Processes & Statistics
* `ps -ax`	Output currently running processes. Here, a shows processes from all users and x shows processes that are not connected with the Terminal  
* `ps -aux`	Shows all the processes with %cpu, %mem, page in, PID, and command  
* `top`	Display live information about currently running processes  
* `htop`	See processes and memory stats  
* `top -ocpu -s 5`	Display processes sorted by CPU usage, updating every 5 seconds  
* `top -o rsize`	Sort top by memory usage
* `free` Show memory usage  
* `vmstat`  Report virtual memory statistics  
* `dstat, atop` Helps correlate all existing resource data for processes, memory, paging, block I/O, traps, and CPU activity.  
* `iftop` Interactive network traffic viewer per interface
* `nethogs` Interactive network traffic viewer per process  
* `iotop` Interactive I/O viewer  
* `iostat` For storage I/O statistics
* `sar` 
* `mpstat` For CPU statistics  
* `tload` Load average graph for terminal  
* `xload` Load average graph for X  
* `/proc/loadavg` Text file containing load average  
* `kill PID`	Quit process with ID PID. You'll see PID as a column in the Activity Monitor  
* `ps -ax | grep [appname]` Find a process by name or PID
* `factor`  Factor integers  

## Networking
* `ifconfig` Find your IP address
* `ping [host]`	Ping host and display status  
* `whois [domain]`	Output whois info for a domain  
* `curl -O [url/to/file]`	Download file via HTTP, HTTPS, or FTP  
* `ssh [username]@[host]`	Establish SSH connection to host with user username  
* `scp file[user]@[host]:[/remote/path]`	Copy file to a remote host  
* `nettop`	Display network activity  
* `traceroute [host]`	Display the packets route to the host   
* `dig [host]`	Simulate the domain name server
* `netstat` Show listening ports (deprecated)
* `ss` Show listening ports (successor to `netstat`)  
* `networkQuality`	macOS Monterey specific network quality test  

## Homebrew
* `brew doctor`	Check brew for potential problems
* `brew install [formula]`	Install a formula
* `brew uninstall [formula]`	Uninstall a formula
* `brew list`	List all the installed formulas
* `brew search`	Display available formulas for brewing
* `brew upgrade`	Upgrade all outdated and unpinned brews
* `brew update`	Fetch latest version of homebrew and formula
* `brew cleanup`	Remove older version of installed formula
* `brew tap homebrew/cask`	Tap the cask repository from GitHub
* `brew cask list`	List all installed casks
* `brew cask install [cask]`	Install the given cask
* `brew cask uninstall [cask]`	Uninstall the given cask

## Search
* `find dir -name ["file"]`	Find all files named file inside dir. Use wildcards (*) to search for parts of filenames
* `grep "[text]" [file]`	Output all occurrences of TEXT inside file (add -i for case insensitivity)
* `grep -rl "[text]" dir`	Search for all files containing TEXT inside dir
* `ls | grep "^abc"`    Find all the files with name starting with abc in the current directory

## Output
* `cat [file]`	Output the content of file
* `less [file]`	Output the contents of file using the less command that supports pagination and more
* `head [file]`	Output the first 10 lines of file

## Raspberry Pi hooks
* `sudo apt update` Update Package Lists
* `sudo apt upgrade` Download and Install Updated Packages
* `sudo apt clean` Clean Old Package Files
* `sudo raspi-config` The Raspberry Pi Configuration Tool
* `tree -d` Show a Tree of Directories
* `clear` Clear the Terminal Window
* `sudo halt` Shut Down a Raspberry Pi
* `sudo reboot` Restart a Raspberry Pi
* `startx` Start the Desktop Environment (LXDE)

## Specific Scripts
* `security find-generic-password -wa wifiname`	Show Wi-Fi password  
* `sudo powermetrics --samplers cpupower,gpupower,thermal,battery -i 1000 -o powermetricslog.txt`	Powermetrics logs into a file 
* `sudo powermetrics -s smc`	macOS specific get fan speed  
* `yes > /dev/null &`	Stress CPU  
* `find / -type f -name something.txt`    Searches for a file from root directory  
* `locate [filename]` Locate a file by name  
* `cat /dev/urandom`    Freeze the console with endless random stream output

# Win32

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