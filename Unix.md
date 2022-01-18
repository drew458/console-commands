**Disclaimer:** Don't insert the square brackets when typing the command in the console, they are used here just for clarity.

## Basics  
* **/** _(Forward Slash)_   Top level directory  
* **.** _(Single Period)_	Current directory  
* **..** _(Double Period)_	Parent directory  
* **~** _(Tilde)_	Home directory  
* **sudo _[command]_**	Run command with the security privileges of the super user  
* **nano _[file]_**	Opens the Terminal editor  
* **open _[file]_**	Opens a file  
* **_[command]_ -h**	Get help about a command  
* **man _[command]_**	Show the help manual of the command  

## Change Directory
* **cd**	Home directory  
* **cd _[folder]_**	Change directory, e.g. cd Documents  
* **cd _~_**	Home directory  
* **cd/**	Root of the drive  
* **cd _-_**	Previous directory or folder you last browsed  
* **pwd**	Show your working directory  
* **cd..**	Move up to the parent directory  
* **cd../..**	Move up two levels  

## List Directory Contents  
* **ls**	Display the name of files and subdirectories in the directory  
* **ls _-C_**	Force multi-column output of the listing  
* **ls _-a_**	List all entries including those with .(period) and ..(double period)  
* **ls _-1_**	Output the list of files in one entry per line format  
* **ls _-F_**	Display a / (slash) immediately after each path that is a directory, * (asterisk) after executable   programs or scripts, and @ after a symbolic link
* **ls _-S_**	Sort files or entries by size  
* **ls _-l_**	List in a long format. Includes file mode, owner and group name, date and time file was modified, pathname, and more  
* **ls _-lt_**	List the files sorted by time modified (most recent first)  
* **ls _-lh_**	Long listing with human readable file sizes in KB, MB, or GB  
* **ls _-lo_**	List the file names with size, owner, and flags  
* **ls _-la_**	List detailed directory contents, including hidden files  

## File Size and Disk Space
* **du**	List usage for each subdirectory and its contents
* **du _-sh [folder]_**	Human readable output of all files in a directory
* **du _-s_**	Display an entry for each specified file
* <strong>du _-sk* | sort -nr_</strong>	List files and folders, totaling the size including the subfolders. Replace sk* with sm* to list directories in MB
* **df _-h_**	Calculate your system's free disk space
* **df _-H_**	Calculate free disk space in powers of 1,000 (as opposed to 1,024)
* **lscpu**   Show cpu stats
* **lshw**    Show hardware stats
* **hwinfo**  Show hardware infos
* **inixi _-Fx_**   Show hardware info, beautifully wrapped

## File and Directory Management
* **mkdir _[DIR]_**	Create new folder named DIR  
* **mkdir _-p [DIR/DIR]_**	Create nested folders  
* **mkdir _[DIR1] [DIR2] [DIR3]_**	Create several folders at once  
* **mkdir _["DIR"]_**	Create a folder with a space in the filename  
* **rmdir _[DIR]_**	Delete a folder (only works on empty folders)  
* **rm _-R [DIR]_**	Delete a folder and its contents    
* **cp _[FILE] [DIR]_**	Copy a file to the folder  
* **cp _[FILE] [NEWFILE]_**	Copy a file to the current folder  
* **cp _[FILE] [~/DIR/NEWFILE]_**	Copy a file to the folder and rename the copied file  
* **cp _-R [DIR] ["new dir"]_**	Copy a folder to a new folder with spaces in the filename  
* **cp _-i [FILEDIR]_**	Prompts you before copying a file with a warning overwrite message  
* **cp _[FILE1] [FILE2] [FILE3/DIR]_**	Copy multiple files to a folder  
* **rm _[FILE]_**	Delete a file (This deletes the file permanently; use with caution.)  
* **rm _-i [FILE]_**	Delete a file only when you give confirmation  
* **rm _-f [FILE]_**	Force removal without confirmation  
* **rm _[FILE1] [FILE2] [FILE3]_**	Delete multiple files without any confirmation  
* **mv _[FILE] [NEWFILENAME]_**	Move/rename  
* **mv _[FILE] [DIR]_** Move a file to the folder, possibly by overwriting an existing file  
* **mv _-i [FILE] [DIR]_**	Optional -i flag to warn you before overwriting the file  
* <strong>mv _*.png [~/DIR]_</strong>	Move all PNG files from current folder to a different folder  
* **mdfind**  Spotlight search file  
* **open**    Open a file with desktop app

## Command History  
* **Ctrl + R**	Search through previously used commands  
* **history n**	Shows the previous commands you've typed Add a number to limit to the last n items  
* **![value]**	Execute the last command typed that starts with a value  
* **!!**	Execute the last command typed  

## Permissions  
* **ls _-ld_**	Display the default permission for a home directory  
* **ls _-ld/[DIR]_**	Display the read, write, and access permission of a particular folder  
* **chmod _755 [FILE]_**	Change the permission of a file to 755  
* **chmod _-R 600 [DIR]_**	Change the permission of a folder (and its contents) to 600  
* **chown _USER:GROUP [FILE]_**	Change the ownership of a file to user and group. Add -R to include folder contents

## Processes & Statistics
* **ps _-ax_**	Output currently running processes. Here, a shows processes from all users and x shows processes that are not connected with the Terminal  
* **ps _-aux_**	Shows all the processes with %cpu, %mem, page in, PID, and command  
* **top**	Display live information about currently running processes  
* **htop**	See processes and memory stats  
* **top _-ocpu -s 5_**	Display processes sorted by CPU usage, updating every 5 seconds  
* **top _-o rsize_**	Sort top by memory usage  
* **vmstat**  Report virtual memory statistics  
* **dstat, atop** Helps correlate all existing resource data for processes, memory, paging, block I/O, traps, and CPU activity.  
* **iftop** Interactive network traffic viewer per interface
* **nethogs** Interactive network traffic viewer per process  
* **iotop** Interactive I/O viewer  
* **iostat** For storage I/O statistics  
* **netstat** For network statistics  
* **mpstat** For CPU statistics  
* **tload** Load average graph for terminal  
* **xload** Load average graph for X  
* **/proc/loadavg** Text file containing load average  
* **kill _PID_**	Quit process with ID _PID_. You'll see PID as a column in the Activity Monitor  
* **ps _-ax | grep [APPNAME]_** Find a process by name or PID
* **factor**  Factor integers  

## Networking
* **ping _[HOST]_**	Ping host and display status  
* **whois _[DOMAIN]_**	Output whois info for a domain  
* **curl _-O [url/to/file]_**	Download file via HTTP, HTTPS, or FTP  
* **ssh _[username]@[host]_**	Establish SSH connection to _host_ with user _username_  
* **scp _FILE[user]@[host]:[/remote/path]_**	Copy _FILE_ to a remote _host_  
* **nettop**	Display network activity  
* **traceroute _[host]_**	Display the packets route to the host   
* **dig _[host]_**	Simulate the domain name server  **networkQuality**	macOS Monterey specific network quality test    

## Homebrew
* **brew _doctor_**	Check brew for potential problems
* **brew _install [formula]_**	Install a formula
* **brew _uninstall [formula]_**	Uninstall a formula
* **brew _list_**	List all the installed formulas
* **brew _search_**	Display available formulas for brewing
* **brew _upgrade_**	Upgrade all outdated and unpinned brews
* **brew _update_**	Fetch latest version of homebrew and formula
* **brew _cleanup_**	Remove older version of installed formula
* **brew _tap homebrew/cask_**	Tap the cask repository from GitHub
* **brew _cask list_**	List all installed casks
* **brew _cask install [cask]_**	Install the given cask
* **brew _cask uninstall [cask]_**	Uninstall the given cask

## Search
* **find _DIR -name ["FILE"]_**	Find all files named _FILE_ inside _DIR_. Use wildcards (*) to search for parts of filenames
* **grep _"[TEXT]" [FILE]_**	Output all occurrences of _TEXT_ inside FILE (add -i for case insensitivity)
* **grep _-rl "[TEXT]" DIR_**	Search for all files containing _TEXT_ inside _DIR_
* **ls | grep _"^abc"_**    Find all the files with name starting with abc in the current directory

## Output
* **cat _[FILE]_**	Output the content of _FILE_
* **less _[FILE]_**	Output the contents of _FILE_ using the less command that supports pagination and more
* **head _[FILE]_**	Output the first 10 lines of _FILE_

## Raspberry Pi hooks
* **sudo apt _update_** Update Package Lists
* **sudo apt _upgrade_** Download and Install Updated Packages
* **sudo apt _clean_** Clean Old Package Files
* **sudo raspi-config** The Raspberry Pi Configuration Tool
* **tree _-d_** Show a Tree of Directories
* **clear** Clear the Terminal Window
* **sudo _halt_** Shut Down a Raspberry Pi
* **sudo _reboot_** Restart a Raspberry Pi
* **startx** Start the Desktop Environment (LXDE)
* **ifconfig** Find a Raspberry Pi's IP Address


## Specific Scripts
* **security _find-generic-password -wa wifiname_**	Show Wi-Fi password  
* **sudo powermetrics _--samplers cpu_power,gpu_power,thermal,battery -i 1000 -o powermetrics_log.txt_**	Powermetrics logs into a file 
* **sudo powermetrics _-s smc_**	macOS specific get fan speed  
* **yes _> /dev/null &_**	Stress CPU  
* **find _/ -type f -name something.txt_**    Searches for a file from root directory  
* **locate _[FILENAME]_** Locate a file by name  
* **cat _/dev/urandom_**    Freeze the console with endless random stream output